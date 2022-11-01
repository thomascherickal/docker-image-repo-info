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
-	[`caddy:2.6`](#caddy26)
-	[`caddy:2.6-alpine`](#caddy26-alpine)
-	[`caddy:2.6-builder`](#caddy26-builder)
-	[`caddy:2.6-builder-alpine`](#caddy26-builder-alpine)
-	[`caddy:2.6-builder-windowsservercore-1809`](#caddy26-builder-windowsservercore-1809)
-	[`caddy:2.6-builder-windowsservercore-ltsc2022`](#caddy26-builder-windowsservercore-ltsc2022)
-	[`caddy:2.6-windowsservercore`](#caddy26-windowsservercore)
-	[`caddy:2.6-windowsservercore-1809`](#caddy26-windowsservercore-1809)
-	[`caddy:2.6-windowsservercore-ltsc2022`](#caddy26-windowsservercore-ltsc2022)
-	[`caddy:2.6.2`](#caddy262)
-	[`caddy:2.6.2-alpine`](#caddy262-alpine)
-	[`caddy:2.6.2-builder`](#caddy262-builder)
-	[`caddy:2.6.2-builder-alpine`](#caddy262-builder-alpine)
-	[`caddy:2.6.2-builder-windowsservercore-1809`](#caddy262-builder-windowsservercore-1809)
-	[`caddy:2.6.2-builder-windowsservercore-ltsc2022`](#caddy262-builder-windowsservercore-ltsc2022)
-	[`caddy:2.6.2-windowsservercore`](#caddy262-windowsservercore)
-	[`caddy:2.6.2-windowsservercore-1809`](#caddy262-windowsservercore-1809)
-	[`caddy:2.6.2-windowsservercore-ltsc2022`](#caddy262-windowsservercore-ltsc2022)
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
$ docker pull caddy@sha256:d3e5e175b10a2a5b66be9570ed9867aeb77af8eca7a14b6033dcde2c9f6fee6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3532; amd64
	-	windows version 10.0.20348.1129; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:7992b931b7da3cf0840dd69ea74b2c67d423faf03408da8abdc31b7590a239a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17676993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:006d393a4e6a01f82413e41b3e0f06dfb1872d5ca6a37aba315e4ec9e2cc6c4c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:34:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 04:34:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 01:43:19 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 01:43:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 01:43:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 01:43:22 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 01:43:22 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 01:43:22 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 01:43:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 80
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 443
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 01:43:24 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 01:43:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5625668cf98fd3e4d769f18d45f27e34fe3d085cfb9927ff7ad2cdc84d8c493f`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 304.5 KB (304517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675d09b34c5347b62625d31b2a458824240b90e51d18bcc38ad37d317e83d64c`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1747be7065842ba85f86aed65e75608dfd2f546ab9d8ecd4a8842c8f4634795`  
		Last Modified: Fri, 14 Oct 2022 01:43:47 GMT  
		Size: 14.6 MB (14560435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8ee6c4c21d12cd28fcd0e196acb8569f35518dc36c691c91b4c8ca1928bf9d`  
		Last Modified: Fri, 14 Oct 2022 01:43:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:76b70e0dc74358fc1f7ef178c46cc9c047a90cd05e842d26305da1ee04ff3ad8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16834877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cac02415934eaae38be5b122f6a0c760f747e6f50f1551c9a45f4f186454f04`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 19:49:23 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 27 Oct 2022 19:49:25 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 27 Oct 2022 19:49:25 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 27 Oct 2022 19:49:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 27 Oct 2022 19:49:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 19:49:28 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 27 Oct 2022 19:49:28 GMT
ENV XDG_DATA_HOME=/data
# Thu, 27 Oct 2022 19:49:28 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 27 Oct 2022 19:49:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 80
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 443
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 443/udp
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 2019
# Thu, 27 Oct 2022 19:49:30 GMT
WORKDIR /srv
# Thu, 27 Oct 2022 19:49:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7f6197b1f089356a6bff8bf29fdcef692051048bd17db70d72df822c89c04d`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 304.4 KB (304404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc91cb09da181c7973089ccf7aca9c7830c738ac1e614883f86c2eecdcb68002`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 5.8 KB (5751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ffb96b75d9dc6019cfe6202b9fed588b3ff9a91cc89237d6a24c98eb5fd590`  
		Last Modified: Thu, 27 Oct 2022 19:50:36 GMT  
		Size: 13.9 MB (13910603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb4866598fa794379095b277b41d4b0cb626d61cc20c6f6cff7d920bc99330`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9df5bfbadaf5495675c4de47918d3631d439d159681e352069eaa206f664a8ac
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16617541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d61e1121278866d5afee597ba2ac37a9b5bec51b6323b551fe9a89b5d99d63e5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 10:30:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 27 Oct 2022 10:30:41 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 27 Oct 2022 10:30:41 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 27 Oct 2022 10:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 27 Oct 2022 10:30:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 10:30:45 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 27 Oct 2022 10:30:45 GMT
ENV XDG_DATA_HOME=/data
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 27 Oct 2022 10:30:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 80
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 443
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 443/udp
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 2019
# Thu, 27 Oct 2022 10:30:46 GMT
WORKDIR /srv
# Thu, 27 Oct 2022 10:30:46 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9f1011ebc9810d3e61468e7ce6c2866fc65920db06e3bccde2da749f976500`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 303.5 KB (303537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28310071f60503f30048b0cad1abe85c763c57dd4e69715cc57d60560481318`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 5.8 KB (5753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7792abbee8ad8ec28f7e6e2864a9e8ad229de5f701ba4bf04be77cffac8835ac`  
		Last Modified: Thu, 27 Oct 2022 10:31:39 GMT  
		Size: 13.9 MB (13891032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c5be986b3fadf5f34a0a4311ffa6a22b4f1f0ff79c510fb7c58cb93c64e2f3`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f06fb46d2c67f3b7f9447b6c19f5b9909931b603d2b475f647624f577c6d94ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16278669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8876f25c7ec7330d6bf197e452e3a37deeea42e52b8c2b2c9103bc86b26795`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 26 Oct 2022 18:53:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 Oct 2022 18:53:58 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Wed, 26 Oct 2022 18:53:58 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 26 Oct 2022 18:54:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 Oct 2022 18:54:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 Oct 2022 18:54:01 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 Oct 2022 18:54:01 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 80
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 443
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 443/udp
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 2019
# Wed, 26 Oct 2022 18:54:02 GMT
WORKDIR /srv
# Wed, 26 Oct 2022 18:54:02 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5532e6e746eecf0e890ee17251a52841dd55694ae55c919dc6ddf6159e27cd5b`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 304.5 KB (304512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b816658ad2f9debd81f6df21dd733e54fc6eda530080cc3957e6f63d9677b9a`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d7ee92d83c49ca71b5440fd76d22ac6b75304bc48a0183bf392689ae8d5897`  
		Last Modified: Wed, 26 Oct 2022 18:54:26 GMT  
		Size: 13.3 MB (13260508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00da94c60a7ed1fc9acd392aedea2ab7b2bd6a7d67cc83b2d5d85c5cbd40090b`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:9665c6fd33be967b3bdfcdbeeb605e3a92e70080ef5caa8907a6cbdef064be3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (16031232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96553401995800bf37590502c237b4ab8cee57bd3885e83f76dcb42c53a7d7db`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:56:10 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 07:56:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 03:47:38 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 03:47:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 03:47:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 03:47:44 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 03:47:44 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 03:47:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 03:47:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 80
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 443
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 03:47:49 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 03:47:49 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 03:47:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf49ba2a5c90a152d4aef09519c7019835fbf2884d6afb1c85b3353b7d91388e`  
		Last Modified: Fri, 07 Oct 2022 07:57:09 GMT  
		Size: 306.5 KB (306522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dac87aba8912de3ce6fb3ca14bb6833f931fd15d7ec2d7435a18f11e5ddb6fb`  
		Last Modified: Fri, 07 Oct 2022 07:57:08 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea24f9a44c53fbd359328daff2e10e4e3f1c7d7bae21190ea2f6af3be43dd0b`  
		Last Modified: Fri, 14 Oct 2022 03:48:33 GMT  
		Size: 12.9 MB (12915404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4704e2ddccf987da9605ef1c8d4ef68a86cf3e6ba2f8c5d1e80e5915481e25c`  
		Last Modified: Fri, 14 Oct 2022 03:48:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:5702e27172b1bfb5e9930d544d7cf16a83f774419b1aa2078be464351ff5f70b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16967685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05ec4a186bcadcf0e691a443c7edebf42d46cff3997d01a56de43db0ecbab8e2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 10:23:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 10:23:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 00:55:05 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 00:55:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 00:55:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 00:55:15 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 00:55:16 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 00:55:17 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 00:55:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 00:55:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 00:55:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 00:55:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 00:55:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 00:55:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 00:55:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 00:55:22 GMT
EXPOSE 80
# Fri, 14 Oct 2022 00:55:22 GMT
EXPOSE 443
# Fri, 14 Oct 2022 00:55:23 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 00:55:23 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 00:55:24 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 00:55:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5123e0e5a47a6dfbd8cae1e2589df59b198f82ba790c211aeb3eefbbe41a17be`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 304.8 KB (304752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557f08048878eca2f16fd3b05bb138300739b9e74e467509792efc4278e74b3f`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91158060b74650f434cb3419f6ed862b0616480567b651bfae73b297f69b9992`  
		Last Modified: Fri, 14 Oct 2022 00:56:22 GMT  
		Size: 14.1 MB (14066352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511ac9f174e3fed802157937e9192a940800d73835958de90f5a363b5edf46ad`  
		Last Modified: Fri, 14 Oct 2022 00:56:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.3532; amd64

```console
$ docker pull caddy@sha256:c795b26fccceaa3ea3738c3d086e0c9da9978392aeb6e2c69ae3d71131b88998
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726785951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a0ffc50daa8e99f5d3029bd930601ec939b66a180da1ad5fef783d1fcb69eb3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 16:58:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:14:49 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:16:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:16:10 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:16:11 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:16:12 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:16:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:16:14 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:16:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:16:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:16:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:16:19 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:16:20 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:16:21 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:16:22 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:17:16 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:17:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:028c482fad0f111537a40f65401f65de54c9fd682951a4f8cf9b644d7c128e18`  
		Size: 834.0 MB (833997855 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77462c8fbd8b2782ee2fc5f09bebfb350912f754186b058478ab8d22f50bb047`  
		Last Modified: Wed, 12 Oct 2022 17:04:34 GMT  
		Size: 358.2 KB (358248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a372be4d9f43d4d5884bc4093c44aedf12150f55ea9457baa2fcceb43ef8074`  
		Last Modified: Thu, 13 Oct 2022 23:21:08 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a8993c29bb6d4c31b0be3609bc7fb2af2666435fe70bb2f329784277d629d1`  
		Last Modified: Thu, 13 Oct 2022 23:21:11 GMT  
		Size: 14.9 MB (14947938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98662b730099437011356fa77ef9072054f4ad73d3781e9b02d4750689762162`  
		Last Modified: Thu, 13 Oct 2022 23:21:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7e77f6a080ad6fa8a7320831868ccd7b6385e995988f2e6cca76090a565c99`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec71d29d036cab0bdbc7765216513aad527933ededfec4492a97724c6bab52d`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a11bac4631094c366303dd3c571fe04cf1b543bafba72d8dd1030f8ae2ec185`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4dc588cdabd0672f8b29c59cd9ddc6d927160284a6f6529fbe39b8e34ca766`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f39777f21d48153f681f16b5a1cd2e12440066bc96a665fa3b85a6275b74942`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638736df2ba6ceaed21b97ee12046d2d0494561bd735581618ab505ff602b0da`  
		Last Modified: Thu, 13 Oct 2022 23:21:04 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e0fe53dba785fdf61d7431392d7e15beeebbe5f215d9a2de2ee00975e7b5c4`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb7b8fc42485b0656b2afcb99344cda044ce10d0107cc91955fbe11433c358`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb8f166931be4f8f0b0a07611df01a8e7d1101f8a8ce564144ded43917e1021`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bc6f4b7a114b7722cfc81aa83b74727261766c2cef9bc0787e447435c33d2a`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5563ab3963680a40da3bc2269bbc1e76362b359547dae9705892cf8f54b50dd1`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d300f0320cd2b8ce3f3e58cbb3acb06e24c5f59a342725056a10667329f914`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfb9dfa0b00914a255876439613219f4a74e83734df6b8a197e6e0bb53bf905`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b9233dbf203ca77eea2271813856d219ba7d2f633adf99f3262612edfad738`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 291.8 KB (291836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefde31b509f056641749adae4daa4e0ad3265d260ac1c61b41c8950a10824e6`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.20348.1129; amd64

```console
$ docker pull caddy@sha256:e1e15c80e157d71221ec43035cae93b3ea8ba7a6b203428e93159aa6ff5e1463
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2432333411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbd806ca24dfacee0d098f111cc9f6d5f42fdbd9db91a63a8de0d048d3984d5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 17:01:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:17:37 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:18:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:18:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:18:13 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:18:13 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:18:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:18:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:18:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:18:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:18:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:18:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:18:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:18:21 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:18:22 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:18:23 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:18:24 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:18:40 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:18:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ab91661ce2a2a2c14684a2ba0f543a81d7896773f88200b31be0e37c589de38`  
		Size: 979.4 MB (979359717 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cd84a277fd91a008fe0c8fc7d6706544075a294512940b16f57998588ea892`  
		Last Modified: Wed, 12 Oct 2022 17:04:58 GMT  
		Size: 616.9 KB (616893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b069dfbedeca0437916f85fdd78a598955839b91ffc4cba4d6327e5c79487`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5263d846656ffa3662062b1a58d9c6d114e00fa5344edc9b93ea5895c4fa46`  
		Last Modified: Thu, 13 Oct 2022 23:21:34 GMT  
		Size: 15.1 MB (15149356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e378404d94c7fb280c51201d60aef05af3196a0ead3b716521cedbe766ba5e3e`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11749bcf2c3e4097f9a1a30d1fc22184e48c94ab54945730c51c36be175c668d`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cb14f39fa0dce5d6dab4bdd1a896c02b5a6bba01dcd46ed36928c2cce27295`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf622a21cfc36d8958be2f273f52b7d4824d500be08f6a2de791506dcc6c981f`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b246af35953d05f1c4292cb1cf8cfc29215ceac2e013ae2a0759aa2d216516`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08367cd2562c20737156e692dca481f835f4832fabb63602fb5edc78494057ae`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6d70510bf329eff739580f04b59acba9cb4aa74e57bcb6fca996d6df6b6d2c`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc6e963fa5949ceb99519a652299dea21a92c9389aadabedb2deeb4e51855b5`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d175d8244325a62c683c4d1fa6cc266f73231f93142fd0f52c3378da6db1464`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4ce9495075c9b00994ef154c9eb0974ba1853a8244869e35af4eecfca4dce7`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceee07aab1c573de692984f7655da9e6c4aee31260b8df8735344242e6f1ff8`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295041dd24e85177aaf7e1bbd1c0b032d2eafaf3da59213972894238dd5b3d72`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3583f031f13dfd9a933b6e8d4808a3ac7f3e007d2e751af9581b76b08b6e0c4a`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1603973d06c7b0a01ab165d727b40f842361ce898a8e7b8579d6bd9db938c8a6`  
		Last Modified: Thu, 13 Oct 2022 23:21:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c4bf5f410b0a58ef5b477fdf99b90ad01e7deb85b685cf06eaae5c9d83a531`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 319.8 KB (319842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da4c854489e4317220200f8dca47e2335696fe8fa9e7a2aa678467b12b4db7b`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:0e3c6d476eb251d2e271c61d12472698e2be1909626d342c405ed58c70772857
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
$ docker pull caddy@sha256:7992b931b7da3cf0840dd69ea74b2c67d423faf03408da8abdc31b7590a239a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17676993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:006d393a4e6a01f82413e41b3e0f06dfb1872d5ca6a37aba315e4ec9e2cc6c4c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:34:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 04:34:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 01:43:19 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 01:43:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 01:43:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 01:43:22 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 01:43:22 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 01:43:22 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 01:43:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 80
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 443
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 01:43:24 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 01:43:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5625668cf98fd3e4d769f18d45f27e34fe3d085cfb9927ff7ad2cdc84d8c493f`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 304.5 KB (304517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675d09b34c5347b62625d31b2a458824240b90e51d18bcc38ad37d317e83d64c`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1747be7065842ba85f86aed65e75608dfd2f546ab9d8ecd4a8842c8f4634795`  
		Last Modified: Fri, 14 Oct 2022 01:43:47 GMT  
		Size: 14.6 MB (14560435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8ee6c4c21d12cd28fcd0e196acb8569f35518dc36c691c91b4c8ca1928bf9d`  
		Last Modified: Fri, 14 Oct 2022 01:43:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:76b70e0dc74358fc1f7ef178c46cc9c047a90cd05e842d26305da1ee04ff3ad8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16834877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cac02415934eaae38be5b122f6a0c760f747e6f50f1551c9a45f4f186454f04`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 19:49:23 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 27 Oct 2022 19:49:25 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 27 Oct 2022 19:49:25 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 27 Oct 2022 19:49:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 27 Oct 2022 19:49:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 19:49:28 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 27 Oct 2022 19:49:28 GMT
ENV XDG_DATA_HOME=/data
# Thu, 27 Oct 2022 19:49:28 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 27 Oct 2022 19:49:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 80
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 443
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 443/udp
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 2019
# Thu, 27 Oct 2022 19:49:30 GMT
WORKDIR /srv
# Thu, 27 Oct 2022 19:49:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7f6197b1f089356a6bff8bf29fdcef692051048bd17db70d72df822c89c04d`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 304.4 KB (304404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc91cb09da181c7973089ccf7aca9c7830c738ac1e614883f86c2eecdcb68002`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 5.8 KB (5751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ffb96b75d9dc6019cfe6202b9fed588b3ff9a91cc89237d6a24c98eb5fd590`  
		Last Modified: Thu, 27 Oct 2022 19:50:36 GMT  
		Size: 13.9 MB (13910603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb4866598fa794379095b277b41d4b0cb626d61cc20c6f6cff7d920bc99330`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9df5bfbadaf5495675c4de47918d3631d439d159681e352069eaa206f664a8ac
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16617541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d61e1121278866d5afee597ba2ac37a9b5bec51b6323b551fe9a89b5d99d63e5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 10:30:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 27 Oct 2022 10:30:41 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 27 Oct 2022 10:30:41 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 27 Oct 2022 10:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 27 Oct 2022 10:30:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 10:30:45 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 27 Oct 2022 10:30:45 GMT
ENV XDG_DATA_HOME=/data
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 27 Oct 2022 10:30:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 80
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 443
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 443/udp
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 2019
# Thu, 27 Oct 2022 10:30:46 GMT
WORKDIR /srv
# Thu, 27 Oct 2022 10:30:46 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9f1011ebc9810d3e61468e7ce6c2866fc65920db06e3bccde2da749f976500`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 303.5 KB (303537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28310071f60503f30048b0cad1abe85c763c57dd4e69715cc57d60560481318`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 5.8 KB (5753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7792abbee8ad8ec28f7e6e2864a9e8ad229de5f701ba4bf04be77cffac8835ac`  
		Last Modified: Thu, 27 Oct 2022 10:31:39 GMT  
		Size: 13.9 MB (13891032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c5be986b3fadf5f34a0a4311ffa6a22b4f1f0ff79c510fb7c58cb93c64e2f3`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f06fb46d2c67f3b7f9447b6c19f5b9909931b603d2b475f647624f577c6d94ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16278669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8876f25c7ec7330d6bf197e452e3a37deeea42e52b8c2b2c9103bc86b26795`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 26 Oct 2022 18:53:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 Oct 2022 18:53:58 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Wed, 26 Oct 2022 18:53:58 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 26 Oct 2022 18:54:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 Oct 2022 18:54:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 Oct 2022 18:54:01 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 Oct 2022 18:54:01 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 80
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 443
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 443/udp
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 2019
# Wed, 26 Oct 2022 18:54:02 GMT
WORKDIR /srv
# Wed, 26 Oct 2022 18:54:02 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5532e6e746eecf0e890ee17251a52841dd55694ae55c919dc6ddf6159e27cd5b`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 304.5 KB (304512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b816658ad2f9debd81f6df21dd733e54fc6eda530080cc3957e6f63d9677b9a`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d7ee92d83c49ca71b5440fd76d22ac6b75304bc48a0183bf392689ae8d5897`  
		Last Modified: Wed, 26 Oct 2022 18:54:26 GMT  
		Size: 13.3 MB (13260508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00da94c60a7ed1fc9acd392aedea2ab7b2bd6a7d67cc83b2d5d85c5cbd40090b`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:9665c6fd33be967b3bdfcdbeeb605e3a92e70080ef5caa8907a6cbdef064be3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (16031232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96553401995800bf37590502c237b4ab8cee57bd3885e83f76dcb42c53a7d7db`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:56:10 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 07:56:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 03:47:38 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 03:47:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 03:47:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 03:47:44 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 03:47:44 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 03:47:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 03:47:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 80
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 443
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 03:47:49 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 03:47:49 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 03:47:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf49ba2a5c90a152d4aef09519c7019835fbf2884d6afb1c85b3353b7d91388e`  
		Last Modified: Fri, 07 Oct 2022 07:57:09 GMT  
		Size: 306.5 KB (306522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dac87aba8912de3ce6fb3ca14bb6833f931fd15d7ec2d7435a18f11e5ddb6fb`  
		Last Modified: Fri, 07 Oct 2022 07:57:08 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea24f9a44c53fbd359328daff2e10e4e3f1c7d7bae21190ea2f6af3be43dd0b`  
		Last Modified: Fri, 14 Oct 2022 03:48:33 GMT  
		Size: 12.9 MB (12915404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4704e2ddccf987da9605ef1c8d4ef68a86cf3e6ba2f8c5d1e80e5915481e25c`  
		Last Modified: Fri, 14 Oct 2022 03:48:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:5702e27172b1bfb5e9930d544d7cf16a83f774419b1aa2078be464351ff5f70b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16967685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05ec4a186bcadcf0e691a443c7edebf42d46cff3997d01a56de43db0ecbab8e2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 10:23:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 10:23:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 00:55:05 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 00:55:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 00:55:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 00:55:15 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 00:55:16 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 00:55:17 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 00:55:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 00:55:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 00:55:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 00:55:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 00:55:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 00:55:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 00:55:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 00:55:22 GMT
EXPOSE 80
# Fri, 14 Oct 2022 00:55:22 GMT
EXPOSE 443
# Fri, 14 Oct 2022 00:55:23 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 00:55:23 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 00:55:24 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 00:55:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5123e0e5a47a6dfbd8cae1e2589df59b198f82ba790c211aeb3eefbbe41a17be`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 304.8 KB (304752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557f08048878eca2f16fd3b05bb138300739b9e74e467509792efc4278e74b3f`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91158060b74650f434cb3419f6ed862b0616480567b651bfae73b297f69b9992`  
		Last Modified: Fri, 14 Oct 2022 00:56:22 GMT  
		Size: 14.1 MB (14066352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511ac9f174e3fed802157937e9192a940800d73835958de90f5a363b5edf46ad`  
		Last Modified: Fri, 14 Oct 2022 00:56:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:9a395d60c9cba0036b919495f7637be3fafb0a97459ee970f1738e0252dfa2f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3532; amd64
	-	windows version 10.0.20348.1129; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:735ad7b9a5ba5baf3df5f93034af5fa90c3554da9725d260df238d2511be6b23
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133519902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4fa387ebb822f454dc9877bfe19aaba627e1b422f476a4952468eb35c419c3f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 21:16:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 21:16:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 21:16:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:20:19 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:21:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:21:57 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:21:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:21:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:21:57 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:49:49 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:49:49 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:49:49 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:49:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:49:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:49:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:49:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4583459ba0371c715f926a9bbd37a9dae909234f4b898220160425131eb53bd4`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 284.7 KB (284734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c1e223e6f2123b855e0c95898eba50cb6a055881ba9023527c0a361761c1cf`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbef1b99e503551b709afdb24ef66954c0792f99d76bb0018afd3a65a1347b5b`  
		Last Modified: Tue, 01 Nov 2022 19:30:19 GMT  
		Size: 122.3 MB (122275572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99825e86aac9391fd3d709522864ff3282479450067b8431df9c4f9e4da4da1`  
		Last Modified: Tue, 01 Nov 2022 19:30:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd6f4fde4a1bb5cc5dd5adba9566a8e0e11ac8cf06adffd9dbefe69a80fc50e`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 6.9 MB (6937644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc2cb786c4d70bac77de2092dd9d3fe5b54e59daa8918ccd6ce64d32929e339`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 1.2 MB (1215184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189da6bcd6c18118e6c5774a9bf9eaba6cde20b87848c17960d265f518beb280`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2b94490e7740d5762996c3f1af82a99c3a298122ab46f5312d75b015ed07fdb3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129501509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:484eab50c7b23327b3246fbfe1577b2cb318df92dd5e1e7695611bc34588a965`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 01 Nov 2022 18:49:34 GMT
RUN apk add --no-cache ca-certificates
# Tue, 01 Nov 2022 18:49:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Nov 2022 18:49:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:49:35 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:51:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:51:57 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:51:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:51:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:51:58 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:18:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:18:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:18:14 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:18:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:18:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:18:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:18:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e34adf14e74afbe714188593430596566b859daec67932063af22ae26cfb41`  
		Last Modified: Tue, 01 Nov 2022 18:59:56 GMT  
		Size: 284.6 KB (284604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30829221241bb1a4c4b78ced30216bd6e772290df6d02b43de82ec13847f2ea`  
		Last Modified: Tue, 01 Nov 2022 18:59:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5175fa50505ed8e1ebb1cc778186a5571aceaf68880fb7f30ce0a002543fde16`  
		Last Modified: Tue, 01 Nov 2022 19:00:18 GMT  
		Size: 118.6 MB (118633129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9462914fb6be31fa7883e2ac24e0b90c77b0dd01eed92e5eb2717d2d58757a21`  
		Last Modified: Tue, 01 Nov 2022 18:59:55 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bae57654f3779f11c3403f04b1e6edc1160b85b75ec1b7aaeebd3ab918fdb3e`  
		Last Modified: Tue, 01 Nov 2022 19:19:10 GMT  
		Size: 6.8 MB (6806143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ccbb51616839b72199c780dc3fb4b40d6337c1b64a8e503b85e43d17ae6bee`  
		Last Modified: Tue, 01 Nov 2022 19:19:09 GMT  
		Size: 1.2 MB (1162983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8bf63e08652d8b6f6f6f0710daa4bfdfd8cd8a9b63599b309be0e046fb2405`  
		Last Modified: Tue, 01 Nov 2022 19:19:09 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:38e0977df61d81ad978adc5aeff5351e967c86e79faa8b7707674d0ac2e63774
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128321867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0724d3115962e959325f2a9a4a8824cd2292a204ddd5db99808f8c1c3b28610a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 03:11:14 GMT
RUN apk add --no-cache ca-certificates
# Thu, 27 Oct 2022 03:11:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 03:11:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:58:35 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:00:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:00:36 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:00:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:00:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:00:37 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:30:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:30:18 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:30:18 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:30:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:30:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:30:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:30:20 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb4eb882dd734293a28e32a55182efac09a590954d1c7e0ac4e9afd668b950f`  
		Last Modified: Thu, 27 Oct 2022 03:23:31 GMT  
		Size: 283.8 KB (283751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62601eba0f2135ba01bd7632b6cd5858fd87c654ebbd7aa446022efda221518`  
		Last Modified: Thu, 27 Oct 2022 03:23:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f8cf932723cb79c6511c7a4565c26fc3c1a8b195b63a1b4f27567664469b8`  
		Last Modified: Tue, 01 Nov 2022 19:11:07 GMT  
		Size: 118.4 MB (118395001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06295a7c5807cf45167f1a47e93084873628c3417ae38bd41c276b71ba1c46ab`  
		Last Modified: Tue, 01 Nov 2022 19:10:45 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92d8ff62b16b450357e75981f8b6277cddab5a79836683195be024c5b466eb1`  
		Last Modified: Tue, 01 Nov 2022 19:31:14 GMT  
		Size: 6.1 MB (6065387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136c853b146e693b550c1d68b6b6713b79d7befffc79acb1530b83593b8fa935`  
		Last Modified: Tue, 01 Nov 2022 19:31:13 GMT  
		Size: 1.2 MB (1159979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f924d6193ccce35a47a6ee295f40e327abf4a8492374030689faf3f505632e08`  
		Last Modified: Tue, 01 Nov 2022 19:31:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6b8569ece82b11e5f6720884af16dce90859af84c6a9ab271ce05a08435fbd77
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127999797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1543ea235e3a8ec3d0ad049bdc81b95745b72848028c6dbc10cde12da0b876fc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 26 Oct 2022 08:09:57 GMT
RUN apk add --no-cache ca-certificates
# Wed, 26 Oct 2022 08:09:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 Oct 2022 08:09:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:40:17 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:41:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:41:34 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:41:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:41:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:41:35 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:05:53 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:05:53 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:05:53 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:05:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:05:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:05:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:05:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d82f9e3411d2eff49049d09ae871e53b96a0cc7dd335883f1fec28c43f9c86`  
		Last Modified: Wed, 26 Oct 2022 08:17:16 GMT  
		Size: 284.7 KB (284723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e169736571560c1a3278f9971532d55ddc4abfaef12e8c54c05f4644445d5520`  
		Last Modified: Wed, 26 Oct 2022 08:17:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc530f9a61e7c0e16b1cb3d48b70136b625cf624976acc638b9d6aef5525995`  
		Last Modified: Tue, 01 Nov 2022 18:48:07 GMT  
		Size: 116.8 MB (116836732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562d55c2123be45d40bfd4dd4dea65161ad3d83b50153de3cc0b63ec7a061f4b`  
		Last Modified: Tue, 01 Nov 2022 18:47:54 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90594629b6df4d09d221ea3fc570b4944e36520a3503ffa3a838772b0e46561`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 7.0 MB (7049481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e41bd715f5f0d05c59b600661a8f0cfb5145de632b14a77d012cfd1ffeea780`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 1.1 MB (1120483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3da6b029e0d694358fe69ed7435eb464495babb3bc51d3d5f30a5222406935`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:0bfdd9fd29aabe5e64b1c692ef01a8064dc2c4932747c3bf06363fd238817630
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128911035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3d666ccc1132e45cb0e54d7fd1891ab309ad3ae1fa96a20556f67f531c4bcc0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:26:01 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:26:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:26:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:17:13 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:19:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:20:03 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:20:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:20:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:20:05 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:50:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:50:46 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:50:46 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:50:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:50:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:50:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:50:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36899d7325c2c25a7d8e61ef33bb1e93b83f811f462e9ddad81c86df87b0685`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 286.7 KB (286747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9309524edda98df2abd6704c6f56004422a28b63364f028763ea000fc32d6eca`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b608654249afe5c44e2b3f100f6b333302506cd24adc46afa3302bb03ff96e`  
		Last Modified: Tue, 01 Nov 2022 19:31:59 GMT  
		Size: 117.2 MB (117238077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93311758f4ff1a16fa50dab5c51c12dd47a1920496e07493f5452c97e24eff9c`  
		Last Modified: Tue, 01 Nov 2022 19:31:32 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce6b57ae4a73b81094351a45358cebcbfbccd4d0d31ab77e71afc97d675dc63`  
		Last Modified: Tue, 01 Nov 2022 19:51:34 GMT  
		Size: 7.5 MB (7478322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5fa9d97b98179c5269f7f488f5488ec1a31fa543c75dc88705c8ed0a755e1c`  
		Last Modified: Tue, 01 Nov 2022 19:51:33 GMT  
		Size: 1.1 MB (1103853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f6efc0777ee24d394842b20cc0fe8c229ae5fecbb8dbb5537e66f5fc1fcf41`  
		Last Modified: Tue, 01 Nov 2022 19:51:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:660f4e58ece536977f580dad53c004e3fe9b1496a0af262adf93a8480746e615
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131825256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d3b89f5e95a2acfe27efc6ab49664e2a25268891a03b26100d1cca071938a79`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:16:09 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:16:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:16:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:43:10 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:46:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:47:10 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:47:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:47:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:47:13 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:20:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:20:25 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:20:26 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:20:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:20:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:20:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:20:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d31ae2e1f77c70a25e9cbeea435b4ab68149a4e17f9d4668768da8dd5ac68a`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 285.0 KB (284954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2788e533105e3c00ed84523a8f99d7947c0bb8b12932018a3081ecc29964605`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a12f83dfb1b48c3152a859b9b55b4483128b0be37e4877271cbd453b23fb43`  
		Last Modified: Tue, 01 Nov 2022 19:02:36 GMT  
		Size: 120.7 MB (120729474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e663873bb0a71689aee0be3ce5f4195e0b573039585fcc3182fe189e8e8fe05`  
		Last Modified: Tue, 01 Nov 2022 19:02:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802d29971118d482599687d5c1f1c069a8f0b8cb0c96e3ec3d5f550416223491`  
		Last Modified: Tue, 01 Nov 2022 19:21:20 GMT  
		Size: 7.1 MB (7052072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eea39f6b8018dc8d0011d05cdf7f2412b1435fdedc607d0087cfb9c631ccc23`  
		Last Modified: Tue, 01 Nov 2022 19:21:19 GMT  
		Size: 1.2 MB (1167444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a34c766fedcef740b10fddb96cd1ffd7aeae2d9628ddfa2510fedd4bbe64d2b`  
		Last Modified: Tue, 01 Nov 2022 19:21:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.3532; amd64

```console
$ docker pull caddy@sha256:f279c274451500e517aada07ecabddffd03b23f0b9d81791d2347e369b267a6f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2958579667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c57c677f08a022815e25e725365624f628555a00eab2b42f1830e71794c949`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 12:45:06 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Oct 2022 12:45:07 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Oct 2022 12:45:08 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Oct 2022 12:45:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Oct 2022 12:46:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Oct 2022 12:46:38 GMT
ENV GOPATH=C:\go
# Wed, 12 Oct 2022 12:47:37 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 01 Nov 2022 19:19:52 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:25:48 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 01 Nov 2022 19:25:50 GMT
WORKDIR C:\go
# Tue, 01 Nov 2022 20:18:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 01 Nov 2022 20:18:12 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 20:18:13 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 20:18:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 20:19:33 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 01 Nov 2022 20:19:34 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094a4c27e78f8821517fd551cd9e3d5f4b1e4199bdcd783b3fbda849e4995ad1`  
		Last Modified: Wed, 12 Oct 2022 13:16:26 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e91de5ff2103556b1048388473379f95d41247701f0911ebc7c530a861f3f5e`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52642f9e5e3a52bef8ee5677bcb62a364e07003da51f16eb28b8a4ce34fe9f7d`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26528ba698d400f5680be93457d24581b9e4e7a2399de7bb23cbd549f206613`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c89703eb31300a2a39c85ce287a6b9fe88da033828368275bdbb53c2f7704c`  
		Last Modified: Wed, 12 Oct 2022 13:16:30 GMT  
		Size: 25.4 MB (25439927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8705eaae12fa4840be2d79e376eb1b4b7b18da881acad2892b1c47336e796f46`  
		Last Modified: Wed, 12 Oct 2022 13:16:19 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebda8897c2727e3b971c947385632df6f19de06da75e9f161200d43d1acf714`  
		Last Modified: Wed, 12 Oct 2022 13:16:19 GMT  
		Size: 315.0 KB (315035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8667d37dce62bb077cd534d490f047b61dfe9c30023659258862cada9cbd0ba`  
		Last Modified: Tue, 01 Nov 2022 19:54:40 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac8e32e89f1739964a644b8b8b5b44bbae9752f8ea1f87e93455ca36cc86a7d`  
		Last Modified: Tue, 01 Nov 2022 19:55:33 GMT  
		Size: 157.7 MB (157676844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cabbd4ff51bc72ab20efd9f4eb4ebb788679ef03c2fc9b8a72f711fe3558590`  
		Last Modified: Tue, 01 Nov 2022 19:54:40 GMT  
		Size: 1.5 KB (1459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a7aa6766a51e2f5a5add77b40fd7eafa9d3d5049c3b4506b6b4e6dffb65cd6`  
		Last Modified: Tue, 01 Nov 2022 20:21:08 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54feb136a1e02e5d213be9750ca621c39022ff48f54c1e67daace9a82dd241f1`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7c0ce28f0f06a413d72723dbca806a7b025194983d436501cb04b7b2d7379`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e48594ab78eca9cfe42619a2f721de764c027be8fa22700565227c765b4ed7e`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55feb68cd00871cb13079eb862d65521274326d062594c7522edcc8f9bac23f1`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.6 MB (1631634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d398f623f33e057b5d399473e3ee1243fef32140e9a4411c1f69a913b43acb08`  
		Last Modified: Tue, 01 Nov 2022 20:21:05 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.20348.1129; amd64

```console
$ docker pull caddy@sha256:6e35c0ddda3afe05cb015c908260022b09ae192d81ad72f3bf1e32c70d7cb243
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2659936170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:265570f6cf9dffda304fb3a6712c85940e0f8d23ef6d8ffbfd8e1ebdd6d89d85`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 12:40:52 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Oct 2022 12:40:53 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Oct 2022 12:40:54 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Oct 2022 12:40:55 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Oct 2022 12:41:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Oct 2022 12:41:26 GMT
ENV GOPATH=C:\go
# Wed, 12 Oct 2022 12:41:47 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 01 Nov 2022 19:15:18 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:19:35 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 01 Nov 2022 19:19:38 GMT
WORKDIR C:\go
# Tue, 01 Nov 2022 20:19:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 01 Nov 2022 20:19:43 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 20:19:45 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 20:19:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 20:20:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 01 Nov 2022 20:20:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e9b54b31e104f64c9eb8a65ac0af5effd645bd00a77ea297b6015d28022a74`  
		Last Modified: Mon, 17 Oct 2022 21:39:11 GMT  
		Size: 1000.0 MB (1000028645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f8b589252b90e37349f39b9d4495646791b4050d7cd218336fcc4624b0ebe2`  
		Last Modified: Wed, 12 Oct 2022 13:15:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811ef63d5261b55ee6b499dbc7fcd1ed13386326466fb81a0801abbcbcb75d3f`  
		Last Modified: Wed, 12 Oct 2022 13:15:28 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816740cd643a7a4e72aa527cd033d0c95686c9725ff70dac3260b44dce508e73`  
		Last Modified: Wed, 12 Oct 2022 13:15:28 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599e30c8b316e75d786cfd91f97b9fae4c89fb00f3fce0619eb4e66bc3165521`  
		Last Modified: Wed, 12 Oct 2022 13:15:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77a0d37b81c920d4b783c0b2cfad656a4b8733960ba3afd4e0a1f39f202f948`  
		Last Modified: Wed, 12 Oct 2022 13:15:32 GMT  
		Size: 25.7 MB (25689345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b699f53b56e90279b0bb8ce4434f9b68bbc28fa30756476e22c7ef3dc869e24a`  
		Last Modified: Wed, 12 Oct 2022 13:15:21 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57fcf632f60c89dd981a8a7fa084e738f55129b1786fd9a9e9f5ab8aa1e02d82`  
		Last Modified: Wed, 12 Oct 2022 13:15:24 GMT  
		Size: 526.5 KB (526519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8b0d888223c93af8f0c84ad35156f79df9b0d9ae107f61ded320d2a4fed5f3`  
		Last Modified: Tue, 01 Nov 2022 19:53:29 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49602de12fff655f45d03b1befdd7e56321771c65ed690492e4092da51046bb3`  
		Last Modified: Tue, 01 Nov 2022 19:54:22 GMT  
		Size: 157.8 MB (157838831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cb5ede4eaf1f86f7c0957639a8b53a0c6740df6fa395d3d286e32bff6b9195`  
		Last Modified: Tue, 01 Nov 2022 19:53:29 GMT  
		Size: 1.6 KB (1584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d0ae347408d32205a9ca4c0628e814833984ac8c0fbfb6c6687b9c94a733aa`  
		Last Modified: Tue, 01 Nov 2022 20:21:30 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453489637085324b6412fd9d83cc639d7a9f9135fb5db5dec214462b3293c98f`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cc23fcabe43926f14c7d7e786e9175c87fe573e41fc0158bdc02cfc08fb567`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528f2dc5e38ba5bad570845252c13446ea9637f9c7a80590c93c28886ab79803`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd45b40a0e40f3a52f9a7e2e1cf3cf3b0501ca3f8d637ef46596ee30a9193264`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.8 MB (1837122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bd243dcf25ec803b906e53fa263b2803735773f0227c1c4bac5d52654bb8c6`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:9a51f1a1098ec283efeb9174633447c4bb3142e5bbc7649c8ced7f8d685da3f4
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
$ docker pull caddy@sha256:735ad7b9a5ba5baf3df5f93034af5fa90c3554da9725d260df238d2511be6b23
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133519902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4fa387ebb822f454dc9877bfe19aaba627e1b422f476a4952468eb35c419c3f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 21:16:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 21:16:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 21:16:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:20:19 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:21:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:21:57 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:21:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:21:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:21:57 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:49:49 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:49:49 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:49:49 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:49:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:49:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:49:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:49:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4583459ba0371c715f926a9bbd37a9dae909234f4b898220160425131eb53bd4`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 284.7 KB (284734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c1e223e6f2123b855e0c95898eba50cb6a055881ba9023527c0a361761c1cf`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbef1b99e503551b709afdb24ef66954c0792f99d76bb0018afd3a65a1347b5b`  
		Last Modified: Tue, 01 Nov 2022 19:30:19 GMT  
		Size: 122.3 MB (122275572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99825e86aac9391fd3d709522864ff3282479450067b8431df9c4f9e4da4da1`  
		Last Modified: Tue, 01 Nov 2022 19:30:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd6f4fde4a1bb5cc5dd5adba9566a8e0e11ac8cf06adffd9dbefe69a80fc50e`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 6.9 MB (6937644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc2cb786c4d70bac77de2092dd9d3fe5b54e59daa8918ccd6ce64d32929e339`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 1.2 MB (1215184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189da6bcd6c18118e6c5774a9bf9eaba6cde20b87848c17960d265f518beb280`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2b94490e7740d5762996c3f1af82a99c3a298122ab46f5312d75b015ed07fdb3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129501509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:484eab50c7b23327b3246fbfe1577b2cb318df92dd5e1e7695611bc34588a965`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 01 Nov 2022 18:49:34 GMT
RUN apk add --no-cache ca-certificates
# Tue, 01 Nov 2022 18:49:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Nov 2022 18:49:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:49:35 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:51:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:51:57 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:51:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:51:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:51:58 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:18:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:18:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:18:14 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:18:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:18:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:18:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:18:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e34adf14e74afbe714188593430596566b859daec67932063af22ae26cfb41`  
		Last Modified: Tue, 01 Nov 2022 18:59:56 GMT  
		Size: 284.6 KB (284604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30829221241bb1a4c4b78ced30216bd6e772290df6d02b43de82ec13847f2ea`  
		Last Modified: Tue, 01 Nov 2022 18:59:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5175fa50505ed8e1ebb1cc778186a5571aceaf68880fb7f30ce0a002543fde16`  
		Last Modified: Tue, 01 Nov 2022 19:00:18 GMT  
		Size: 118.6 MB (118633129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9462914fb6be31fa7883e2ac24e0b90c77b0dd01eed92e5eb2717d2d58757a21`  
		Last Modified: Tue, 01 Nov 2022 18:59:55 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bae57654f3779f11c3403f04b1e6edc1160b85b75ec1b7aaeebd3ab918fdb3e`  
		Last Modified: Tue, 01 Nov 2022 19:19:10 GMT  
		Size: 6.8 MB (6806143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ccbb51616839b72199c780dc3fb4b40d6337c1b64a8e503b85e43d17ae6bee`  
		Last Modified: Tue, 01 Nov 2022 19:19:09 GMT  
		Size: 1.2 MB (1162983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8bf63e08652d8b6f6f6f0710daa4bfdfd8cd8a9b63599b309be0e046fb2405`  
		Last Modified: Tue, 01 Nov 2022 19:19:09 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:38e0977df61d81ad978adc5aeff5351e967c86e79faa8b7707674d0ac2e63774
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128321867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0724d3115962e959325f2a9a4a8824cd2292a204ddd5db99808f8c1c3b28610a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 03:11:14 GMT
RUN apk add --no-cache ca-certificates
# Thu, 27 Oct 2022 03:11:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 03:11:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:58:35 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:00:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:00:36 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:00:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:00:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:00:37 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:30:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:30:18 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:30:18 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:30:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:30:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:30:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:30:20 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb4eb882dd734293a28e32a55182efac09a590954d1c7e0ac4e9afd668b950f`  
		Last Modified: Thu, 27 Oct 2022 03:23:31 GMT  
		Size: 283.8 KB (283751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62601eba0f2135ba01bd7632b6cd5858fd87c654ebbd7aa446022efda221518`  
		Last Modified: Thu, 27 Oct 2022 03:23:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f8cf932723cb79c6511c7a4565c26fc3c1a8b195b63a1b4f27567664469b8`  
		Last Modified: Tue, 01 Nov 2022 19:11:07 GMT  
		Size: 118.4 MB (118395001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06295a7c5807cf45167f1a47e93084873628c3417ae38bd41c276b71ba1c46ab`  
		Last Modified: Tue, 01 Nov 2022 19:10:45 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92d8ff62b16b450357e75981f8b6277cddab5a79836683195be024c5b466eb1`  
		Last Modified: Tue, 01 Nov 2022 19:31:14 GMT  
		Size: 6.1 MB (6065387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136c853b146e693b550c1d68b6b6713b79d7befffc79acb1530b83593b8fa935`  
		Last Modified: Tue, 01 Nov 2022 19:31:13 GMT  
		Size: 1.2 MB (1159979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f924d6193ccce35a47a6ee295f40e327abf4a8492374030689faf3f505632e08`  
		Last Modified: Tue, 01 Nov 2022 19:31:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6b8569ece82b11e5f6720884af16dce90859af84c6a9ab271ce05a08435fbd77
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127999797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1543ea235e3a8ec3d0ad049bdc81b95745b72848028c6dbc10cde12da0b876fc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 26 Oct 2022 08:09:57 GMT
RUN apk add --no-cache ca-certificates
# Wed, 26 Oct 2022 08:09:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 Oct 2022 08:09:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:40:17 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:41:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:41:34 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:41:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:41:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:41:35 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:05:53 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:05:53 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:05:53 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:05:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:05:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:05:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:05:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d82f9e3411d2eff49049d09ae871e53b96a0cc7dd335883f1fec28c43f9c86`  
		Last Modified: Wed, 26 Oct 2022 08:17:16 GMT  
		Size: 284.7 KB (284723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e169736571560c1a3278f9971532d55ddc4abfaef12e8c54c05f4644445d5520`  
		Last Modified: Wed, 26 Oct 2022 08:17:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc530f9a61e7c0e16b1cb3d48b70136b625cf624976acc638b9d6aef5525995`  
		Last Modified: Tue, 01 Nov 2022 18:48:07 GMT  
		Size: 116.8 MB (116836732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562d55c2123be45d40bfd4dd4dea65161ad3d83b50153de3cc0b63ec7a061f4b`  
		Last Modified: Tue, 01 Nov 2022 18:47:54 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90594629b6df4d09d221ea3fc570b4944e36520a3503ffa3a838772b0e46561`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 7.0 MB (7049481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e41bd715f5f0d05c59b600661a8f0cfb5145de632b14a77d012cfd1ffeea780`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 1.1 MB (1120483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3da6b029e0d694358fe69ed7435eb464495babb3bc51d3d5f30a5222406935`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:0bfdd9fd29aabe5e64b1c692ef01a8064dc2c4932747c3bf06363fd238817630
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128911035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3d666ccc1132e45cb0e54d7fd1891ab309ad3ae1fa96a20556f67f531c4bcc0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:26:01 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:26:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:26:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:17:13 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:19:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:20:03 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:20:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:20:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:20:05 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:50:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:50:46 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:50:46 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:50:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:50:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:50:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:50:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36899d7325c2c25a7d8e61ef33bb1e93b83f811f462e9ddad81c86df87b0685`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 286.7 KB (286747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9309524edda98df2abd6704c6f56004422a28b63364f028763ea000fc32d6eca`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b608654249afe5c44e2b3f100f6b333302506cd24adc46afa3302bb03ff96e`  
		Last Modified: Tue, 01 Nov 2022 19:31:59 GMT  
		Size: 117.2 MB (117238077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93311758f4ff1a16fa50dab5c51c12dd47a1920496e07493f5452c97e24eff9c`  
		Last Modified: Tue, 01 Nov 2022 19:31:32 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce6b57ae4a73b81094351a45358cebcbfbccd4d0d31ab77e71afc97d675dc63`  
		Last Modified: Tue, 01 Nov 2022 19:51:34 GMT  
		Size: 7.5 MB (7478322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5fa9d97b98179c5269f7f488f5488ec1a31fa543c75dc88705c8ed0a755e1c`  
		Last Modified: Tue, 01 Nov 2022 19:51:33 GMT  
		Size: 1.1 MB (1103853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f6efc0777ee24d394842b20cc0fe8c229ae5fecbb8dbb5537e66f5fc1fcf41`  
		Last Modified: Tue, 01 Nov 2022 19:51:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:660f4e58ece536977f580dad53c004e3fe9b1496a0af262adf93a8480746e615
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131825256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d3b89f5e95a2acfe27efc6ab49664e2a25268891a03b26100d1cca071938a79`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:16:09 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:16:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:16:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:43:10 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:46:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:47:10 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:47:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:47:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:47:13 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:20:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:20:25 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:20:26 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:20:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:20:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:20:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:20:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d31ae2e1f77c70a25e9cbeea435b4ab68149a4e17f9d4668768da8dd5ac68a`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 285.0 KB (284954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2788e533105e3c00ed84523a8f99d7947c0bb8b12932018a3081ecc29964605`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a12f83dfb1b48c3152a859b9b55b4483128b0be37e4877271cbd453b23fb43`  
		Last Modified: Tue, 01 Nov 2022 19:02:36 GMT  
		Size: 120.7 MB (120729474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e663873bb0a71689aee0be3ce5f4195e0b573039585fcc3182fe189e8e8fe05`  
		Last Modified: Tue, 01 Nov 2022 19:02:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802d29971118d482599687d5c1f1c069a8f0b8cb0c96e3ec3d5f550416223491`  
		Last Modified: Tue, 01 Nov 2022 19:21:20 GMT  
		Size: 7.1 MB (7052072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eea39f6b8018dc8d0011d05cdf7f2412b1435fdedc607d0087cfb9c631ccc23`  
		Last Modified: Tue, 01 Nov 2022 19:21:19 GMT  
		Size: 1.2 MB (1167444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a34c766fedcef740b10fddb96cd1ffd7aeae2d9628ddfa2510fedd4bbe64d2b`  
		Last Modified: Tue, 01 Nov 2022 19:21:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:ee5b9081fd81e7adbf4a0c1bf8fd4f9f882e755ac9fc03b24f12c7699aa5b52b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull caddy@sha256:f279c274451500e517aada07ecabddffd03b23f0b9d81791d2347e369b267a6f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2958579667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c57c677f08a022815e25e725365624f628555a00eab2b42f1830e71794c949`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 12:45:06 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Oct 2022 12:45:07 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Oct 2022 12:45:08 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Oct 2022 12:45:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Oct 2022 12:46:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Oct 2022 12:46:38 GMT
ENV GOPATH=C:\go
# Wed, 12 Oct 2022 12:47:37 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 01 Nov 2022 19:19:52 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:25:48 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 01 Nov 2022 19:25:50 GMT
WORKDIR C:\go
# Tue, 01 Nov 2022 20:18:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 01 Nov 2022 20:18:12 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 20:18:13 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 20:18:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 20:19:33 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 01 Nov 2022 20:19:34 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094a4c27e78f8821517fd551cd9e3d5f4b1e4199bdcd783b3fbda849e4995ad1`  
		Last Modified: Wed, 12 Oct 2022 13:16:26 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e91de5ff2103556b1048388473379f95d41247701f0911ebc7c530a861f3f5e`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52642f9e5e3a52bef8ee5677bcb62a364e07003da51f16eb28b8a4ce34fe9f7d`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26528ba698d400f5680be93457d24581b9e4e7a2399de7bb23cbd549f206613`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c89703eb31300a2a39c85ce287a6b9fe88da033828368275bdbb53c2f7704c`  
		Last Modified: Wed, 12 Oct 2022 13:16:30 GMT  
		Size: 25.4 MB (25439927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8705eaae12fa4840be2d79e376eb1b4b7b18da881acad2892b1c47336e796f46`  
		Last Modified: Wed, 12 Oct 2022 13:16:19 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebda8897c2727e3b971c947385632df6f19de06da75e9f161200d43d1acf714`  
		Last Modified: Wed, 12 Oct 2022 13:16:19 GMT  
		Size: 315.0 KB (315035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8667d37dce62bb077cd534d490f047b61dfe9c30023659258862cada9cbd0ba`  
		Last Modified: Tue, 01 Nov 2022 19:54:40 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac8e32e89f1739964a644b8b8b5b44bbae9752f8ea1f87e93455ca36cc86a7d`  
		Last Modified: Tue, 01 Nov 2022 19:55:33 GMT  
		Size: 157.7 MB (157676844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cabbd4ff51bc72ab20efd9f4eb4ebb788679ef03c2fc9b8a72f711fe3558590`  
		Last Modified: Tue, 01 Nov 2022 19:54:40 GMT  
		Size: 1.5 KB (1459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a7aa6766a51e2f5a5add77b40fd7eafa9d3d5049c3b4506b6b4e6dffb65cd6`  
		Last Modified: Tue, 01 Nov 2022 20:21:08 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54feb136a1e02e5d213be9750ca621c39022ff48f54c1e67daace9a82dd241f1`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7c0ce28f0f06a413d72723dbca806a7b025194983d436501cb04b7b2d7379`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e48594ab78eca9cfe42619a2f721de764c027be8fa22700565227c765b4ed7e`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55feb68cd00871cb13079eb862d65521274326d062594c7522edcc8f9bac23f1`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.6 MB (1631634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d398f623f33e057b5d399473e3ee1243fef32140e9a4411c1f69a913b43acb08`  
		Last Modified: Tue, 01 Nov 2022 20:21:05 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:39520901129debe71fc3b671250e73c438c85ee3435b24c8c8c5bc6293f05800
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1129; amd64

### `caddy:2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1129; amd64

```console
$ docker pull caddy@sha256:6e35c0ddda3afe05cb015c908260022b09ae192d81ad72f3bf1e32c70d7cb243
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2659936170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:265570f6cf9dffda304fb3a6712c85940e0f8d23ef6d8ffbfd8e1ebdd6d89d85`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 12:40:52 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Oct 2022 12:40:53 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Oct 2022 12:40:54 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Oct 2022 12:40:55 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Oct 2022 12:41:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Oct 2022 12:41:26 GMT
ENV GOPATH=C:\go
# Wed, 12 Oct 2022 12:41:47 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 01 Nov 2022 19:15:18 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:19:35 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 01 Nov 2022 19:19:38 GMT
WORKDIR C:\go
# Tue, 01 Nov 2022 20:19:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 01 Nov 2022 20:19:43 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 20:19:45 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 20:19:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 20:20:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 01 Nov 2022 20:20:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e9b54b31e104f64c9eb8a65ac0af5effd645bd00a77ea297b6015d28022a74`  
		Last Modified: Mon, 17 Oct 2022 21:39:11 GMT  
		Size: 1000.0 MB (1000028645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f8b589252b90e37349f39b9d4495646791b4050d7cd218336fcc4624b0ebe2`  
		Last Modified: Wed, 12 Oct 2022 13:15:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811ef63d5261b55ee6b499dbc7fcd1ed13386326466fb81a0801abbcbcb75d3f`  
		Last Modified: Wed, 12 Oct 2022 13:15:28 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816740cd643a7a4e72aa527cd033d0c95686c9725ff70dac3260b44dce508e73`  
		Last Modified: Wed, 12 Oct 2022 13:15:28 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599e30c8b316e75d786cfd91f97b9fae4c89fb00f3fce0619eb4e66bc3165521`  
		Last Modified: Wed, 12 Oct 2022 13:15:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77a0d37b81c920d4b783c0b2cfad656a4b8733960ba3afd4e0a1f39f202f948`  
		Last Modified: Wed, 12 Oct 2022 13:15:32 GMT  
		Size: 25.7 MB (25689345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b699f53b56e90279b0bb8ce4434f9b68bbc28fa30756476e22c7ef3dc869e24a`  
		Last Modified: Wed, 12 Oct 2022 13:15:21 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57fcf632f60c89dd981a8a7fa084e738f55129b1786fd9a9e9f5ab8aa1e02d82`  
		Last Modified: Wed, 12 Oct 2022 13:15:24 GMT  
		Size: 526.5 KB (526519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8b0d888223c93af8f0c84ad35156f79df9b0d9ae107f61ded320d2a4fed5f3`  
		Last Modified: Tue, 01 Nov 2022 19:53:29 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49602de12fff655f45d03b1befdd7e56321771c65ed690492e4092da51046bb3`  
		Last Modified: Tue, 01 Nov 2022 19:54:22 GMT  
		Size: 157.8 MB (157838831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cb5ede4eaf1f86f7c0957639a8b53a0c6740df6fa395d3d286e32bff6b9195`  
		Last Modified: Tue, 01 Nov 2022 19:53:29 GMT  
		Size: 1.6 KB (1584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d0ae347408d32205a9ca4c0628e814833984ac8c0fbfb6c6687b9c94a733aa`  
		Last Modified: Tue, 01 Nov 2022 20:21:30 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453489637085324b6412fd9d83cc639d7a9f9135fb5db5dec214462b3293c98f`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cc23fcabe43926f14c7d7e786e9175c87fe573e41fc0158bdc02cfc08fb567`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528f2dc5e38ba5bad570845252c13446ea9637f9c7a80590c93c28886ab79803`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd45b40a0e40f3a52f9a7e2e1cf3cf3b0501ca3f8d637ef46596ee30a9193264`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.8 MB (1837122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bd243dcf25ec803b906e53fa263b2803735773f0227c1c4bac5d52654bb8c6`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:a2ab9b4da81fb5793c09308f6353dec3d5aa70255288aa5a9390cf5333e74935
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3532; amd64
	-	windows version 10.0.20348.1129; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.3532; amd64

```console
$ docker pull caddy@sha256:c795b26fccceaa3ea3738c3d086e0c9da9978392aeb6e2c69ae3d71131b88998
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726785951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a0ffc50daa8e99f5d3029bd930601ec939b66a180da1ad5fef783d1fcb69eb3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 16:58:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:14:49 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:16:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:16:10 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:16:11 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:16:12 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:16:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:16:14 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:16:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:16:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:16:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:16:19 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:16:20 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:16:21 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:16:22 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:17:16 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:17:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:028c482fad0f111537a40f65401f65de54c9fd682951a4f8cf9b644d7c128e18`  
		Size: 834.0 MB (833997855 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77462c8fbd8b2782ee2fc5f09bebfb350912f754186b058478ab8d22f50bb047`  
		Last Modified: Wed, 12 Oct 2022 17:04:34 GMT  
		Size: 358.2 KB (358248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a372be4d9f43d4d5884bc4093c44aedf12150f55ea9457baa2fcceb43ef8074`  
		Last Modified: Thu, 13 Oct 2022 23:21:08 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a8993c29bb6d4c31b0be3609bc7fb2af2666435fe70bb2f329784277d629d1`  
		Last Modified: Thu, 13 Oct 2022 23:21:11 GMT  
		Size: 14.9 MB (14947938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98662b730099437011356fa77ef9072054f4ad73d3781e9b02d4750689762162`  
		Last Modified: Thu, 13 Oct 2022 23:21:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7e77f6a080ad6fa8a7320831868ccd7b6385e995988f2e6cca76090a565c99`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec71d29d036cab0bdbc7765216513aad527933ededfec4492a97724c6bab52d`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a11bac4631094c366303dd3c571fe04cf1b543bafba72d8dd1030f8ae2ec185`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4dc588cdabd0672f8b29c59cd9ddc6d927160284a6f6529fbe39b8e34ca766`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f39777f21d48153f681f16b5a1cd2e12440066bc96a665fa3b85a6275b74942`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638736df2ba6ceaed21b97ee12046d2d0494561bd735581618ab505ff602b0da`  
		Last Modified: Thu, 13 Oct 2022 23:21:04 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e0fe53dba785fdf61d7431392d7e15beeebbe5f215d9a2de2ee00975e7b5c4`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb7b8fc42485b0656b2afcb99344cda044ce10d0107cc91955fbe11433c358`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb8f166931be4f8f0b0a07611df01a8e7d1101f8a8ce564144ded43917e1021`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bc6f4b7a114b7722cfc81aa83b74727261766c2cef9bc0787e447435c33d2a`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5563ab3963680a40da3bc2269bbc1e76362b359547dae9705892cf8f54b50dd1`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d300f0320cd2b8ce3f3e58cbb3acb06e24c5f59a342725056a10667329f914`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfb9dfa0b00914a255876439613219f4a74e83734df6b8a197e6e0bb53bf905`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b9233dbf203ca77eea2271813856d219ba7d2f633adf99f3262612edfad738`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 291.8 KB (291836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefde31b509f056641749adae4daa4e0ad3265d260ac1c61b41c8950a10824e6`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.20348.1129; amd64

```console
$ docker pull caddy@sha256:e1e15c80e157d71221ec43035cae93b3ea8ba7a6b203428e93159aa6ff5e1463
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2432333411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbd806ca24dfacee0d098f111cc9f6d5f42fdbd9db91a63a8de0d048d3984d5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 17:01:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:17:37 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:18:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:18:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:18:13 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:18:13 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:18:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:18:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:18:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:18:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:18:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:18:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:18:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:18:21 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:18:22 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:18:23 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:18:24 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:18:40 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:18:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ab91661ce2a2a2c14684a2ba0f543a81d7896773f88200b31be0e37c589de38`  
		Size: 979.4 MB (979359717 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cd84a277fd91a008fe0c8fc7d6706544075a294512940b16f57998588ea892`  
		Last Modified: Wed, 12 Oct 2022 17:04:58 GMT  
		Size: 616.9 KB (616893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b069dfbedeca0437916f85fdd78a598955839b91ffc4cba4d6327e5c79487`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5263d846656ffa3662062b1a58d9c6d114e00fa5344edc9b93ea5895c4fa46`  
		Last Modified: Thu, 13 Oct 2022 23:21:34 GMT  
		Size: 15.1 MB (15149356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e378404d94c7fb280c51201d60aef05af3196a0ead3b716521cedbe766ba5e3e`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11749bcf2c3e4097f9a1a30d1fc22184e48c94ab54945730c51c36be175c668d`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cb14f39fa0dce5d6dab4bdd1a896c02b5a6bba01dcd46ed36928c2cce27295`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf622a21cfc36d8958be2f273f52b7d4824d500be08f6a2de791506dcc6c981f`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b246af35953d05f1c4292cb1cf8cfc29215ceac2e013ae2a0759aa2d216516`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08367cd2562c20737156e692dca481f835f4832fabb63602fb5edc78494057ae`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6d70510bf329eff739580f04b59acba9cb4aa74e57bcb6fca996d6df6b6d2c`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc6e963fa5949ceb99519a652299dea21a92c9389aadabedb2deeb4e51855b5`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d175d8244325a62c683c4d1fa6cc266f73231f93142fd0f52c3378da6db1464`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4ce9495075c9b00994ef154c9eb0974ba1853a8244869e35af4eecfca4dce7`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceee07aab1c573de692984f7655da9e6c4aee31260b8df8735344242e6f1ff8`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295041dd24e85177aaf7e1bbd1c0b032d2eafaf3da59213972894238dd5b3d72`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3583f031f13dfd9a933b6e8d4808a3ac7f3e007d2e751af9581b76b08b6e0c4a`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1603973d06c7b0a01ab165d727b40f842361ce898a8e7b8579d6bd9db938c8a6`  
		Last Modified: Thu, 13 Oct 2022 23:21:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c4bf5f410b0a58ef5b477fdf99b90ad01e7deb85b685cf06eaae5c9d83a531`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 319.8 KB (319842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da4c854489e4317220200f8dca47e2335696fe8fa9e7a2aa678467b12b4db7b`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:750ce937e1a109f41cc11cad93540eeb4b7ab051847137267847c104941dfe75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull caddy@sha256:c795b26fccceaa3ea3738c3d086e0c9da9978392aeb6e2c69ae3d71131b88998
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726785951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a0ffc50daa8e99f5d3029bd930601ec939b66a180da1ad5fef783d1fcb69eb3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 16:58:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:14:49 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:16:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:16:10 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:16:11 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:16:12 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:16:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:16:14 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:16:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:16:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:16:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:16:19 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:16:20 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:16:21 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:16:22 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:17:16 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:17:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:028c482fad0f111537a40f65401f65de54c9fd682951a4f8cf9b644d7c128e18`  
		Size: 834.0 MB (833997855 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77462c8fbd8b2782ee2fc5f09bebfb350912f754186b058478ab8d22f50bb047`  
		Last Modified: Wed, 12 Oct 2022 17:04:34 GMT  
		Size: 358.2 KB (358248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a372be4d9f43d4d5884bc4093c44aedf12150f55ea9457baa2fcceb43ef8074`  
		Last Modified: Thu, 13 Oct 2022 23:21:08 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a8993c29bb6d4c31b0be3609bc7fb2af2666435fe70bb2f329784277d629d1`  
		Last Modified: Thu, 13 Oct 2022 23:21:11 GMT  
		Size: 14.9 MB (14947938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98662b730099437011356fa77ef9072054f4ad73d3781e9b02d4750689762162`  
		Last Modified: Thu, 13 Oct 2022 23:21:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7e77f6a080ad6fa8a7320831868ccd7b6385e995988f2e6cca76090a565c99`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec71d29d036cab0bdbc7765216513aad527933ededfec4492a97724c6bab52d`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a11bac4631094c366303dd3c571fe04cf1b543bafba72d8dd1030f8ae2ec185`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4dc588cdabd0672f8b29c59cd9ddc6d927160284a6f6529fbe39b8e34ca766`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f39777f21d48153f681f16b5a1cd2e12440066bc96a665fa3b85a6275b74942`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638736df2ba6ceaed21b97ee12046d2d0494561bd735581618ab505ff602b0da`  
		Last Modified: Thu, 13 Oct 2022 23:21:04 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e0fe53dba785fdf61d7431392d7e15beeebbe5f215d9a2de2ee00975e7b5c4`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb7b8fc42485b0656b2afcb99344cda044ce10d0107cc91955fbe11433c358`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb8f166931be4f8f0b0a07611df01a8e7d1101f8a8ce564144ded43917e1021`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bc6f4b7a114b7722cfc81aa83b74727261766c2cef9bc0787e447435c33d2a`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5563ab3963680a40da3bc2269bbc1e76362b359547dae9705892cf8f54b50dd1`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d300f0320cd2b8ce3f3e58cbb3acb06e24c5f59a342725056a10667329f914`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfb9dfa0b00914a255876439613219f4a74e83734df6b8a197e6e0bb53bf905`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b9233dbf203ca77eea2271813856d219ba7d2f633adf99f3262612edfad738`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 291.8 KB (291836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefde31b509f056641749adae4daa4e0ad3265d260ac1c61b41c8950a10824e6`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:6a6b89102bf9584016d1a0364792d3cea05585c2fc057b4ffce271b8496a8bc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1129; amd64

### `caddy:2-windowsservercore-ltsc2022` - windows version 10.0.20348.1129; amd64

```console
$ docker pull caddy@sha256:e1e15c80e157d71221ec43035cae93b3ea8ba7a6b203428e93159aa6ff5e1463
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2432333411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbd806ca24dfacee0d098f111cc9f6d5f42fdbd9db91a63a8de0d048d3984d5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 17:01:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:17:37 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:18:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:18:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:18:13 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:18:13 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:18:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:18:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:18:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:18:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:18:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:18:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:18:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:18:21 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:18:22 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:18:23 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:18:24 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:18:40 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:18:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ab91661ce2a2a2c14684a2ba0f543a81d7896773f88200b31be0e37c589de38`  
		Size: 979.4 MB (979359717 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cd84a277fd91a008fe0c8fc7d6706544075a294512940b16f57998588ea892`  
		Last Modified: Wed, 12 Oct 2022 17:04:58 GMT  
		Size: 616.9 KB (616893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b069dfbedeca0437916f85fdd78a598955839b91ffc4cba4d6327e5c79487`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5263d846656ffa3662062b1a58d9c6d114e00fa5344edc9b93ea5895c4fa46`  
		Last Modified: Thu, 13 Oct 2022 23:21:34 GMT  
		Size: 15.1 MB (15149356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e378404d94c7fb280c51201d60aef05af3196a0ead3b716521cedbe766ba5e3e`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11749bcf2c3e4097f9a1a30d1fc22184e48c94ab54945730c51c36be175c668d`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cb14f39fa0dce5d6dab4bdd1a896c02b5a6bba01dcd46ed36928c2cce27295`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf622a21cfc36d8958be2f273f52b7d4824d500be08f6a2de791506dcc6c981f`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b246af35953d05f1c4292cb1cf8cfc29215ceac2e013ae2a0759aa2d216516`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08367cd2562c20737156e692dca481f835f4832fabb63602fb5edc78494057ae`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6d70510bf329eff739580f04b59acba9cb4aa74e57bcb6fca996d6df6b6d2c`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc6e963fa5949ceb99519a652299dea21a92c9389aadabedb2deeb4e51855b5`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d175d8244325a62c683c4d1fa6cc266f73231f93142fd0f52c3378da6db1464`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4ce9495075c9b00994ef154c9eb0974ba1853a8244869e35af4eecfca4dce7`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceee07aab1c573de692984f7655da9e6c4aee31260b8df8735344242e6f1ff8`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295041dd24e85177aaf7e1bbd1c0b032d2eafaf3da59213972894238dd5b3d72`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3583f031f13dfd9a933b6e8d4808a3ac7f3e007d2e751af9581b76b08b6e0c4a`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1603973d06c7b0a01ab165d727b40f842361ce898a8e7b8579d6bd9db938c8a6`  
		Last Modified: Thu, 13 Oct 2022 23:21:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c4bf5f410b0a58ef5b477fdf99b90ad01e7deb85b685cf06eaae5c9d83a531`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 319.8 KB (319842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da4c854489e4317220200f8dca47e2335696fe8fa9e7a2aa678467b12b4db7b`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6`

```console
$ docker pull caddy@sha256:d3e5e175b10a2a5b66be9570ed9867aeb77af8eca7a14b6033dcde2c9f6fee6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3532; amd64
	-	windows version 10.0.20348.1129; amd64

### `caddy:2.6` - linux; amd64

```console
$ docker pull caddy@sha256:7992b931b7da3cf0840dd69ea74b2c67d423faf03408da8abdc31b7590a239a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17676993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:006d393a4e6a01f82413e41b3e0f06dfb1872d5ca6a37aba315e4ec9e2cc6c4c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:34:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 04:34:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 01:43:19 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 01:43:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 01:43:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 01:43:22 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 01:43:22 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 01:43:22 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 01:43:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 80
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 443
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 01:43:24 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 01:43:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5625668cf98fd3e4d769f18d45f27e34fe3d085cfb9927ff7ad2cdc84d8c493f`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 304.5 KB (304517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675d09b34c5347b62625d31b2a458824240b90e51d18bcc38ad37d317e83d64c`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1747be7065842ba85f86aed65e75608dfd2f546ab9d8ecd4a8842c8f4634795`  
		Last Modified: Fri, 14 Oct 2022 01:43:47 GMT  
		Size: 14.6 MB (14560435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8ee6c4c21d12cd28fcd0e196acb8569f35518dc36c691c91b4c8ca1928bf9d`  
		Last Modified: Fri, 14 Oct 2022 01:43:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - linux; arm variant v6

```console
$ docker pull caddy@sha256:76b70e0dc74358fc1f7ef178c46cc9c047a90cd05e842d26305da1ee04ff3ad8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16834877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cac02415934eaae38be5b122f6a0c760f747e6f50f1551c9a45f4f186454f04`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 19:49:23 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 27 Oct 2022 19:49:25 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 27 Oct 2022 19:49:25 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 27 Oct 2022 19:49:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 27 Oct 2022 19:49:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 19:49:28 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 27 Oct 2022 19:49:28 GMT
ENV XDG_DATA_HOME=/data
# Thu, 27 Oct 2022 19:49:28 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 27 Oct 2022 19:49:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 80
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 443
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 443/udp
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 2019
# Thu, 27 Oct 2022 19:49:30 GMT
WORKDIR /srv
# Thu, 27 Oct 2022 19:49:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7f6197b1f089356a6bff8bf29fdcef692051048bd17db70d72df822c89c04d`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 304.4 KB (304404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc91cb09da181c7973089ccf7aca9c7830c738ac1e614883f86c2eecdcb68002`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 5.8 KB (5751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ffb96b75d9dc6019cfe6202b9fed588b3ff9a91cc89237d6a24c98eb5fd590`  
		Last Modified: Thu, 27 Oct 2022 19:50:36 GMT  
		Size: 13.9 MB (13910603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb4866598fa794379095b277b41d4b0cb626d61cc20c6f6cff7d920bc99330`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9df5bfbadaf5495675c4de47918d3631d439d159681e352069eaa206f664a8ac
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16617541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d61e1121278866d5afee597ba2ac37a9b5bec51b6323b551fe9a89b5d99d63e5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 10:30:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 27 Oct 2022 10:30:41 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 27 Oct 2022 10:30:41 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 27 Oct 2022 10:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 27 Oct 2022 10:30:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 10:30:45 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 27 Oct 2022 10:30:45 GMT
ENV XDG_DATA_HOME=/data
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 27 Oct 2022 10:30:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 80
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 443
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 443/udp
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 2019
# Thu, 27 Oct 2022 10:30:46 GMT
WORKDIR /srv
# Thu, 27 Oct 2022 10:30:46 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9f1011ebc9810d3e61468e7ce6c2866fc65920db06e3bccde2da749f976500`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 303.5 KB (303537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28310071f60503f30048b0cad1abe85c763c57dd4e69715cc57d60560481318`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 5.8 KB (5753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7792abbee8ad8ec28f7e6e2864a9e8ad229de5f701ba4bf04be77cffac8835ac`  
		Last Modified: Thu, 27 Oct 2022 10:31:39 GMT  
		Size: 13.9 MB (13891032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c5be986b3fadf5f34a0a4311ffa6a22b4f1f0ff79c510fb7c58cb93c64e2f3`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f06fb46d2c67f3b7f9447b6c19f5b9909931b603d2b475f647624f577c6d94ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16278669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8876f25c7ec7330d6bf197e452e3a37deeea42e52b8c2b2c9103bc86b26795`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 26 Oct 2022 18:53:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 Oct 2022 18:53:58 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Wed, 26 Oct 2022 18:53:58 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 26 Oct 2022 18:54:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 Oct 2022 18:54:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 Oct 2022 18:54:01 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 Oct 2022 18:54:01 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 80
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 443
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 443/udp
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 2019
# Wed, 26 Oct 2022 18:54:02 GMT
WORKDIR /srv
# Wed, 26 Oct 2022 18:54:02 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5532e6e746eecf0e890ee17251a52841dd55694ae55c919dc6ddf6159e27cd5b`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 304.5 KB (304512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b816658ad2f9debd81f6df21dd733e54fc6eda530080cc3957e6f63d9677b9a`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d7ee92d83c49ca71b5440fd76d22ac6b75304bc48a0183bf392689ae8d5897`  
		Last Modified: Wed, 26 Oct 2022 18:54:26 GMT  
		Size: 13.3 MB (13260508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00da94c60a7ed1fc9acd392aedea2ab7b2bd6a7d67cc83b2d5d85c5cbd40090b`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - linux; ppc64le

```console
$ docker pull caddy@sha256:9665c6fd33be967b3bdfcdbeeb605e3a92e70080ef5caa8907a6cbdef064be3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (16031232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96553401995800bf37590502c237b4ab8cee57bd3885e83f76dcb42c53a7d7db`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:56:10 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 07:56:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 03:47:38 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 03:47:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 03:47:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 03:47:44 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 03:47:44 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 03:47:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 03:47:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 80
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 443
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 03:47:49 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 03:47:49 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 03:47:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf49ba2a5c90a152d4aef09519c7019835fbf2884d6afb1c85b3353b7d91388e`  
		Last Modified: Fri, 07 Oct 2022 07:57:09 GMT  
		Size: 306.5 KB (306522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dac87aba8912de3ce6fb3ca14bb6833f931fd15d7ec2d7435a18f11e5ddb6fb`  
		Last Modified: Fri, 07 Oct 2022 07:57:08 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea24f9a44c53fbd359328daff2e10e4e3f1c7d7bae21190ea2f6af3be43dd0b`  
		Last Modified: Fri, 14 Oct 2022 03:48:33 GMT  
		Size: 12.9 MB (12915404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4704e2ddccf987da9605ef1c8d4ef68a86cf3e6ba2f8c5d1e80e5915481e25c`  
		Last Modified: Fri, 14 Oct 2022 03:48:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - linux; s390x

```console
$ docker pull caddy@sha256:5702e27172b1bfb5e9930d544d7cf16a83f774419b1aa2078be464351ff5f70b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16967685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05ec4a186bcadcf0e691a443c7edebf42d46cff3997d01a56de43db0ecbab8e2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 10:23:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 10:23:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 00:55:05 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 00:55:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 00:55:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 00:55:15 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 00:55:16 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 00:55:17 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 00:55:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 00:55:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 00:55:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 00:55:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 00:55:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 00:55:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 00:55:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 00:55:22 GMT
EXPOSE 80
# Fri, 14 Oct 2022 00:55:22 GMT
EXPOSE 443
# Fri, 14 Oct 2022 00:55:23 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 00:55:23 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 00:55:24 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 00:55:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5123e0e5a47a6dfbd8cae1e2589df59b198f82ba790c211aeb3eefbbe41a17be`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 304.8 KB (304752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557f08048878eca2f16fd3b05bb138300739b9e74e467509792efc4278e74b3f`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91158060b74650f434cb3419f6ed862b0616480567b651bfae73b297f69b9992`  
		Last Modified: Fri, 14 Oct 2022 00:56:22 GMT  
		Size: 14.1 MB (14066352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511ac9f174e3fed802157937e9192a940800d73835958de90f5a363b5edf46ad`  
		Last Modified: Fri, 14 Oct 2022 00:56:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - windows version 10.0.17763.3532; amd64

```console
$ docker pull caddy@sha256:c795b26fccceaa3ea3738c3d086e0c9da9978392aeb6e2c69ae3d71131b88998
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726785951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a0ffc50daa8e99f5d3029bd930601ec939b66a180da1ad5fef783d1fcb69eb3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 16:58:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:14:49 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:16:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:16:10 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:16:11 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:16:12 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:16:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:16:14 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:16:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:16:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:16:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:16:19 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:16:20 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:16:21 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:16:22 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:17:16 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:17:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:028c482fad0f111537a40f65401f65de54c9fd682951a4f8cf9b644d7c128e18`  
		Size: 834.0 MB (833997855 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77462c8fbd8b2782ee2fc5f09bebfb350912f754186b058478ab8d22f50bb047`  
		Last Modified: Wed, 12 Oct 2022 17:04:34 GMT  
		Size: 358.2 KB (358248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a372be4d9f43d4d5884bc4093c44aedf12150f55ea9457baa2fcceb43ef8074`  
		Last Modified: Thu, 13 Oct 2022 23:21:08 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a8993c29bb6d4c31b0be3609bc7fb2af2666435fe70bb2f329784277d629d1`  
		Last Modified: Thu, 13 Oct 2022 23:21:11 GMT  
		Size: 14.9 MB (14947938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98662b730099437011356fa77ef9072054f4ad73d3781e9b02d4750689762162`  
		Last Modified: Thu, 13 Oct 2022 23:21:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7e77f6a080ad6fa8a7320831868ccd7b6385e995988f2e6cca76090a565c99`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec71d29d036cab0bdbc7765216513aad527933ededfec4492a97724c6bab52d`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a11bac4631094c366303dd3c571fe04cf1b543bafba72d8dd1030f8ae2ec185`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4dc588cdabd0672f8b29c59cd9ddc6d927160284a6f6529fbe39b8e34ca766`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f39777f21d48153f681f16b5a1cd2e12440066bc96a665fa3b85a6275b74942`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638736df2ba6ceaed21b97ee12046d2d0494561bd735581618ab505ff602b0da`  
		Last Modified: Thu, 13 Oct 2022 23:21:04 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e0fe53dba785fdf61d7431392d7e15beeebbe5f215d9a2de2ee00975e7b5c4`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb7b8fc42485b0656b2afcb99344cda044ce10d0107cc91955fbe11433c358`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb8f166931be4f8f0b0a07611df01a8e7d1101f8a8ce564144ded43917e1021`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bc6f4b7a114b7722cfc81aa83b74727261766c2cef9bc0787e447435c33d2a`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5563ab3963680a40da3bc2269bbc1e76362b359547dae9705892cf8f54b50dd1`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d300f0320cd2b8ce3f3e58cbb3acb06e24c5f59a342725056a10667329f914`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfb9dfa0b00914a255876439613219f4a74e83734df6b8a197e6e0bb53bf905`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b9233dbf203ca77eea2271813856d219ba7d2f633adf99f3262612edfad738`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 291.8 KB (291836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefde31b509f056641749adae4daa4e0ad3265d260ac1c61b41c8950a10824e6`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - windows version 10.0.20348.1129; amd64

```console
$ docker pull caddy@sha256:e1e15c80e157d71221ec43035cae93b3ea8ba7a6b203428e93159aa6ff5e1463
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2432333411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbd806ca24dfacee0d098f111cc9f6d5f42fdbd9db91a63a8de0d048d3984d5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 17:01:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:17:37 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:18:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:18:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:18:13 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:18:13 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:18:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:18:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:18:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:18:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:18:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:18:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:18:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:18:21 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:18:22 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:18:23 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:18:24 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:18:40 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:18:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ab91661ce2a2a2c14684a2ba0f543a81d7896773f88200b31be0e37c589de38`  
		Size: 979.4 MB (979359717 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cd84a277fd91a008fe0c8fc7d6706544075a294512940b16f57998588ea892`  
		Last Modified: Wed, 12 Oct 2022 17:04:58 GMT  
		Size: 616.9 KB (616893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b069dfbedeca0437916f85fdd78a598955839b91ffc4cba4d6327e5c79487`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5263d846656ffa3662062b1a58d9c6d114e00fa5344edc9b93ea5895c4fa46`  
		Last Modified: Thu, 13 Oct 2022 23:21:34 GMT  
		Size: 15.1 MB (15149356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e378404d94c7fb280c51201d60aef05af3196a0ead3b716521cedbe766ba5e3e`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11749bcf2c3e4097f9a1a30d1fc22184e48c94ab54945730c51c36be175c668d`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cb14f39fa0dce5d6dab4bdd1a896c02b5a6bba01dcd46ed36928c2cce27295`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf622a21cfc36d8958be2f273f52b7d4824d500be08f6a2de791506dcc6c981f`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b246af35953d05f1c4292cb1cf8cfc29215ceac2e013ae2a0759aa2d216516`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08367cd2562c20737156e692dca481f835f4832fabb63602fb5edc78494057ae`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6d70510bf329eff739580f04b59acba9cb4aa74e57bcb6fca996d6df6b6d2c`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc6e963fa5949ceb99519a652299dea21a92c9389aadabedb2deeb4e51855b5`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d175d8244325a62c683c4d1fa6cc266f73231f93142fd0f52c3378da6db1464`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4ce9495075c9b00994ef154c9eb0974ba1853a8244869e35af4eecfca4dce7`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceee07aab1c573de692984f7655da9e6c4aee31260b8df8735344242e6f1ff8`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295041dd24e85177aaf7e1bbd1c0b032d2eafaf3da59213972894238dd5b3d72`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3583f031f13dfd9a933b6e8d4808a3ac7f3e007d2e751af9581b76b08b6e0c4a`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1603973d06c7b0a01ab165d727b40f842361ce898a8e7b8579d6bd9db938c8a6`  
		Last Modified: Thu, 13 Oct 2022 23:21:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c4bf5f410b0a58ef5b477fdf99b90ad01e7deb85b685cf06eaae5c9d83a531`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 319.8 KB (319842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da4c854489e4317220200f8dca47e2335696fe8fa9e7a2aa678467b12b4db7b`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-alpine`

```console
$ docker pull caddy@sha256:0e3c6d476eb251d2e271c61d12472698e2be1909626d342c405ed58c70772857
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.6-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:7992b931b7da3cf0840dd69ea74b2c67d423faf03408da8abdc31b7590a239a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17676993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:006d393a4e6a01f82413e41b3e0f06dfb1872d5ca6a37aba315e4ec9e2cc6c4c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:34:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 04:34:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 01:43:19 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 01:43:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 01:43:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 01:43:22 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 01:43:22 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 01:43:22 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 01:43:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 80
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 443
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 01:43:24 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 01:43:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5625668cf98fd3e4d769f18d45f27e34fe3d085cfb9927ff7ad2cdc84d8c493f`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 304.5 KB (304517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675d09b34c5347b62625d31b2a458824240b90e51d18bcc38ad37d317e83d64c`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1747be7065842ba85f86aed65e75608dfd2f546ab9d8ecd4a8842c8f4634795`  
		Last Modified: Fri, 14 Oct 2022 01:43:47 GMT  
		Size: 14.6 MB (14560435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8ee6c4c21d12cd28fcd0e196acb8569f35518dc36c691c91b4c8ca1928bf9d`  
		Last Modified: Fri, 14 Oct 2022 01:43:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:76b70e0dc74358fc1f7ef178c46cc9c047a90cd05e842d26305da1ee04ff3ad8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16834877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cac02415934eaae38be5b122f6a0c760f747e6f50f1551c9a45f4f186454f04`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 19:49:23 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 27 Oct 2022 19:49:25 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 27 Oct 2022 19:49:25 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 27 Oct 2022 19:49:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 27 Oct 2022 19:49:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 19:49:28 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 27 Oct 2022 19:49:28 GMT
ENV XDG_DATA_HOME=/data
# Thu, 27 Oct 2022 19:49:28 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 27 Oct 2022 19:49:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 80
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 443
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 443/udp
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 2019
# Thu, 27 Oct 2022 19:49:30 GMT
WORKDIR /srv
# Thu, 27 Oct 2022 19:49:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7f6197b1f089356a6bff8bf29fdcef692051048bd17db70d72df822c89c04d`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 304.4 KB (304404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc91cb09da181c7973089ccf7aca9c7830c738ac1e614883f86c2eecdcb68002`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 5.8 KB (5751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ffb96b75d9dc6019cfe6202b9fed588b3ff9a91cc89237d6a24c98eb5fd590`  
		Last Modified: Thu, 27 Oct 2022 19:50:36 GMT  
		Size: 13.9 MB (13910603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb4866598fa794379095b277b41d4b0cb626d61cc20c6f6cff7d920bc99330`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9df5bfbadaf5495675c4de47918d3631d439d159681e352069eaa206f664a8ac
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16617541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d61e1121278866d5afee597ba2ac37a9b5bec51b6323b551fe9a89b5d99d63e5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 10:30:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 27 Oct 2022 10:30:41 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 27 Oct 2022 10:30:41 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 27 Oct 2022 10:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 27 Oct 2022 10:30:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 10:30:45 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 27 Oct 2022 10:30:45 GMT
ENV XDG_DATA_HOME=/data
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 27 Oct 2022 10:30:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 80
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 443
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 443/udp
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 2019
# Thu, 27 Oct 2022 10:30:46 GMT
WORKDIR /srv
# Thu, 27 Oct 2022 10:30:46 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9f1011ebc9810d3e61468e7ce6c2866fc65920db06e3bccde2da749f976500`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 303.5 KB (303537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28310071f60503f30048b0cad1abe85c763c57dd4e69715cc57d60560481318`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 5.8 KB (5753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7792abbee8ad8ec28f7e6e2864a9e8ad229de5f701ba4bf04be77cffac8835ac`  
		Last Modified: Thu, 27 Oct 2022 10:31:39 GMT  
		Size: 13.9 MB (13891032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c5be986b3fadf5f34a0a4311ffa6a22b4f1f0ff79c510fb7c58cb93c64e2f3`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f06fb46d2c67f3b7f9447b6c19f5b9909931b603d2b475f647624f577c6d94ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16278669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8876f25c7ec7330d6bf197e452e3a37deeea42e52b8c2b2c9103bc86b26795`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 26 Oct 2022 18:53:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 Oct 2022 18:53:58 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Wed, 26 Oct 2022 18:53:58 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 26 Oct 2022 18:54:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 Oct 2022 18:54:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 Oct 2022 18:54:01 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 Oct 2022 18:54:01 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 80
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 443
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 443/udp
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 2019
# Wed, 26 Oct 2022 18:54:02 GMT
WORKDIR /srv
# Wed, 26 Oct 2022 18:54:02 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5532e6e746eecf0e890ee17251a52841dd55694ae55c919dc6ddf6159e27cd5b`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 304.5 KB (304512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b816658ad2f9debd81f6df21dd733e54fc6eda530080cc3957e6f63d9677b9a`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d7ee92d83c49ca71b5440fd76d22ac6b75304bc48a0183bf392689ae8d5897`  
		Last Modified: Wed, 26 Oct 2022 18:54:26 GMT  
		Size: 13.3 MB (13260508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00da94c60a7ed1fc9acd392aedea2ab7b2bd6a7d67cc83b2d5d85c5cbd40090b`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:9665c6fd33be967b3bdfcdbeeb605e3a92e70080ef5caa8907a6cbdef064be3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (16031232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96553401995800bf37590502c237b4ab8cee57bd3885e83f76dcb42c53a7d7db`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:56:10 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 07:56:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 03:47:38 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 03:47:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 03:47:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 03:47:44 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 03:47:44 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 03:47:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 03:47:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 80
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 443
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 03:47:49 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 03:47:49 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 03:47:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf49ba2a5c90a152d4aef09519c7019835fbf2884d6afb1c85b3353b7d91388e`  
		Last Modified: Fri, 07 Oct 2022 07:57:09 GMT  
		Size: 306.5 KB (306522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dac87aba8912de3ce6fb3ca14bb6833f931fd15d7ec2d7435a18f11e5ddb6fb`  
		Last Modified: Fri, 07 Oct 2022 07:57:08 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea24f9a44c53fbd359328daff2e10e4e3f1c7d7bae21190ea2f6af3be43dd0b`  
		Last Modified: Fri, 14 Oct 2022 03:48:33 GMT  
		Size: 12.9 MB (12915404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4704e2ddccf987da9605ef1c8d4ef68a86cf3e6ba2f8c5d1e80e5915481e25c`  
		Last Modified: Fri, 14 Oct 2022 03:48:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:5702e27172b1bfb5e9930d544d7cf16a83f774419b1aa2078be464351ff5f70b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16967685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05ec4a186bcadcf0e691a443c7edebf42d46cff3997d01a56de43db0ecbab8e2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 10:23:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 10:23:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 00:55:05 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 00:55:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 00:55:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 00:55:15 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 00:55:16 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 00:55:17 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 00:55:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 00:55:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 00:55:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 00:55:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 00:55:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 00:55:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 00:55:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 00:55:22 GMT
EXPOSE 80
# Fri, 14 Oct 2022 00:55:22 GMT
EXPOSE 443
# Fri, 14 Oct 2022 00:55:23 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 00:55:23 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 00:55:24 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 00:55:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5123e0e5a47a6dfbd8cae1e2589df59b198f82ba790c211aeb3eefbbe41a17be`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 304.8 KB (304752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557f08048878eca2f16fd3b05bb138300739b9e74e467509792efc4278e74b3f`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91158060b74650f434cb3419f6ed862b0616480567b651bfae73b297f69b9992`  
		Last Modified: Fri, 14 Oct 2022 00:56:22 GMT  
		Size: 14.1 MB (14066352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511ac9f174e3fed802157937e9192a940800d73835958de90f5a363b5edf46ad`  
		Last Modified: Fri, 14 Oct 2022 00:56:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder`

```console
$ docker pull caddy@sha256:9a395d60c9cba0036b919495f7637be3fafb0a97459ee970f1738e0252dfa2f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3532; amd64
	-	windows version 10.0.20348.1129; amd64

### `caddy:2.6-builder` - linux; amd64

```console
$ docker pull caddy@sha256:735ad7b9a5ba5baf3df5f93034af5fa90c3554da9725d260df238d2511be6b23
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133519902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4fa387ebb822f454dc9877bfe19aaba627e1b422f476a4952468eb35c419c3f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 21:16:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 21:16:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 21:16:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:20:19 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:21:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:21:57 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:21:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:21:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:21:57 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:49:49 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:49:49 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:49:49 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:49:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:49:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:49:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:49:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4583459ba0371c715f926a9bbd37a9dae909234f4b898220160425131eb53bd4`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 284.7 KB (284734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c1e223e6f2123b855e0c95898eba50cb6a055881ba9023527c0a361761c1cf`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbef1b99e503551b709afdb24ef66954c0792f99d76bb0018afd3a65a1347b5b`  
		Last Modified: Tue, 01 Nov 2022 19:30:19 GMT  
		Size: 122.3 MB (122275572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99825e86aac9391fd3d709522864ff3282479450067b8431df9c4f9e4da4da1`  
		Last Modified: Tue, 01 Nov 2022 19:30:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd6f4fde4a1bb5cc5dd5adba9566a8e0e11ac8cf06adffd9dbefe69a80fc50e`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 6.9 MB (6937644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc2cb786c4d70bac77de2092dd9d3fe5b54e59daa8918ccd6ce64d32929e339`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 1.2 MB (1215184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189da6bcd6c18118e6c5774a9bf9eaba6cde20b87848c17960d265f518beb280`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2b94490e7740d5762996c3f1af82a99c3a298122ab46f5312d75b015ed07fdb3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129501509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:484eab50c7b23327b3246fbfe1577b2cb318df92dd5e1e7695611bc34588a965`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 01 Nov 2022 18:49:34 GMT
RUN apk add --no-cache ca-certificates
# Tue, 01 Nov 2022 18:49:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Nov 2022 18:49:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:49:35 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:51:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:51:57 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:51:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:51:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:51:58 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:18:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:18:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:18:14 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:18:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:18:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:18:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:18:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e34adf14e74afbe714188593430596566b859daec67932063af22ae26cfb41`  
		Last Modified: Tue, 01 Nov 2022 18:59:56 GMT  
		Size: 284.6 KB (284604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30829221241bb1a4c4b78ced30216bd6e772290df6d02b43de82ec13847f2ea`  
		Last Modified: Tue, 01 Nov 2022 18:59:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5175fa50505ed8e1ebb1cc778186a5571aceaf68880fb7f30ce0a002543fde16`  
		Last Modified: Tue, 01 Nov 2022 19:00:18 GMT  
		Size: 118.6 MB (118633129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9462914fb6be31fa7883e2ac24e0b90c77b0dd01eed92e5eb2717d2d58757a21`  
		Last Modified: Tue, 01 Nov 2022 18:59:55 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bae57654f3779f11c3403f04b1e6edc1160b85b75ec1b7aaeebd3ab918fdb3e`  
		Last Modified: Tue, 01 Nov 2022 19:19:10 GMT  
		Size: 6.8 MB (6806143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ccbb51616839b72199c780dc3fb4b40d6337c1b64a8e503b85e43d17ae6bee`  
		Last Modified: Tue, 01 Nov 2022 19:19:09 GMT  
		Size: 1.2 MB (1162983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8bf63e08652d8b6f6f6f0710daa4bfdfd8cd8a9b63599b309be0e046fb2405`  
		Last Modified: Tue, 01 Nov 2022 19:19:09 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:38e0977df61d81ad978adc5aeff5351e967c86e79faa8b7707674d0ac2e63774
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128321867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0724d3115962e959325f2a9a4a8824cd2292a204ddd5db99808f8c1c3b28610a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 03:11:14 GMT
RUN apk add --no-cache ca-certificates
# Thu, 27 Oct 2022 03:11:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 03:11:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:58:35 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:00:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:00:36 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:00:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:00:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:00:37 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:30:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:30:18 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:30:18 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:30:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:30:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:30:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:30:20 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb4eb882dd734293a28e32a55182efac09a590954d1c7e0ac4e9afd668b950f`  
		Last Modified: Thu, 27 Oct 2022 03:23:31 GMT  
		Size: 283.8 KB (283751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62601eba0f2135ba01bd7632b6cd5858fd87c654ebbd7aa446022efda221518`  
		Last Modified: Thu, 27 Oct 2022 03:23:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f8cf932723cb79c6511c7a4565c26fc3c1a8b195b63a1b4f27567664469b8`  
		Last Modified: Tue, 01 Nov 2022 19:11:07 GMT  
		Size: 118.4 MB (118395001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06295a7c5807cf45167f1a47e93084873628c3417ae38bd41c276b71ba1c46ab`  
		Last Modified: Tue, 01 Nov 2022 19:10:45 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92d8ff62b16b450357e75981f8b6277cddab5a79836683195be024c5b466eb1`  
		Last Modified: Tue, 01 Nov 2022 19:31:14 GMT  
		Size: 6.1 MB (6065387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136c853b146e693b550c1d68b6b6713b79d7befffc79acb1530b83593b8fa935`  
		Last Modified: Tue, 01 Nov 2022 19:31:13 GMT  
		Size: 1.2 MB (1159979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f924d6193ccce35a47a6ee295f40e327abf4a8492374030689faf3f505632e08`  
		Last Modified: Tue, 01 Nov 2022 19:31:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6b8569ece82b11e5f6720884af16dce90859af84c6a9ab271ce05a08435fbd77
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127999797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1543ea235e3a8ec3d0ad049bdc81b95745b72848028c6dbc10cde12da0b876fc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 26 Oct 2022 08:09:57 GMT
RUN apk add --no-cache ca-certificates
# Wed, 26 Oct 2022 08:09:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 Oct 2022 08:09:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:40:17 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:41:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:41:34 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:41:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:41:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:41:35 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:05:53 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:05:53 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:05:53 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:05:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:05:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:05:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:05:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d82f9e3411d2eff49049d09ae871e53b96a0cc7dd335883f1fec28c43f9c86`  
		Last Modified: Wed, 26 Oct 2022 08:17:16 GMT  
		Size: 284.7 KB (284723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e169736571560c1a3278f9971532d55ddc4abfaef12e8c54c05f4644445d5520`  
		Last Modified: Wed, 26 Oct 2022 08:17:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc530f9a61e7c0e16b1cb3d48b70136b625cf624976acc638b9d6aef5525995`  
		Last Modified: Tue, 01 Nov 2022 18:48:07 GMT  
		Size: 116.8 MB (116836732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562d55c2123be45d40bfd4dd4dea65161ad3d83b50153de3cc0b63ec7a061f4b`  
		Last Modified: Tue, 01 Nov 2022 18:47:54 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90594629b6df4d09d221ea3fc570b4944e36520a3503ffa3a838772b0e46561`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 7.0 MB (7049481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e41bd715f5f0d05c59b600661a8f0cfb5145de632b14a77d012cfd1ffeea780`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 1.1 MB (1120483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3da6b029e0d694358fe69ed7435eb464495babb3bc51d3d5f30a5222406935`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:0bfdd9fd29aabe5e64b1c692ef01a8064dc2c4932747c3bf06363fd238817630
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128911035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3d666ccc1132e45cb0e54d7fd1891ab309ad3ae1fa96a20556f67f531c4bcc0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:26:01 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:26:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:26:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:17:13 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:19:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:20:03 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:20:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:20:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:20:05 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:50:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:50:46 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:50:46 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:50:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:50:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:50:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:50:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36899d7325c2c25a7d8e61ef33bb1e93b83f811f462e9ddad81c86df87b0685`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 286.7 KB (286747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9309524edda98df2abd6704c6f56004422a28b63364f028763ea000fc32d6eca`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b608654249afe5c44e2b3f100f6b333302506cd24adc46afa3302bb03ff96e`  
		Last Modified: Tue, 01 Nov 2022 19:31:59 GMT  
		Size: 117.2 MB (117238077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93311758f4ff1a16fa50dab5c51c12dd47a1920496e07493f5452c97e24eff9c`  
		Last Modified: Tue, 01 Nov 2022 19:31:32 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce6b57ae4a73b81094351a45358cebcbfbccd4d0d31ab77e71afc97d675dc63`  
		Last Modified: Tue, 01 Nov 2022 19:51:34 GMT  
		Size: 7.5 MB (7478322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5fa9d97b98179c5269f7f488f5488ec1a31fa543c75dc88705c8ed0a755e1c`  
		Last Modified: Tue, 01 Nov 2022 19:51:33 GMT  
		Size: 1.1 MB (1103853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f6efc0777ee24d394842b20cc0fe8c229ae5fecbb8dbb5537e66f5fc1fcf41`  
		Last Modified: Tue, 01 Nov 2022 19:51:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; s390x

```console
$ docker pull caddy@sha256:660f4e58ece536977f580dad53c004e3fe9b1496a0af262adf93a8480746e615
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131825256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d3b89f5e95a2acfe27efc6ab49664e2a25268891a03b26100d1cca071938a79`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:16:09 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:16:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:16:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:43:10 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:46:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:47:10 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:47:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:47:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:47:13 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:20:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:20:25 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:20:26 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:20:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:20:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:20:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:20:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d31ae2e1f77c70a25e9cbeea435b4ab68149a4e17f9d4668768da8dd5ac68a`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 285.0 KB (284954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2788e533105e3c00ed84523a8f99d7947c0bb8b12932018a3081ecc29964605`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a12f83dfb1b48c3152a859b9b55b4483128b0be37e4877271cbd453b23fb43`  
		Last Modified: Tue, 01 Nov 2022 19:02:36 GMT  
		Size: 120.7 MB (120729474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e663873bb0a71689aee0be3ce5f4195e0b573039585fcc3182fe189e8e8fe05`  
		Last Modified: Tue, 01 Nov 2022 19:02:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802d29971118d482599687d5c1f1c069a8f0b8cb0c96e3ec3d5f550416223491`  
		Last Modified: Tue, 01 Nov 2022 19:21:20 GMT  
		Size: 7.1 MB (7052072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eea39f6b8018dc8d0011d05cdf7f2412b1435fdedc607d0087cfb9c631ccc23`  
		Last Modified: Tue, 01 Nov 2022 19:21:19 GMT  
		Size: 1.2 MB (1167444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a34c766fedcef740b10fddb96cd1ffd7aeae2d9628ddfa2510fedd4bbe64d2b`  
		Last Modified: Tue, 01 Nov 2022 19:21:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - windows version 10.0.17763.3532; amd64

```console
$ docker pull caddy@sha256:f279c274451500e517aada07ecabddffd03b23f0b9d81791d2347e369b267a6f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2958579667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c57c677f08a022815e25e725365624f628555a00eab2b42f1830e71794c949`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 12:45:06 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Oct 2022 12:45:07 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Oct 2022 12:45:08 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Oct 2022 12:45:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Oct 2022 12:46:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Oct 2022 12:46:38 GMT
ENV GOPATH=C:\go
# Wed, 12 Oct 2022 12:47:37 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 01 Nov 2022 19:19:52 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:25:48 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 01 Nov 2022 19:25:50 GMT
WORKDIR C:\go
# Tue, 01 Nov 2022 20:18:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 01 Nov 2022 20:18:12 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 20:18:13 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 20:18:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 20:19:33 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 01 Nov 2022 20:19:34 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094a4c27e78f8821517fd551cd9e3d5f4b1e4199bdcd783b3fbda849e4995ad1`  
		Last Modified: Wed, 12 Oct 2022 13:16:26 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e91de5ff2103556b1048388473379f95d41247701f0911ebc7c530a861f3f5e`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52642f9e5e3a52bef8ee5677bcb62a364e07003da51f16eb28b8a4ce34fe9f7d`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26528ba698d400f5680be93457d24581b9e4e7a2399de7bb23cbd549f206613`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c89703eb31300a2a39c85ce287a6b9fe88da033828368275bdbb53c2f7704c`  
		Last Modified: Wed, 12 Oct 2022 13:16:30 GMT  
		Size: 25.4 MB (25439927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8705eaae12fa4840be2d79e376eb1b4b7b18da881acad2892b1c47336e796f46`  
		Last Modified: Wed, 12 Oct 2022 13:16:19 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebda8897c2727e3b971c947385632df6f19de06da75e9f161200d43d1acf714`  
		Last Modified: Wed, 12 Oct 2022 13:16:19 GMT  
		Size: 315.0 KB (315035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8667d37dce62bb077cd534d490f047b61dfe9c30023659258862cada9cbd0ba`  
		Last Modified: Tue, 01 Nov 2022 19:54:40 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac8e32e89f1739964a644b8b8b5b44bbae9752f8ea1f87e93455ca36cc86a7d`  
		Last Modified: Tue, 01 Nov 2022 19:55:33 GMT  
		Size: 157.7 MB (157676844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cabbd4ff51bc72ab20efd9f4eb4ebb788679ef03c2fc9b8a72f711fe3558590`  
		Last Modified: Tue, 01 Nov 2022 19:54:40 GMT  
		Size: 1.5 KB (1459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a7aa6766a51e2f5a5add77b40fd7eafa9d3d5049c3b4506b6b4e6dffb65cd6`  
		Last Modified: Tue, 01 Nov 2022 20:21:08 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54feb136a1e02e5d213be9750ca621c39022ff48f54c1e67daace9a82dd241f1`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7c0ce28f0f06a413d72723dbca806a7b025194983d436501cb04b7b2d7379`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e48594ab78eca9cfe42619a2f721de764c027be8fa22700565227c765b4ed7e`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55feb68cd00871cb13079eb862d65521274326d062594c7522edcc8f9bac23f1`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.6 MB (1631634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d398f623f33e057b5d399473e3ee1243fef32140e9a4411c1f69a913b43acb08`  
		Last Modified: Tue, 01 Nov 2022 20:21:05 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - windows version 10.0.20348.1129; amd64

```console
$ docker pull caddy@sha256:6e35c0ddda3afe05cb015c908260022b09ae192d81ad72f3bf1e32c70d7cb243
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2659936170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:265570f6cf9dffda304fb3a6712c85940e0f8d23ef6d8ffbfd8e1ebdd6d89d85`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 12:40:52 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Oct 2022 12:40:53 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Oct 2022 12:40:54 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Oct 2022 12:40:55 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Oct 2022 12:41:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Oct 2022 12:41:26 GMT
ENV GOPATH=C:\go
# Wed, 12 Oct 2022 12:41:47 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 01 Nov 2022 19:15:18 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:19:35 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 01 Nov 2022 19:19:38 GMT
WORKDIR C:\go
# Tue, 01 Nov 2022 20:19:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 01 Nov 2022 20:19:43 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 20:19:45 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 20:19:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 20:20:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 01 Nov 2022 20:20:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e9b54b31e104f64c9eb8a65ac0af5effd645bd00a77ea297b6015d28022a74`  
		Last Modified: Mon, 17 Oct 2022 21:39:11 GMT  
		Size: 1000.0 MB (1000028645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f8b589252b90e37349f39b9d4495646791b4050d7cd218336fcc4624b0ebe2`  
		Last Modified: Wed, 12 Oct 2022 13:15:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811ef63d5261b55ee6b499dbc7fcd1ed13386326466fb81a0801abbcbcb75d3f`  
		Last Modified: Wed, 12 Oct 2022 13:15:28 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816740cd643a7a4e72aa527cd033d0c95686c9725ff70dac3260b44dce508e73`  
		Last Modified: Wed, 12 Oct 2022 13:15:28 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599e30c8b316e75d786cfd91f97b9fae4c89fb00f3fce0619eb4e66bc3165521`  
		Last Modified: Wed, 12 Oct 2022 13:15:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77a0d37b81c920d4b783c0b2cfad656a4b8733960ba3afd4e0a1f39f202f948`  
		Last Modified: Wed, 12 Oct 2022 13:15:32 GMT  
		Size: 25.7 MB (25689345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b699f53b56e90279b0bb8ce4434f9b68bbc28fa30756476e22c7ef3dc869e24a`  
		Last Modified: Wed, 12 Oct 2022 13:15:21 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57fcf632f60c89dd981a8a7fa084e738f55129b1786fd9a9e9f5ab8aa1e02d82`  
		Last Modified: Wed, 12 Oct 2022 13:15:24 GMT  
		Size: 526.5 KB (526519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8b0d888223c93af8f0c84ad35156f79df9b0d9ae107f61ded320d2a4fed5f3`  
		Last Modified: Tue, 01 Nov 2022 19:53:29 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49602de12fff655f45d03b1befdd7e56321771c65ed690492e4092da51046bb3`  
		Last Modified: Tue, 01 Nov 2022 19:54:22 GMT  
		Size: 157.8 MB (157838831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cb5ede4eaf1f86f7c0957639a8b53a0c6740df6fa395d3d286e32bff6b9195`  
		Last Modified: Tue, 01 Nov 2022 19:53:29 GMT  
		Size: 1.6 KB (1584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d0ae347408d32205a9ca4c0628e814833984ac8c0fbfb6c6687b9c94a733aa`  
		Last Modified: Tue, 01 Nov 2022 20:21:30 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453489637085324b6412fd9d83cc639d7a9f9135fb5db5dec214462b3293c98f`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cc23fcabe43926f14c7d7e786e9175c87fe573e41fc0158bdc02cfc08fb567`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528f2dc5e38ba5bad570845252c13446ea9637f9c7a80590c93c28886ab79803`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd45b40a0e40f3a52f9a7e2e1cf3cf3b0501ca3f8d637ef46596ee30a9193264`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.8 MB (1837122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bd243dcf25ec803b906e53fa263b2803735773f0227c1c4bac5d52654bb8c6`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder-alpine`

```console
$ docker pull caddy@sha256:9a51f1a1098ec283efeb9174633447c4bb3142e5bbc7649c8ced7f8d685da3f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.6-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:735ad7b9a5ba5baf3df5f93034af5fa90c3554da9725d260df238d2511be6b23
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133519902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4fa387ebb822f454dc9877bfe19aaba627e1b422f476a4952468eb35c419c3f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 21:16:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 21:16:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 21:16:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:20:19 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:21:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:21:57 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:21:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:21:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:21:57 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:49:49 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:49:49 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:49:49 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:49:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:49:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:49:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:49:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4583459ba0371c715f926a9bbd37a9dae909234f4b898220160425131eb53bd4`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 284.7 KB (284734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c1e223e6f2123b855e0c95898eba50cb6a055881ba9023527c0a361761c1cf`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbef1b99e503551b709afdb24ef66954c0792f99d76bb0018afd3a65a1347b5b`  
		Last Modified: Tue, 01 Nov 2022 19:30:19 GMT  
		Size: 122.3 MB (122275572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99825e86aac9391fd3d709522864ff3282479450067b8431df9c4f9e4da4da1`  
		Last Modified: Tue, 01 Nov 2022 19:30:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd6f4fde4a1bb5cc5dd5adba9566a8e0e11ac8cf06adffd9dbefe69a80fc50e`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 6.9 MB (6937644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc2cb786c4d70bac77de2092dd9d3fe5b54e59daa8918ccd6ce64d32929e339`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 1.2 MB (1215184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189da6bcd6c18118e6c5774a9bf9eaba6cde20b87848c17960d265f518beb280`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2b94490e7740d5762996c3f1af82a99c3a298122ab46f5312d75b015ed07fdb3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129501509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:484eab50c7b23327b3246fbfe1577b2cb318df92dd5e1e7695611bc34588a965`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 01 Nov 2022 18:49:34 GMT
RUN apk add --no-cache ca-certificates
# Tue, 01 Nov 2022 18:49:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Nov 2022 18:49:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:49:35 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:51:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:51:57 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:51:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:51:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:51:58 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:18:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:18:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:18:14 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:18:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:18:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:18:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:18:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e34adf14e74afbe714188593430596566b859daec67932063af22ae26cfb41`  
		Last Modified: Tue, 01 Nov 2022 18:59:56 GMT  
		Size: 284.6 KB (284604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30829221241bb1a4c4b78ced30216bd6e772290df6d02b43de82ec13847f2ea`  
		Last Modified: Tue, 01 Nov 2022 18:59:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5175fa50505ed8e1ebb1cc778186a5571aceaf68880fb7f30ce0a002543fde16`  
		Last Modified: Tue, 01 Nov 2022 19:00:18 GMT  
		Size: 118.6 MB (118633129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9462914fb6be31fa7883e2ac24e0b90c77b0dd01eed92e5eb2717d2d58757a21`  
		Last Modified: Tue, 01 Nov 2022 18:59:55 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bae57654f3779f11c3403f04b1e6edc1160b85b75ec1b7aaeebd3ab918fdb3e`  
		Last Modified: Tue, 01 Nov 2022 19:19:10 GMT  
		Size: 6.8 MB (6806143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ccbb51616839b72199c780dc3fb4b40d6337c1b64a8e503b85e43d17ae6bee`  
		Last Modified: Tue, 01 Nov 2022 19:19:09 GMT  
		Size: 1.2 MB (1162983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8bf63e08652d8b6f6f6f0710daa4bfdfd8cd8a9b63599b309be0e046fb2405`  
		Last Modified: Tue, 01 Nov 2022 19:19:09 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:38e0977df61d81ad978adc5aeff5351e967c86e79faa8b7707674d0ac2e63774
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128321867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0724d3115962e959325f2a9a4a8824cd2292a204ddd5db99808f8c1c3b28610a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 03:11:14 GMT
RUN apk add --no-cache ca-certificates
# Thu, 27 Oct 2022 03:11:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 03:11:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:58:35 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:00:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:00:36 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:00:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:00:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:00:37 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:30:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:30:18 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:30:18 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:30:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:30:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:30:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:30:20 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb4eb882dd734293a28e32a55182efac09a590954d1c7e0ac4e9afd668b950f`  
		Last Modified: Thu, 27 Oct 2022 03:23:31 GMT  
		Size: 283.8 KB (283751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62601eba0f2135ba01bd7632b6cd5858fd87c654ebbd7aa446022efda221518`  
		Last Modified: Thu, 27 Oct 2022 03:23:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f8cf932723cb79c6511c7a4565c26fc3c1a8b195b63a1b4f27567664469b8`  
		Last Modified: Tue, 01 Nov 2022 19:11:07 GMT  
		Size: 118.4 MB (118395001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06295a7c5807cf45167f1a47e93084873628c3417ae38bd41c276b71ba1c46ab`  
		Last Modified: Tue, 01 Nov 2022 19:10:45 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92d8ff62b16b450357e75981f8b6277cddab5a79836683195be024c5b466eb1`  
		Last Modified: Tue, 01 Nov 2022 19:31:14 GMT  
		Size: 6.1 MB (6065387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136c853b146e693b550c1d68b6b6713b79d7befffc79acb1530b83593b8fa935`  
		Last Modified: Tue, 01 Nov 2022 19:31:13 GMT  
		Size: 1.2 MB (1159979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f924d6193ccce35a47a6ee295f40e327abf4a8492374030689faf3f505632e08`  
		Last Modified: Tue, 01 Nov 2022 19:31:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6b8569ece82b11e5f6720884af16dce90859af84c6a9ab271ce05a08435fbd77
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127999797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1543ea235e3a8ec3d0ad049bdc81b95745b72848028c6dbc10cde12da0b876fc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 26 Oct 2022 08:09:57 GMT
RUN apk add --no-cache ca-certificates
# Wed, 26 Oct 2022 08:09:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 Oct 2022 08:09:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:40:17 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:41:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:41:34 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:41:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:41:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:41:35 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:05:53 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:05:53 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:05:53 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:05:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:05:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:05:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:05:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d82f9e3411d2eff49049d09ae871e53b96a0cc7dd335883f1fec28c43f9c86`  
		Last Modified: Wed, 26 Oct 2022 08:17:16 GMT  
		Size: 284.7 KB (284723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e169736571560c1a3278f9971532d55ddc4abfaef12e8c54c05f4644445d5520`  
		Last Modified: Wed, 26 Oct 2022 08:17:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc530f9a61e7c0e16b1cb3d48b70136b625cf624976acc638b9d6aef5525995`  
		Last Modified: Tue, 01 Nov 2022 18:48:07 GMT  
		Size: 116.8 MB (116836732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562d55c2123be45d40bfd4dd4dea65161ad3d83b50153de3cc0b63ec7a061f4b`  
		Last Modified: Tue, 01 Nov 2022 18:47:54 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90594629b6df4d09d221ea3fc570b4944e36520a3503ffa3a838772b0e46561`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 7.0 MB (7049481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e41bd715f5f0d05c59b600661a8f0cfb5145de632b14a77d012cfd1ffeea780`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 1.1 MB (1120483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3da6b029e0d694358fe69ed7435eb464495babb3bc51d3d5f30a5222406935`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:0bfdd9fd29aabe5e64b1c692ef01a8064dc2c4932747c3bf06363fd238817630
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128911035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3d666ccc1132e45cb0e54d7fd1891ab309ad3ae1fa96a20556f67f531c4bcc0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:26:01 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:26:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:26:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:17:13 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:19:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:20:03 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:20:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:20:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:20:05 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:50:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:50:46 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:50:46 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:50:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:50:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:50:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:50:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36899d7325c2c25a7d8e61ef33bb1e93b83f811f462e9ddad81c86df87b0685`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 286.7 KB (286747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9309524edda98df2abd6704c6f56004422a28b63364f028763ea000fc32d6eca`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b608654249afe5c44e2b3f100f6b333302506cd24adc46afa3302bb03ff96e`  
		Last Modified: Tue, 01 Nov 2022 19:31:59 GMT  
		Size: 117.2 MB (117238077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93311758f4ff1a16fa50dab5c51c12dd47a1920496e07493f5452c97e24eff9c`  
		Last Modified: Tue, 01 Nov 2022 19:31:32 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce6b57ae4a73b81094351a45358cebcbfbccd4d0d31ab77e71afc97d675dc63`  
		Last Modified: Tue, 01 Nov 2022 19:51:34 GMT  
		Size: 7.5 MB (7478322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5fa9d97b98179c5269f7f488f5488ec1a31fa543c75dc88705c8ed0a755e1c`  
		Last Modified: Tue, 01 Nov 2022 19:51:33 GMT  
		Size: 1.1 MB (1103853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f6efc0777ee24d394842b20cc0fe8c229ae5fecbb8dbb5537e66f5fc1fcf41`  
		Last Modified: Tue, 01 Nov 2022 19:51:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:660f4e58ece536977f580dad53c004e3fe9b1496a0af262adf93a8480746e615
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131825256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d3b89f5e95a2acfe27efc6ab49664e2a25268891a03b26100d1cca071938a79`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:16:09 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:16:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:16:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:43:10 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:46:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:47:10 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:47:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:47:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:47:13 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:20:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:20:25 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:20:26 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:20:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:20:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:20:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:20:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d31ae2e1f77c70a25e9cbeea435b4ab68149a4e17f9d4668768da8dd5ac68a`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 285.0 KB (284954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2788e533105e3c00ed84523a8f99d7947c0bb8b12932018a3081ecc29964605`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a12f83dfb1b48c3152a859b9b55b4483128b0be37e4877271cbd453b23fb43`  
		Last Modified: Tue, 01 Nov 2022 19:02:36 GMT  
		Size: 120.7 MB (120729474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e663873bb0a71689aee0be3ce5f4195e0b573039585fcc3182fe189e8e8fe05`  
		Last Modified: Tue, 01 Nov 2022 19:02:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802d29971118d482599687d5c1f1c069a8f0b8cb0c96e3ec3d5f550416223491`  
		Last Modified: Tue, 01 Nov 2022 19:21:20 GMT  
		Size: 7.1 MB (7052072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eea39f6b8018dc8d0011d05cdf7f2412b1435fdedc607d0087cfb9c631ccc23`  
		Last Modified: Tue, 01 Nov 2022 19:21:19 GMT  
		Size: 1.2 MB (1167444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a34c766fedcef740b10fddb96cd1ffd7aeae2d9628ddfa2510fedd4bbe64d2b`  
		Last Modified: Tue, 01 Nov 2022 19:21:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:ee5b9081fd81e7adbf4a0c1bf8fd4f9f882e755ac9fc03b24f12c7699aa5b52b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `caddy:2.6-builder-windowsservercore-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull caddy@sha256:f279c274451500e517aada07ecabddffd03b23f0b9d81791d2347e369b267a6f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2958579667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c57c677f08a022815e25e725365624f628555a00eab2b42f1830e71794c949`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 12:45:06 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Oct 2022 12:45:07 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Oct 2022 12:45:08 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Oct 2022 12:45:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Oct 2022 12:46:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Oct 2022 12:46:38 GMT
ENV GOPATH=C:\go
# Wed, 12 Oct 2022 12:47:37 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 01 Nov 2022 19:19:52 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:25:48 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 01 Nov 2022 19:25:50 GMT
WORKDIR C:\go
# Tue, 01 Nov 2022 20:18:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 01 Nov 2022 20:18:12 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 20:18:13 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 20:18:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 20:19:33 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 01 Nov 2022 20:19:34 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094a4c27e78f8821517fd551cd9e3d5f4b1e4199bdcd783b3fbda849e4995ad1`  
		Last Modified: Wed, 12 Oct 2022 13:16:26 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e91de5ff2103556b1048388473379f95d41247701f0911ebc7c530a861f3f5e`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52642f9e5e3a52bef8ee5677bcb62a364e07003da51f16eb28b8a4ce34fe9f7d`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26528ba698d400f5680be93457d24581b9e4e7a2399de7bb23cbd549f206613`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c89703eb31300a2a39c85ce287a6b9fe88da033828368275bdbb53c2f7704c`  
		Last Modified: Wed, 12 Oct 2022 13:16:30 GMT  
		Size: 25.4 MB (25439927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8705eaae12fa4840be2d79e376eb1b4b7b18da881acad2892b1c47336e796f46`  
		Last Modified: Wed, 12 Oct 2022 13:16:19 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebda8897c2727e3b971c947385632df6f19de06da75e9f161200d43d1acf714`  
		Last Modified: Wed, 12 Oct 2022 13:16:19 GMT  
		Size: 315.0 KB (315035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8667d37dce62bb077cd534d490f047b61dfe9c30023659258862cada9cbd0ba`  
		Last Modified: Tue, 01 Nov 2022 19:54:40 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac8e32e89f1739964a644b8b8b5b44bbae9752f8ea1f87e93455ca36cc86a7d`  
		Last Modified: Tue, 01 Nov 2022 19:55:33 GMT  
		Size: 157.7 MB (157676844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cabbd4ff51bc72ab20efd9f4eb4ebb788679ef03c2fc9b8a72f711fe3558590`  
		Last Modified: Tue, 01 Nov 2022 19:54:40 GMT  
		Size: 1.5 KB (1459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a7aa6766a51e2f5a5add77b40fd7eafa9d3d5049c3b4506b6b4e6dffb65cd6`  
		Last Modified: Tue, 01 Nov 2022 20:21:08 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54feb136a1e02e5d213be9750ca621c39022ff48f54c1e67daace9a82dd241f1`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7c0ce28f0f06a413d72723dbca806a7b025194983d436501cb04b7b2d7379`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e48594ab78eca9cfe42619a2f721de764c027be8fa22700565227c765b4ed7e`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55feb68cd00871cb13079eb862d65521274326d062594c7522edcc8f9bac23f1`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.6 MB (1631634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d398f623f33e057b5d399473e3ee1243fef32140e9a4411c1f69a913b43acb08`  
		Last Modified: Tue, 01 Nov 2022 20:21:05 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:39520901129debe71fc3b671250e73c438c85ee3435b24c8c8c5bc6293f05800
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1129; amd64

### `caddy:2.6-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1129; amd64

```console
$ docker pull caddy@sha256:6e35c0ddda3afe05cb015c908260022b09ae192d81ad72f3bf1e32c70d7cb243
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2659936170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:265570f6cf9dffda304fb3a6712c85940e0f8d23ef6d8ffbfd8e1ebdd6d89d85`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 12:40:52 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Oct 2022 12:40:53 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Oct 2022 12:40:54 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Oct 2022 12:40:55 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Oct 2022 12:41:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Oct 2022 12:41:26 GMT
ENV GOPATH=C:\go
# Wed, 12 Oct 2022 12:41:47 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 01 Nov 2022 19:15:18 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:19:35 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 01 Nov 2022 19:19:38 GMT
WORKDIR C:\go
# Tue, 01 Nov 2022 20:19:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 01 Nov 2022 20:19:43 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 20:19:45 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 20:19:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 20:20:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 01 Nov 2022 20:20:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e9b54b31e104f64c9eb8a65ac0af5effd645bd00a77ea297b6015d28022a74`  
		Last Modified: Mon, 17 Oct 2022 21:39:11 GMT  
		Size: 1000.0 MB (1000028645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f8b589252b90e37349f39b9d4495646791b4050d7cd218336fcc4624b0ebe2`  
		Last Modified: Wed, 12 Oct 2022 13:15:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811ef63d5261b55ee6b499dbc7fcd1ed13386326466fb81a0801abbcbcb75d3f`  
		Last Modified: Wed, 12 Oct 2022 13:15:28 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816740cd643a7a4e72aa527cd033d0c95686c9725ff70dac3260b44dce508e73`  
		Last Modified: Wed, 12 Oct 2022 13:15:28 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599e30c8b316e75d786cfd91f97b9fae4c89fb00f3fce0619eb4e66bc3165521`  
		Last Modified: Wed, 12 Oct 2022 13:15:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77a0d37b81c920d4b783c0b2cfad656a4b8733960ba3afd4e0a1f39f202f948`  
		Last Modified: Wed, 12 Oct 2022 13:15:32 GMT  
		Size: 25.7 MB (25689345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b699f53b56e90279b0bb8ce4434f9b68bbc28fa30756476e22c7ef3dc869e24a`  
		Last Modified: Wed, 12 Oct 2022 13:15:21 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57fcf632f60c89dd981a8a7fa084e738f55129b1786fd9a9e9f5ab8aa1e02d82`  
		Last Modified: Wed, 12 Oct 2022 13:15:24 GMT  
		Size: 526.5 KB (526519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8b0d888223c93af8f0c84ad35156f79df9b0d9ae107f61ded320d2a4fed5f3`  
		Last Modified: Tue, 01 Nov 2022 19:53:29 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49602de12fff655f45d03b1befdd7e56321771c65ed690492e4092da51046bb3`  
		Last Modified: Tue, 01 Nov 2022 19:54:22 GMT  
		Size: 157.8 MB (157838831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cb5ede4eaf1f86f7c0957639a8b53a0c6740df6fa395d3d286e32bff6b9195`  
		Last Modified: Tue, 01 Nov 2022 19:53:29 GMT  
		Size: 1.6 KB (1584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d0ae347408d32205a9ca4c0628e814833984ac8c0fbfb6c6687b9c94a733aa`  
		Last Modified: Tue, 01 Nov 2022 20:21:30 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453489637085324b6412fd9d83cc639d7a9f9135fb5db5dec214462b3293c98f`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cc23fcabe43926f14c7d7e786e9175c87fe573e41fc0158bdc02cfc08fb567`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528f2dc5e38ba5bad570845252c13446ea9637f9c7a80590c93c28886ab79803`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd45b40a0e40f3a52f9a7e2e1cf3cf3b0501ca3f8d637ef46596ee30a9193264`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.8 MB (1837122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bd243dcf25ec803b906e53fa263b2803735773f0227c1c4bac5d52654bb8c6`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-windowsservercore`

```console
$ docker pull caddy@sha256:a2ab9b4da81fb5793c09308f6353dec3d5aa70255288aa5a9390cf5333e74935
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3532; amd64
	-	windows version 10.0.20348.1129; amd64

### `caddy:2.6-windowsservercore` - windows version 10.0.17763.3532; amd64

```console
$ docker pull caddy@sha256:c795b26fccceaa3ea3738c3d086e0c9da9978392aeb6e2c69ae3d71131b88998
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726785951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a0ffc50daa8e99f5d3029bd930601ec939b66a180da1ad5fef783d1fcb69eb3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 16:58:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:14:49 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:16:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:16:10 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:16:11 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:16:12 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:16:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:16:14 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:16:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:16:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:16:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:16:19 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:16:20 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:16:21 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:16:22 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:17:16 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:17:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:028c482fad0f111537a40f65401f65de54c9fd682951a4f8cf9b644d7c128e18`  
		Size: 834.0 MB (833997855 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77462c8fbd8b2782ee2fc5f09bebfb350912f754186b058478ab8d22f50bb047`  
		Last Modified: Wed, 12 Oct 2022 17:04:34 GMT  
		Size: 358.2 KB (358248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a372be4d9f43d4d5884bc4093c44aedf12150f55ea9457baa2fcceb43ef8074`  
		Last Modified: Thu, 13 Oct 2022 23:21:08 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a8993c29bb6d4c31b0be3609bc7fb2af2666435fe70bb2f329784277d629d1`  
		Last Modified: Thu, 13 Oct 2022 23:21:11 GMT  
		Size: 14.9 MB (14947938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98662b730099437011356fa77ef9072054f4ad73d3781e9b02d4750689762162`  
		Last Modified: Thu, 13 Oct 2022 23:21:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7e77f6a080ad6fa8a7320831868ccd7b6385e995988f2e6cca76090a565c99`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec71d29d036cab0bdbc7765216513aad527933ededfec4492a97724c6bab52d`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a11bac4631094c366303dd3c571fe04cf1b543bafba72d8dd1030f8ae2ec185`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4dc588cdabd0672f8b29c59cd9ddc6d927160284a6f6529fbe39b8e34ca766`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f39777f21d48153f681f16b5a1cd2e12440066bc96a665fa3b85a6275b74942`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638736df2ba6ceaed21b97ee12046d2d0494561bd735581618ab505ff602b0da`  
		Last Modified: Thu, 13 Oct 2022 23:21:04 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e0fe53dba785fdf61d7431392d7e15beeebbe5f215d9a2de2ee00975e7b5c4`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb7b8fc42485b0656b2afcb99344cda044ce10d0107cc91955fbe11433c358`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb8f166931be4f8f0b0a07611df01a8e7d1101f8a8ce564144ded43917e1021`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bc6f4b7a114b7722cfc81aa83b74727261766c2cef9bc0787e447435c33d2a`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5563ab3963680a40da3bc2269bbc1e76362b359547dae9705892cf8f54b50dd1`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d300f0320cd2b8ce3f3e58cbb3acb06e24c5f59a342725056a10667329f914`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfb9dfa0b00914a255876439613219f4a74e83734df6b8a197e6e0bb53bf905`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b9233dbf203ca77eea2271813856d219ba7d2f633adf99f3262612edfad738`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 291.8 KB (291836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefde31b509f056641749adae4daa4e0ad3265d260ac1c61b41c8950a10824e6`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-windowsservercore` - windows version 10.0.20348.1129; amd64

```console
$ docker pull caddy@sha256:e1e15c80e157d71221ec43035cae93b3ea8ba7a6b203428e93159aa6ff5e1463
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2432333411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbd806ca24dfacee0d098f111cc9f6d5f42fdbd9db91a63a8de0d048d3984d5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 17:01:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:17:37 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:18:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:18:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:18:13 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:18:13 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:18:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:18:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:18:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:18:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:18:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:18:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:18:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:18:21 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:18:22 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:18:23 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:18:24 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:18:40 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:18:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ab91661ce2a2a2c14684a2ba0f543a81d7896773f88200b31be0e37c589de38`  
		Size: 979.4 MB (979359717 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cd84a277fd91a008fe0c8fc7d6706544075a294512940b16f57998588ea892`  
		Last Modified: Wed, 12 Oct 2022 17:04:58 GMT  
		Size: 616.9 KB (616893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b069dfbedeca0437916f85fdd78a598955839b91ffc4cba4d6327e5c79487`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5263d846656ffa3662062b1a58d9c6d114e00fa5344edc9b93ea5895c4fa46`  
		Last Modified: Thu, 13 Oct 2022 23:21:34 GMT  
		Size: 15.1 MB (15149356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e378404d94c7fb280c51201d60aef05af3196a0ead3b716521cedbe766ba5e3e`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11749bcf2c3e4097f9a1a30d1fc22184e48c94ab54945730c51c36be175c668d`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cb14f39fa0dce5d6dab4bdd1a896c02b5a6bba01dcd46ed36928c2cce27295`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf622a21cfc36d8958be2f273f52b7d4824d500be08f6a2de791506dcc6c981f`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b246af35953d05f1c4292cb1cf8cfc29215ceac2e013ae2a0759aa2d216516`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08367cd2562c20737156e692dca481f835f4832fabb63602fb5edc78494057ae`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6d70510bf329eff739580f04b59acba9cb4aa74e57bcb6fca996d6df6b6d2c`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc6e963fa5949ceb99519a652299dea21a92c9389aadabedb2deeb4e51855b5`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d175d8244325a62c683c4d1fa6cc266f73231f93142fd0f52c3378da6db1464`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4ce9495075c9b00994ef154c9eb0974ba1853a8244869e35af4eecfca4dce7`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceee07aab1c573de692984f7655da9e6c4aee31260b8df8735344242e6f1ff8`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295041dd24e85177aaf7e1bbd1c0b032d2eafaf3da59213972894238dd5b3d72`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3583f031f13dfd9a933b6e8d4808a3ac7f3e007d2e751af9581b76b08b6e0c4a`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1603973d06c7b0a01ab165d727b40f842361ce898a8e7b8579d6bd9db938c8a6`  
		Last Modified: Thu, 13 Oct 2022 23:21:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c4bf5f410b0a58ef5b477fdf99b90ad01e7deb85b685cf06eaae5c9d83a531`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 319.8 KB (319842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da4c854489e4317220200f8dca47e2335696fe8fa9e7a2aa678467b12b4db7b`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-windowsservercore-1809`

```console
$ docker pull caddy@sha256:90bfba2a933ccf3d365ad190142c6752ca1cc5910eed29fec903f40ea0e63df9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `caddy:2.6-windowsservercore-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull caddy@sha256:b411d08c1e0b31af2ab78b7ce20efb6839b59d7fb1a06c3cddb9258b210a3e6d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2789120357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a0ffc50daa8e99f5d3029bd930601ec939b66a180da1ad5fef783d1fcb69eb3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 16:58:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:14:49 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:16:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:16:10 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:16:11 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:16:12 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:16:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:16:14 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:16:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:16:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:16:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:16:19 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:16:20 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:16:21 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:16:22 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:17:16 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:17:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77462c8fbd8b2782ee2fc5f09bebfb350912f754186b058478ab8d22f50bb047`  
		Last Modified: Wed, 12 Oct 2022 17:04:34 GMT  
		Size: 358.2 KB (358248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a372be4d9f43d4d5884bc4093c44aedf12150f55ea9457baa2fcceb43ef8074`  
		Last Modified: Thu, 13 Oct 2022 23:21:08 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a8993c29bb6d4c31b0be3609bc7fb2af2666435fe70bb2f329784277d629d1`  
		Last Modified: Thu, 13 Oct 2022 23:21:11 GMT  
		Size: 14.9 MB (14947938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98662b730099437011356fa77ef9072054f4ad73d3781e9b02d4750689762162`  
		Last Modified: Thu, 13 Oct 2022 23:21:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7e77f6a080ad6fa8a7320831868ccd7b6385e995988f2e6cca76090a565c99`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec71d29d036cab0bdbc7765216513aad527933ededfec4492a97724c6bab52d`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a11bac4631094c366303dd3c571fe04cf1b543bafba72d8dd1030f8ae2ec185`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4dc588cdabd0672f8b29c59cd9ddc6d927160284a6f6529fbe39b8e34ca766`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f39777f21d48153f681f16b5a1cd2e12440066bc96a665fa3b85a6275b74942`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638736df2ba6ceaed21b97ee12046d2d0494561bd735581618ab505ff602b0da`  
		Last Modified: Thu, 13 Oct 2022 23:21:04 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e0fe53dba785fdf61d7431392d7e15beeebbe5f215d9a2de2ee00975e7b5c4`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb7b8fc42485b0656b2afcb99344cda044ce10d0107cc91955fbe11433c358`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb8f166931be4f8f0b0a07611df01a8e7d1101f8a8ce564144ded43917e1021`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bc6f4b7a114b7722cfc81aa83b74727261766c2cef9bc0787e447435c33d2a`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5563ab3963680a40da3bc2269bbc1e76362b359547dae9705892cf8f54b50dd1`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d300f0320cd2b8ce3f3e58cbb3acb06e24c5f59a342725056a10667329f914`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfb9dfa0b00914a255876439613219f4a74e83734df6b8a197e6e0bb53bf905`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b9233dbf203ca77eea2271813856d219ba7d2f633adf99f3262612edfad738`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 291.8 KB (291836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefde31b509f056641749adae4daa4e0ad3265d260ac1c61b41c8950a10824e6`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:9d8443f679bf4d3a6de40532eae2adc79a55effdb55e201c986a17f267ed1f79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1129; amd64

### `caddy:2.6-windowsservercore-ltsc2022` - windows version 10.0.20348.1129; amd64

```console
$ docker pull caddy@sha256:a703a1324c3d21a7ef24a692ed804585cce687982f0c9b728d4e02c95e9238cd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2490136360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbd806ca24dfacee0d098f111cc9f6d5f42fdbd9db91a63a8de0d048d3984d5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 17:01:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:17:37 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:18:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:18:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:18:13 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:18:13 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:18:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:18:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:18:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:18:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:18:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:18:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:18:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:18:21 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:18:22 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:18:23 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:18:24 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:18:40 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:18:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e9b54b31e104f64c9eb8a65ac0af5effd645bd00a77ea297b6015d28022a74`  
		Last Modified: Mon, 17 Oct 2022 21:39:11 GMT  
		Size: 1000.0 MB (1000028645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cd84a277fd91a008fe0c8fc7d6706544075a294512940b16f57998588ea892`  
		Last Modified: Wed, 12 Oct 2022 17:04:58 GMT  
		Size: 616.9 KB (616893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b069dfbedeca0437916f85fdd78a598955839b91ffc4cba4d6327e5c79487`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5263d846656ffa3662062b1a58d9c6d114e00fa5344edc9b93ea5895c4fa46`  
		Last Modified: Thu, 13 Oct 2022 23:21:34 GMT  
		Size: 15.1 MB (15149356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e378404d94c7fb280c51201d60aef05af3196a0ead3b716521cedbe766ba5e3e`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11749bcf2c3e4097f9a1a30d1fc22184e48c94ab54945730c51c36be175c668d`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cb14f39fa0dce5d6dab4bdd1a896c02b5a6bba01dcd46ed36928c2cce27295`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf622a21cfc36d8958be2f273f52b7d4824d500be08f6a2de791506dcc6c981f`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b246af35953d05f1c4292cb1cf8cfc29215ceac2e013ae2a0759aa2d216516`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08367cd2562c20737156e692dca481f835f4832fabb63602fb5edc78494057ae`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6d70510bf329eff739580f04b59acba9cb4aa74e57bcb6fca996d6df6b6d2c`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc6e963fa5949ceb99519a652299dea21a92c9389aadabedb2deeb4e51855b5`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d175d8244325a62c683c4d1fa6cc266f73231f93142fd0f52c3378da6db1464`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4ce9495075c9b00994ef154c9eb0974ba1853a8244869e35af4eecfca4dce7`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceee07aab1c573de692984f7655da9e6c4aee31260b8df8735344242e6f1ff8`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295041dd24e85177aaf7e1bbd1c0b032d2eafaf3da59213972894238dd5b3d72`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3583f031f13dfd9a933b6e8d4808a3ac7f3e007d2e751af9581b76b08b6e0c4a`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1603973d06c7b0a01ab165d727b40f842361ce898a8e7b8579d6bd9db938c8a6`  
		Last Modified: Thu, 13 Oct 2022 23:21:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c4bf5f410b0a58ef5b477fdf99b90ad01e7deb85b685cf06eaae5c9d83a531`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 319.8 KB (319842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da4c854489e4317220200f8dca47e2335696fe8fa9e7a2aa678467b12b4db7b`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.2`

```console
$ docker pull caddy@sha256:d3e5e175b10a2a5b66be9570ed9867aeb77af8eca7a14b6033dcde2c9f6fee6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3532; amd64
	-	windows version 10.0.20348.1129; amd64

### `caddy:2.6.2` - linux; amd64

```console
$ docker pull caddy@sha256:7992b931b7da3cf0840dd69ea74b2c67d423faf03408da8abdc31b7590a239a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17676993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:006d393a4e6a01f82413e41b3e0f06dfb1872d5ca6a37aba315e4ec9e2cc6c4c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:34:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 04:34:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 01:43:19 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 01:43:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 01:43:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 01:43:22 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 01:43:22 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 01:43:22 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 01:43:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 80
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 443
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 01:43:24 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 01:43:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5625668cf98fd3e4d769f18d45f27e34fe3d085cfb9927ff7ad2cdc84d8c493f`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 304.5 KB (304517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675d09b34c5347b62625d31b2a458824240b90e51d18bcc38ad37d317e83d64c`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1747be7065842ba85f86aed65e75608dfd2f546ab9d8ecd4a8842c8f4634795`  
		Last Modified: Fri, 14 Oct 2022 01:43:47 GMT  
		Size: 14.6 MB (14560435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8ee6c4c21d12cd28fcd0e196acb8569f35518dc36c691c91b4c8ca1928bf9d`  
		Last Modified: Fri, 14 Oct 2022 01:43:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:76b70e0dc74358fc1f7ef178c46cc9c047a90cd05e842d26305da1ee04ff3ad8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16834877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cac02415934eaae38be5b122f6a0c760f747e6f50f1551c9a45f4f186454f04`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 19:49:23 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 27 Oct 2022 19:49:25 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 27 Oct 2022 19:49:25 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 27 Oct 2022 19:49:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 27 Oct 2022 19:49:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 19:49:28 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 27 Oct 2022 19:49:28 GMT
ENV XDG_DATA_HOME=/data
# Thu, 27 Oct 2022 19:49:28 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 27 Oct 2022 19:49:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 80
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 443
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 443/udp
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 2019
# Thu, 27 Oct 2022 19:49:30 GMT
WORKDIR /srv
# Thu, 27 Oct 2022 19:49:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7f6197b1f089356a6bff8bf29fdcef692051048bd17db70d72df822c89c04d`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 304.4 KB (304404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc91cb09da181c7973089ccf7aca9c7830c738ac1e614883f86c2eecdcb68002`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 5.8 KB (5751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ffb96b75d9dc6019cfe6202b9fed588b3ff9a91cc89237d6a24c98eb5fd590`  
		Last Modified: Thu, 27 Oct 2022 19:50:36 GMT  
		Size: 13.9 MB (13910603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb4866598fa794379095b277b41d4b0cb626d61cc20c6f6cff7d920bc99330`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9df5bfbadaf5495675c4de47918d3631d439d159681e352069eaa206f664a8ac
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16617541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d61e1121278866d5afee597ba2ac37a9b5bec51b6323b551fe9a89b5d99d63e5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 10:30:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 27 Oct 2022 10:30:41 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 27 Oct 2022 10:30:41 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 27 Oct 2022 10:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 27 Oct 2022 10:30:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 10:30:45 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 27 Oct 2022 10:30:45 GMT
ENV XDG_DATA_HOME=/data
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 27 Oct 2022 10:30:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 80
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 443
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 443/udp
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 2019
# Thu, 27 Oct 2022 10:30:46 GMT
WORKDIR /srv
# Thu, 27 Oct 2022 10:30:46 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9f1011ebc9810d3e61468e7ce6c2866fc65920db06e3bccde2da749f976500`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 303.5 KB (303537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28310071f60503f30048b0cad1abe85c763c57dd4e69715cc57d60560481318`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 5.8 KB (5753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7792abbee8ad8ec28f7e6e2864a9e8ad229de5f701ba4bf04be77cffac8835ac`  
		Last Modified: Thu, 27 Oct 2022 10:31:39 GMT  
		Size: 13.9 MB (13891032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c5be986b3fadf5f34a0a4311ffa6a22b4f1f0ff79c510fb7c58cb93c64e2f3`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f06fb46d2c67f3b7f9447b6c19f5b9909931b603d2b475f647624f577c6d94ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16278669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8876f25c7ec7330d6bf197e452e3a37deeea42e52b8c2b2c9103bc86b26795`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 26 Oct 2022 18:53:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 Oct 2022 18:53:58 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Wed, 26 Oct 2022 18:53:58 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 26 Oct 2022 18:54:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 Oct 2022 18:54:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 Oct 2022 18:54:01 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 Oct 2022 18:54:01 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 80
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 443
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 443/udp
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 2019
# Wed, 26 Oct 2022 18:54:02 GMT
WORKDIR /srv
# Wed, 26 Oct 2022 18:54:02 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5532e6e746eecf0e890ee17251a52841dd55694ae55c919dc6ddf6159e27cd5b`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 304.5 KB (304512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b816658ad2f9debd81f6df21dd733e54fc6eda530080cc3957e6f63d9677b9a`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d7ee92d83c49ca71b5440fd76d22ac6b75304bc48a0183bf392689ae8d5897`  
		Last Modified: Wed, 26 Oct 2022 18:54:26 GMT  
		Size: 13.3 MB (13260508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00da94c60a7ed1fc9acd392aedea2ab7b2bd6a7d67cc83b2d5d85c5cbd40090b`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2` - linux; ppc64le

```console
$ docker pull caddy@sha256:9665c6fd33be967b3bdfcdbeeb605e3a92e70080ef5caa8907a6cbdef064be3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (16031232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96553401995800bf37590502c237b4ab8cee57bd3885e83f76dcb42c53a7d7db`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:56:10 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 07:56:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 03:47:38 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 03:47:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 03:47:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 03:47:44 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 03:47:44 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 03:47:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 03:47:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 80
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 443
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 03:47:49 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 03:47:49 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 03:47:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf49ba2a5c90a152d4aef09519c7019835fbf2884d6afb1c85b3353b7d91388e`  
		Last Modified: Fri, 07 Oct 2022 07:57:09 GMT  
		Size: 306.5 KB (306522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dac87aba8912de3ce6fb3ca14bb6833f931fd15d7ec2d7435a18f11e5ddb6fb`  
		Last Modified: Fri, 07 Oct 2022 07:57:08 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea24f9a44c53fbd359328daff2e10e4e3f1c7d7bae21190ea2f6af3be43dd0b`  
		Last Modified: Fri, 14 Oct 2022 03:48:33 GMT  
		Size: 12.9 MB (12915404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4704e2ddccf987da9605ef1c8d4ef68a86cf3e6ba2f8c5d1e80e5915481e25c`  
		Last Modified: Fri, 14 Oct 2022 03:48:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2` - linux; s390x

```console
$ docker pull caddy@sha256:5702e27172b1bfb5e9930d544d7cf16a83f774419b1aa2078be464351ff5f70b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16967685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05ec4a186bcadcf0e691a443c7edebf42d46cff3997d01a56de43db0ecbab8e2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 10:23:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 10:23:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 00:55:05 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 00:55:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 00:55:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 00:55:15 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 00:55:16 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 00:55:17 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 00:55:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 00:55:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 00:55:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 00:55:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 00:55:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 00:55:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 00:55:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 00:55:22 GMT
EXPOSE 80
# Fri, 14 Oct 2022 00:55:22 GMT
EXPOSE 443
# Fri, 14 Oct 2022 00:55:23 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 00:55:23 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 00:55:24 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 00:55:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5123e0e5a47a6dfbd8cae1e2589df59b198f82ba790c211aeb3eefbbe41a17be`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 304.8 KB (304752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557f08048878eca2f16fd3b05bb138300739b9e74e467509792efc4278e74b3f`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91158060b74650f434cb3419f6ed862b0616480567b651bfae73b297f69b9992`  
		Last Modified: Fri, 14 Oct 2022 00:56:22 GMT  
		Size: 14.1 MB (14066352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511ac9f174e3fed802157937e9192a940800d73835958de90f5a363b5edf46ad`  
		Last Modified: Fri, 14 Oct 2022 00:56:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2` - windows version 10.0.17763.3532; amd64

```console
$ docker pull caddy@sha256:c795b26fccceaa3ea3738c3d086e0c9da9978392aeb6e2c69ae3d71131b88998
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726785951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a0ffc50daa8e99f5d3029bd930601ec939b66a180da1ad5fef783d1fcb69eb3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 16:58:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:14:49 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:16:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:16:10 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:16:11 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:16:12 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:16:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:16:14 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:16:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:16:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:16:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:16:19 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:16:20 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:16:21 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:16:22 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:17:16 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:17:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:028c482fad0f111537a40f65401f65de54c9fd682951a4f8cf9b644d7c128e18`  
		Size: 834.0 MB (833997855 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77462c8fbd8b2782ee2fc5f09bebfb350912f754186b058478ab8d22f50bb047`  
		Last Modified: Wed, 12 Oct 2022 17:04:34 GMT  
		Size: 358.2 KB (358248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a372be4d9f43d4d5884bc4093c44aedf12150f55ea9457baa2fcceb43ef8074`  
		Last Modified: Thu, 13 Oct 2022 23:21:08 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a8993c29bb6d4c31b0be3609bc7fb2af2666435fe70bb2f329784277d629d1`  
		Last Modified: Thu, 13 Oct 2022 23:21:11 GMT  
		Size: 14.9 MB (14947938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98662b730099437011356fa77ef9072054f4ad73d3781e9b02d4750689762162`  
		Last Modified: Thu, 13 Oct 2022 23:21:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7e77f6a080ad6fa8a7320831868ccd7b6385e995988f2e6cca76090a565c99`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec71d29d036cab0bdbc7765216513aad527933ededfec4492a97724c6bab52d`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a11bac4631094c366303dd3c571fe04cf1b543bafba72d8dd1030f8ae2ec185`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4dc588cdabd0672f8b29c59cd9ddc6d927160284a6f6529fbe39b8e34ca766`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f39777f21d48153f681f16b5a1cd2e12440066bc96a665fa3b85a6275b74942`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638736df2ba6ceaed21b97ee12046d2d0494561bd735581618ab505ff602b0da`  
		Last Modified: Thu, 13 Oct 2022 23:21:04 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e0fe53dba785fdf61d7431392d7e15beeebbe5f215d9a2de2ee00975e7b5c4`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb7b8fc42485b0656b2afcb99344cda044ce10d0107cc91955fbe11433c358`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb8f166931be4f8f0b0a07611df01a8e7d1101f8a8ce564144ded43917e1021`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bc6f4b7a114b7722cfc81aa83b74727261766c2cef9bc0787e447435c33d2a`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5563ab3963680a40da3bc2269bbc1e76362b359547dae9705892cf8f54b50dd1`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d300f0320cd2b8ce3f3e58cbb3acb06e24c5f59a342725056a10667329f914`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfb9dfa0b00914a255876439613219f4a74e83734df6b8a197e6e0bb53bf905`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b9233dbf203ca77eea2271813856d219ba7d2f633adf99f3262612edfad738`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 291.8 KB (291836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefde31b509f056641749adae4daa4e0ad3265d260ac1c61b41c8950a10824e6`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2` - windows version 10.0.20348.1129; amd64

```console
$ docker pull caddy@sha256:e1e15c80e157d71221ec43035cae93b3ea8ba7a6b203428e93159aa6ff5e1463
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2432333411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbd806ca24dfacee0d098f111cc9f6d5f42fdbd9db91a63a8de0d048d3984d5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 17:01:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:17:37 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:18:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:18:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:18:13 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:18:13 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:18:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:18:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:18:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:18:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:18:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:18:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:18:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:18:21 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:18:22 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:18:23 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:18:24 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:18:40 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:18:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ab91661ce2a2a2c14684a2ba0f543a81d7896773f88200b31be0e37c589de38`  
		Size: 979.4 MB (979359717 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cd84a277fd91a008fe0c8fc7d6706544075a294512940b16f57998588ea892`  
		Last Modified: Wed, 12 Oct 2022 17:04:58 GMT  
		Size: 616.9 KB (616893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b069dfbedeca0437916f85fdd78a598955839b91ffc4cba4d6327e5c79487`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5263d846656ffa3662062b1a58d9c6d114e00fa5344edc9b93ea5895c4fa46`  
		Last Modified: Thu, 13 Oct 2022 23:21:34 GMT  
		Size: 15.1 MB (15149356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e378404d94c7fb280c51201d60aef05af3196a0ead3b716521cedbe766ba5e3e`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11749bcf2c3e4097f9a1a30d1fc22184e48c94ab54945730c51c36be175c668d`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cb14f39fa0dce5d6dab4bdd1a896c02b5a6bba01dcd46ed36928c2cce27295`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf622a21cfc36d8958be2f273f52b7d4824d500be08f6a2de791506dcc6c981f`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b246af35953d05f1c4292cb1cf8cfc29215ceac2e013ae2a0759aa2d216516`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08367cd2562c20737156e692dca481f835f4832fabb63602fb5edc78494057ae`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6d70510bf329eff739580f04b59acba9cb4aa74e57bcb6fca996d6df6b6d2c`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc6e963fa5949ceb99519a652299dea21a92c9389aadabedb2deeb4e51855b5`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d175d8244325a62c683c4d1fa6cc266f73231f93142fd0f52c3378da6db1464`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4ce9495075c9b00994ef154c9eb0974ba1853a8244869e35af4eecfca4dce7`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceee07aab1c573de692984f7655da9e6c4aee31260b8df8735344242e6f1ff8`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295041dd24e85177aaf7e1bbd1c0b032d2eafaf3da59213972894238dd5b3d72`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3583f031f13dfd9a933b6e8d4808a3ac7f3e007d2e751af9581b76b08b6e0c4a`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1603973d06c7b0a01ab165d727b40f842361ce898a8e7b8579d6bd9db938c8a6`  
		Last Modified: Thu, 13 Oct 2022 23:21:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c4bf5f410b0a58ef5b477fdf99b90ad01e7deb85b685cf06eaae5c9d83a531`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 319.8 KB (319842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da4c854489e4317220200f8dca47e2335696fe8fa9e7a2aa678467b12b4db7b`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.2-alpine`

```console
$ docker pull caddy@sha256:0e3c6d476eb251d2e271c61d12472698e2be1909626d342c405ed58c70772857
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.6.2-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:7992b931b7da3cf0840dd69ea74b2c67d423faf03408da8abdc31b7590a239a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17676993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:006d393a4e6a01f82413e41b3e0f06dfb1872d5ca6a37aba315e4ec9e2cc6c4c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:34:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 04:34:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 01:43:19 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 01:43:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 01:43:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 01:43:22 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 01:43:22 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 01:43:22 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 01:43:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 80
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 443
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 01:43:24 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 01:43:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5625668cf98fd3e4d769f18d45f27e34fe3d085cfb9927ff7ad2cdc84d8c493f`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 304.5 KB (304517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675d09b34c5347b62625d31b2a458824240b90e51d18bcc38ad37d317e83d64c`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1747be7065842ba85f86aed65e75608dfd2f546ab9d8ecd4a8842c8f4634795`  
		Last Modified: Fri, 14 Oct 2022 01:43:47 GMT  
		Size: 14.6 MB (14560435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8ee6c4c21d12cd28fcd0e196acb8569f35518dc36c691c91b4c8ca1928bf9d`  
		Last Modified: Fri, 14 Oct 2022 01:43:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:76b70e0dc74358fc1f7ef178c46cc9c047a90cd05e842d26305da1ee04ff3ad8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16834877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cac02415934eaae38be5b122f6a0c760f747e6f50f1551c9a45f4f186454f04`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 19:49:23 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 27 Oct 2022 19:49:25 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 27 Oct 2022 19:49:25 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 27 Oct 2022 19:49:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 27 Oct 2022 19:49:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 19:49:28 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 27 Oct 2022 19:49:28 GMT
ENV XDG_DATA_HOME=/data
# Thu, 27 Oct 2022 19:49:28 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 27 Oct 2022 19:49:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 80
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 443
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 443/udp
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 2019
# Thu, 27 Oct 2022 19:49:30 GMT
WORKDIR /srv
# Thu, 27 Oct 2022 19:49:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7f6197b1f089356a6bff8bf29fdcef692051048bd17db70d72df822c89c04d`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 304.4 KB (304404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc91cb09da181c7973089ccf7aca9c7830c738ac1e614883f86c2eecdcb68002`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 5.8 KB (5751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ffb96b75d9dc6019cfe6202b9fed588b3ff9a91cc89237d6a24c98eb5fd590`  
		Last Modified: Thu, 27 Oct 2022 19:50:36 GMT  
		Size: 13.9 MB (13910603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb4866598fa794379095b277b41d4b0cb626d61cc20c6f6cff7d920bc99330`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9df5bfbadaf5495675c4de47918d3631d439d159681e352069eaa206f664a8ac
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16617541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d61e1121278866d5afee597ba2ac37a9b5bec51b6323b551fe9a89b5d99d63e5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 10:30:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 27 Oct 2022 10:30:41 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 27 Oct 2022 10:30:41 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 27 Oct 2022 10:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 27 Oct 2022 10:30:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 10:30:45 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 27 Oct 2022 10:30:45 GMT
ENV XDG_DATA_HOME=/data
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 27 Oct 2022 10:30:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 80
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 443
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 443/udp
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 2019
# Thu, 27 Oct 2022 10:30:46 GMT
WORKDIR /srv
# Thu, 27 Oct 2022 10:30:46 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9f1011ebc9810d3e61468e7ce6c2866fc65920db06e3bccde2da749f976500`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 303.5 KB (303537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28310071f60503f30048b0cad1abe85c763c57dd4e69715cc57d60560481318`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 5.8 KB (5753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7792abbee8ad8ec28f7e6e2864a9e8ad229de5f701ba4bf04be77cffac8835ac`  
		Last Modified: Thu, 27 Oct 2022 10:31:39 GMT  
		Size: 13.9 MB (13891032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c5be986b3fadf5f34a0a4311ffa6a22b4f1f0ff79c510fb7c58cb93c64e2f3`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f06fb46d2c67f3b7f9447b6c19f5b9909931b603d2b475f647624f577c6d94ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16278669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8876f25c7ec7330d6bf197e452e3a37deeea42e52b8c2b2c9103bc86b26795`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 26 Oct 2022 18:53:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 Oct 2022 18:53:58 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Wed, 26 Oct 2022 18:53:58 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 26 Oct 2022 18:54:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 Oct 2022 18:54:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 Oct 2022 18:54:01 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 Oct 2022 18:54:01 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 80
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 443
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 443/udp
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 2019
# Wed, 26 Oct 2022 18:54:02 GMT
WORKDIR /srv
# Wed, 26 Oct 2022 18:54:02 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5532e6e746eecf0e890ee17251a52841dd55694ae55c919dc6ddf6159e27cd5b`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 304.5 KB (304512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b816658ad2f9debd81f6df21dd733e54fc6eda530080cc3957e6f63d9677b9a`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d7ee92d83c49ca71b5440fd76d22ac6b75304bc48a0183bf392689ae8d5897`  
		Last Modified: Wed, 26 Oct 2022 18:54:26 GMT  
		Size: 13.3 MB (13260508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00da94c60a7ed1fc9acd392aedea2ab7b2bd6a7d67cc83b2d5d85c5cbd40090b`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:9665c6fd33be967b3bdfcdbeeb605e3a92e70080ef5caa8907a6cbdef064be3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (16031232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96553401995800bf37590502c237b4ab8cee57bd3885e83f76dcb42c53a7d7db`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:56:10 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 07:56:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 03:47:38 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 03:47:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 03:47:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 03:47:44 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 03:47:44 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 03:47:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 03:47:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 80
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 443
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 03:47:49 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 03:47:49 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 03:47:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf49ba2a5c90a152d4aef09519c7019835fbf2884d6afb1c85b3353b7d91388e`  
		Last Modified: Fri, 07 Oct 2022 07:57:09 GMT  
		Size: 306.5 KB (306522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dac87aba8912de3ce6fb3ca14bb6833f931fd15d7ec2d7435a18f11e5ddb6fb`  
		Last Modified: Fri, 07 Oct 2022 07:57:08 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea24f9a44c53fbd359328daff2e10e4e3f1c7d7bae21190ea2f6af3be43dd0b`  
		Last Modified: Fri, 14 Oct 2022 03:48:33 GMT  
		Size: 12.9 MB (12915404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4704e2ddccf987da9605ef1c8d4ef68a86cf3e6ba2f8c5d1e80e5915481e25c`  
		Last Modified: Fri, 14 Oct 2022 03:48:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:5702e27172b1bfb5e9930d544d7cf16a83f774419b1aa2078be464351ff5f70b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16967685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05ec4a186bcadcf0e691a443c7edebf42d46cff3997d01a56de43db0ecbab8e2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 10:23:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 10:23:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 00:55:05 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 00:55:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 00:55:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 00:55:15 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 00:55:16 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 00:55:17 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 00:55:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 00:55:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 00:55:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 00:55:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 00:55:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 00:55:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 00:55:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 00:55:22 GMT
EXPOSE 80
# Fri, 14 Oct 2022 00:55:22 GMT
EXPOSE 443
# Fri, 14 Oct 2022 00:55:23 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 00:55:23 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 00:55:24 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 00:55:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5123e0e5a47a6dfbd8cae1e2589df59b198f82ba790c211aeb3eefbbe41a17be`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 304.8 KB (304752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557f08048878eca2f16fd3b05bb138300739b9e74e467509792efc4278e74b3f`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91158060b74650f434cb3419f6ed862b0616480567b651bfae73b297f69b9992`  
		Last Modified: Fri, 14 Oct 2022 00:56:22 GMT  
		Size: 14.1 MB (14066352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511ac9f174e3fed802157937e9192a940800d73835958de90f5a363b5edf46ad`  
		Last Modified: Fri, 14 Oct 2022 00:56:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.2-builder`

```console
$ docker pull caddy@sha256:9a395d60c9cba0036b919495f7637be3fafb0a97459ee970f1738e0252dfa2f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3532; amd64
	-	windows version 10.0.20348.1129; amd64

### `caddy:2.6.2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:735ad7b9a5ba5baf3df5f93034af5fa90c3554da9725d260df238d2511be6b23
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133519902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4fa387ebb822f454dc9877bfe19aaba627e1b422f476a4952468eb35c419c3f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 21:16:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 21:16:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 21:16:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:20:19 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:21:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:21:57 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:21:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:21:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:21:57 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:49:49 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:49:49 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:49:49 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:49:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:49:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:49:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:49:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4583459ba0371c715f926a9bbd37a9dae909234f4b898220160425131eb53bd4`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 284.7 KB (284734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c1e223e6f2123b855e0c95898eba50cb6a055881ba9023527c0a361761c1cf`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbef1b99e503551b709afdb24ef66954c0792f99d76bb0018afd3a65a1347b5b`  
		Last Modified: Tue, 01 Nov 2022 19:30:19 GMT  
		Size: 122.3 MB (122275572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99825e86aac9391fd3d709522864ff3282479450067b8431df9c4f9e4da4da1`  
		Last Modified: Tue, 01 Nov 2022 19:30:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd6f4fde4a1bb5cc5dd5adba9566a8e0e11ac8cf06adffd9dbefe69a80fc50e`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 6.9 MB (6937644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc2cb786c4d70bac77de2092dd9d3fe5b54e59daa8918ccd6ce64d32929e339`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 1.2 MB (1215184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189da6bcd6c18118e6c5774a9bf9eaba6cde20b87848c17960d265f518beb280`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2b94490e7740d5762996c3f1af82a99c3a298122ab46f5312d75b015ed07fdb3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129501509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:484eab50c7b23327b3246fbfe1577b2cb318df92dd5e1e7695611bc34588a965`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 01 Nov 2022 18:49:34 GMT
RUN apk add --no-cache ca-certificates
# Tue, 01 Nov 2022 18:49:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Nov 2022 18:49:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:49:35 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:51:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:51:57 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:51:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:51:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:51:58 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:18:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:18:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:18:14 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:18:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:18:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:18:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:18:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e34adf14e74afbe714188593430596566b859daec67932063af22ae26cfb41`  
		Last Modified: Tue, 01 Nov 2022 18:59:56 GMT  
		Size: 284.6 KB (284604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30829221241bb1a4c4b78ced30216bd6e772290df6d02b43de82ec13847f2ea`  
		Last Modified: Tue, 01 Nov 2022 18:59:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5175fa50505ed8e1ebb1cc778186a5571aceaf68880fb7f30ce0a002543fde16`  
		Last Modified: Tue, 01 Nov 2022 19:00:18 GMT  
		Size: 118.6 MB (118633129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9462914fb6be31fa7883e2ac24e0b90c77b0dd01eed92e5eb2717d2d58757a21`  
		Last Modified: Tue, 01 Nov 2022 18:59:55 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bae57654f3779f11c3403f04b1e6edc1160b85b75ec1b7aaeebd3ab918fdb3e`  
		Last Modified: Tue, 01 Nov 2022 19:19:10 GMT  
		Size: 6.8 MB (6806143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ccbb51616839b72199c780dc3fb4b40d6337c1b64a8e503b85e43d17ae6bee`  
		Last Modified: Tue, 01 Nov 2022 19:19:09 GMT  
		Size: 1.2 MB (1162983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8bf63e08652d8b6f6f6f0710daa4bfdfd8cd8a9b63599b309be0e046fb2405`  
		Last Modified: Tue, 01 Nov 2022 19:19:09 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:38e0977df61d81ad978adc5aeff5351e967c86e79faa8b7707674d0ac2e63774
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128321867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0724d3115962e959325f2a9a4a8824cd2292a204ddd5db99808f8c1c3b28610a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 03:11:14 GMT
RUN apk add --no-cache ca-certificates
# Thu, 27 Oct 2022 03:11:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 03:11:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:58:35 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:00:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:00:36 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:00:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:00:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:00:37 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:30:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:30:18 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:30:18 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:30:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:30:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:30:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:30:20 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb4eb882dd734293a28e32a55182efac09a590954d1c7e0ac4e9afd668b950f`  
		Last Modified: Thu, 27 Oct 2022 03:23:31 GMT  
		Size: 283.8 KB (283751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62601eba0f2135ba01bd7632b6cd5858fd87c654ebbd7aa446022efda221518`  
		Last Modified: Thu, 27 Oct 2022 03:23:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f8cf932723cb79c6511c7a4565c26fc3c1a8b195b63a1b4f27567664469b8`  
		Last Modified: Tue, 01 Nov 2022 19:11:07 GMT  
		Size: 118.4 MB (118395001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06295a7c5807cf45167f1a47e93084873628c3417ae38bd41c276b71ba1c46ab`  
		Last Modified: Tue, 01 Nov 2022 19:10:45 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92d8ff62b16b450357e75981f8b6277cddab5a79836683195be024c5b466eb1`  
		Last Modified: Tue, 01 Nov 2022 19:31:14 GMT  
		Size: 6.1 MB (6065387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136c853b146e693b550c1d68b6b6713b79d7befffc79acb1530b83593b8fa935`  
		Last Modified: Tue, 01 Nov 2022 19:31:13 GMT  
		Size: 1.2 MB (1159979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f924d6193ccce35a47a6ee295f40e327abf4a8492374030689faf3f505632e08`  
		Last Modified: Tue, 01 Nov 2022 19:31:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6b8569ece82b11e5f6720884af16dce90859af84c6a9ab271ce05a08435fbd77
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127999797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1543ea235e3a8ec3d0ad049bdc81b95745b72848028c6dbc10cde12da0b876fc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 26 Oct 2022 08:09:57 GMT
RUN apk add --no-cache ca-certificates
# Wed, 26 Oct 2022 08:09:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 Oct 2022 08:09:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:40:17 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:41:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:41:34 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:41:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:41:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:41:35 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:05:53 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:05:53 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:05:53 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:05:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:05:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:05:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:05:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d82f9e3411d2eff49049d09ae871e53b96a0cc7dd335883f1fec28c43f9c86`  
		Last Modified: Wed, 26 Oct 2022 08:17:16 GMT  
		Size: 284.7 KB (284723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e169736571560c1a3278f9971532d55ddc4abfaef12e8c54c05f4644445d5520`  
		Last Modified: Wed, 26 Oct 2022 08:17:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc530f9a61e7c0e16b1cb3d48b70136b625cf624976acc638b9d6aef5525995`  
		Last Modified: Tue, 01 Nov 2022 18:48:07 GMT  
		Size: 116.8 MB (116836732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562d55c2123be45d40bfd4dd4dea65161ad3d83b50153de3cc0b63ec7a061f4b`  
		Last Modified: Tue, 01 Nov 2022 18:47:54 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90594629b6df4d09d221ea3fc570b4944e36520a3503ffa3a838772b0e46561`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 7.0 MB (7049481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e41bd715f5f0d05c59b600661a8f0cfb5145de632b14a77d012cfd1ffeea780`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 1.1 MB (1120483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3da6b029e0d694358fe69ed7435eb464495babb3bc51d3d5f30a5222406935`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:0bfdd9fd29aabe5e64b1c692ef01a8064dc2c4932747c3bf06363fd238817630
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128911035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3d666ccc1132e45cb0e54d7fd1891ab309ad3ae1fa96a20556f67f531c4bcc0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:26:01 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:26:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:26:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:17:13 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:19:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:20:03 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:20:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:20:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:20:05 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:50:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:50:46 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:50:46 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:50:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:50:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:50:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:50:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36899d7325c2c25a7d8e61ef33bb1e93b83f811f462e9ddad81c86df87b0685`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 286.7 KB (286747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9309524edda98df2abd6704c6f56004422a28b63364f028763ea000fc32d6eca`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b608654249afe5c44e2b3f100f6b333302506cd24adc46afa3302bb03ff96e`  
		Last Modified: Tue, 01 Nov 2022 19:31:59 GMT  
		Size: 117.2 MB (117238077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93311758f4ff1a16fa50dab5c51c12dd47a1920496e07493f5452c97e24eff9c`  
		Last Modified: Tue, 01 Nov 2022 19:31:32 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce6b57ae4a73b81094351a45358cebcbfbccd4d0d31ab77e71afc97d675dc63`  
		Last Modified: Tue, 01 Nov 2022 19:51:34 GMT  
		Size: 7.5 MB (7478322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5fa9d97b98179c5269f7f488f5488ec1a31fa543c75dc88705c8ed0a755e1c`  
		Last Modified: Tue, 01 Nov 2022 19:51:33 GMT  
		Size: 1.1 MB (1103853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f6efc0777ee24d394842b20cc0fe8c229ae5fecbb8dbb5537e66f5fc1fcf41`  
		Last Modified: Tue, 01 Nov 2022 19:51:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:660f4e58ece536977f580dad53c004e3fe9b1496a0af262adf93a8480746e615
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131825256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d3b89f5e95a2acfe27efc6ab49664e2a25268891a03b26100d1cca071938a79`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:16:09 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:16:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:16:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:43:10 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:46:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:47:10 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:47:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:47:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:47:13 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:20:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:20:25 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:20:26 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:20:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:20:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:20:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:20:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d31ae2e1f77c70a25e9cbeea435b4ab68149a4e17f9d4668768da8dd5ac68a`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 285.0 KB (284954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2788e533105e3c00ed84523a8f99d7947c0bb8b12932018a3081ecc29964605`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a12f83dfb1b48c3152a859b9b55b4483128b0be37e4877271cbd453b23fb43`  
		Last Modified: Tue, 01 Nov 2022 19:02:36 GMT  
		Size: 120.7 MB (120729474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e663873bb0a71689aee0be3ce5f4195e0b573039585fcc3182fe189e8e8fe05`  
		Last Modified: Tue, 01 Nov 2022 19:02:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802d29971118d482599687d5c1f1c069a8f0b8cb0c96e3ec3d5f550416223491`  
		Last Modified: Tue, 01 Nov 2022 19:21:20 GMT  
		Size: 7.1 MB (7052072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eea39f6b8018dc8d0011d05cdf7f2412b1435fdedc607d0087cfb9c631ccc23`  
		Last Modified: Tue, 01 Nov 2022 19:21:19 GMT  
		Size: 1.2 MB (1167444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a34c766fedcef740b10fddb96cd1ffd7aeae2d9628ddfa2510fedd4bbe64d2b`  
		Last Modified: Tue, 01 Nov 2022 19:21:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2-builder` - windows version 10.0.17763.3532; amd64

```console
$ docker pull caddy@sha256:f279c274451500e517aada07ecabddffd03b23f0b9d81791d2347e369b267a6f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2958579667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c57c677f08a022815e25e725365624f628555a00eab2b42f1830e71794c949`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 12:45:06 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Oct 2022 12:45:07 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Oct 2022 12:45:08 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Oct 2022 12:45:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Oct 2022 12:46:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Oct 2022 12:46:38 GMT
ENV GOPATH=C:\go
# Wed, 12 Oct 2022 12:47:37 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 01 Nov 2022 19:19:52 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:25:48 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 01 Nov 2022 19:25:50 GMT
WORKDIR C:\go
# Tue, 01 Nov 2022 20:18:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 01 Nov 2022 20:18:12 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 20:18:13 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 20:18:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 20:19:33 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 01 Nov 2022 20:19:34 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094a4c27e78f8821517fd551cd9e3d5f4b1e4199bdcd783b3fbda849e4995ad1`  
		Last Modified: Wed, 12 Oct 2022 13:16:26 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e91de5ff2103556b1048388473379f95d41247701f0911ebc7c530a861f3f5e`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52642f9e5e3a52bef8ee5677bcb62a364e07003da51f16eb28b8a4ce34fe9f7d`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26528ba698d400f5680be93457d24581b9e4e7a2399de7bb23cbd549f206613`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c89703eb31300a2a39c85ce287a6b9fe88da033828368275bdbb53c2f7704c`  
		Last Modified: Wed, 12 Oct 2022 13:16:30 GMT  
		Size: 25.4 MB (25439927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8705eaae12fa4840be2d79e376eb1b4b7b18da881acad2892b1c47336e796f46`  
		Last Modified: Wed, 12 Oct 2022 13:16:19 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebda8897c2727e3b971c947385632df6f19de06da75e9f161200d43d1acf714`  
		Last Modified: Wed, 12 Oct 2022 13:16:19 GMT  
		Size: 315.0 KB (315035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8667d37dce62bb077cd534d490f047b61dfe9c30023659258862cada9cbd0ba`  
		Last Modified: Tue, 01 Nov 2022 19:54:40 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac8e32e89f1739964a644b8b8b5b44bbae9752f8ea1f87e93455ca36cc86a7d`  
		Last Modified: Tue, 01 Nov 2022 19:55:33 GMT  
		Size: 157.7 MB (157676844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cabbd4ff51bc72ab20efd9f4eb4ebb788679ef03c2fc9b8a72f711fe3558590`  
		Last Modified: Tue, 01 Nov 2022 19:54:40 GMT  
		Size: 1.5 KB (1459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a7aa6766a51e2f5a5add77b40fd7eafa9d3d5049c3b4506b6b4e6dffb65cd6`  
		Last Modified: Tue, 01 Nov 2022 20:21:08 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54feb136a1e02e5d213be9750ca621c39022ff48f54c1e67daace9a82dd241f1`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7c0ce28f0f06a413d72723dbca806a7b025194983d436501cb04b7b2d7379`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e48594ab78eca9cfe42619a2f721de764c027be8fa22700565227c765b4ed7e`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55feb68cd00871cb13079eb862d65521274326d062594c7522edcc8f9bac23f1`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.6 MB (1631634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d398f623f33e057b5d399473e3ee1243fef32140e9a4411c1f69a913b43acb08`  
		Last Modified: Tue, 01 Nov 2022 20:21:05 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2-builder` - windows version 10.0.20348.1129; amd64

```console
$ docker pull caddy@sha256:6e35c0ddda3afe05cb015c908260022b09ae192d81ad72f3bf1e32c70d7cb243
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2659936170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:265570f6cf9dffda304fb3a6712c85940e0f8d23ef6d8ffbfd8e1ebdd6d89d85`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 12:40:52 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Oct 2022 12:40:53 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Oct 2022 12:40:54 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Oct 2022 12:40:55 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Oct 2022 12:41:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Oct 2022 12:41:26 GMT
ENV GOPATH=C:\go
# Wed, 12 Oct 2022 12:41:47 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 01 Nov 2022 19:15:18 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:19:35 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 01 Nov 2022 19:19:38 GMT
WORKDIR C:\go
# Tue, 01 Nov 2022 20:19:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 01 Nov 2022 20:19:43 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 20:19:45 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 20:19:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 20:20:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 01 Nov 2022 20:20:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e9b54b31e104f64c9eb8a65ac0af5effd645bd00a77ea297b6015d28022a74`  
		Last Modified: Mon, 17 Oct 2022 21:39:11 GMT  
		Size: 1000.0 MB (1000028645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f8b589252b90e37349f39b9d4495646791b4050d7cd218336fcc4624b0ebe2`  
		Last Modified: Wed, 12 Oct 2022 13:15:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811ef63d5261b55ee6b499dbc7fcd1ed13386326466fb81a0801abbcbcb75d3f`  
		Last Modified: Wed, 12 Oct 2022 13:15:28 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816740cd643a7a4e72aa527cd033d0c95686c9725ff70dac3260b44dce508e73`  
		Last Modified: Wed, 12 Oct 2022 13:15:28 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599e30c8b316e75d786cfd91f97b9fae4c89fb00f3fce0619eb4e66bc3165521`  
		Last Modified: Wed, 12 Oct 2022 13:15:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77a0d37b81c920d4b783c0b2cfad656a4b8733960ba3afd4e0a1f39f202f948`  
		Last Modified: Wed, 12 Oct 2022 13:15:32 GMT  
		Size: 25.7 MB (25689345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b699f53b56e90279b0bb8ce4434f9b68bbc28fa30756476e22c7ef3dc869e24a`  
		Last Modified: Wed, 12 Oct 2022 13:15:21 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57fcf632f60c89dd981a8a7fa084e738f55129b1786fd9a9e9f5ab8aa1e02d82`  
		Last Modified: Wed, 12 Oct 2022 13:15:24 GMT  
		Size: 526.5 KB (526519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8b0d888223c93af8f0c84ad35156f79df9b0d9ae107f61ded320d2a4fed5f3`  
		Last Modified: Tue, 01 Nov 2022 19:53:29 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49602de12fff655f45d03b1befdd7e56321771c65ed690492e4092da51046bb3`  
		Last Modified: Tue, 01 Nov 2022 19:54:22 GMT  
		Size: 157.8 MB (157838831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cb5ede4eaf1f86f7c0957639a8b53a0c6740df6fa395d3d286e32bff6b9195`  
		Last Modified: Tue, 01 Nov 2022 19:53:29 GMT  
		Size: 1.6 KB (1584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d0ae347408d32205a9ca4c0628e814833984ac8c0fbfb6c6687b9c94a733aa`  
		Last Modified: Tue, 01 Nov 2022 20:21:30 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453489637085324b6412fd9d83cc639d7a9f9135fb5db5dec214462b3293c98f`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cc23fcabe43926f14c7d7e786e9175c87fe573e41fc0158bdc02cfc08fb567`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528f2dc5e38ba5bad570845252c13446ea9637f9c7a80590c93c28886ab79803`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd45b40a0e40f3a52f9a7e2e1cf3cf3b0501ca3f8d637ef46596ee30a9193264`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.8 MB (1837122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bd243dcf25ec803b906e53fa263b2803735773f0227c1c4bac5d52654bb8c6`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.2-builder-alpine`

```console
$ docker pull caddy@sha256:9a51f1a1098ec283efeb9174633447c4bb3142e5bbc7649c8ced7f8d685da3f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.6.2-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:735ad7b9a5ba5baf3df5f93034af5fa90c3554da9725d260df238d2511be6b23
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133519902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4fa387ebb822f454dc9877bfe19aaba627e1b422f476a4952468eb35c419c3f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 21:16:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 21:16:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 21:16:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:20:19 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:21:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:21:57 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:21:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:21:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:21:57 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:49:49 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:49:49 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:49:49 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:49:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:49:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:49:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:49:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4583459ba0371c715f926a9bbd37a9dae909234f4b898220160425131eb53bd4`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 284.7 KB (284734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c1e223e6f2123b855e0c95898eba50cb6a055881ba9023527c0a361761c1cf`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbef1b99e503551b709afdb24ef66954c0792f99d76bb0018afd3a65a1347b5b`  
		Last Modified: Tue, 01 Nov 2022 19:30:19 GMT  
		Size: 122.3 MB (122275572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99825e86aac9391fd3d709522864ff3282479450067b8431df9c4f9e4da4da1`  
		Last Modified: Tue, 01 Nov 2022 19:30:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd6f4fde4a1bb5cc5dd5adba9566a8e0e11ac8cf06adffd9dbefe69a80fc50e`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 6.9 MB (6937644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc2cb786c4d70bac77de2092dd9d3fe5b54e59daa8918ccd6ce64d32929e339`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 1.2 MB (1215184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189da6bcd6c18118e6c5774a9bf9eaba6cde20b87848c17960d265f518beb280`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2b94490e7740d5762996c3f1af82a99c3a298122ab46f5312d75b015ed07fdb3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129501509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:484eab50c7b23327b3246fbfe1577b2cb318df92dd5e1e7695611bc34588a965`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 01 Nov 2022 18:49:34 GMT
RUN apk add --no-cache ca-certificates
# Tue, 01 Nov 2022 18:49:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Nov 2022 18:49:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:49:35 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:51:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:51:57 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:51:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:51:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:51:58 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:18:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:18:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:18:14 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:18:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:18:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:18:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:18:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e34adf14e74afbe714188593430596566b859daec67932063af22ae26cfb41`  
		Last Modified: Tue, 01 Nov 2022 18:59:56 GMT  
		Size: 284.6 KB (284604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30829221241bb1a4c4b78ced30216bd6e772290df6d02b43de82ec13847f2ea`  
		Last Modified: Tue, 01 Nov 2022 18:59:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5175fa50505ed8e1ebb1cc778186a5571aceaf68880fb7f30ce0a002543fde16`  
		Last Modified: Tue, 01 Nov 2022 19:00:18 GMT  
		Size: 118.6 MB (118633129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9462914fb6be31fa7883e2ac24e0b90c77b0dd01eed92e5eb2717d2d58757a21`  
		Last Modified: Tue, 01 Nov 2022 18:59:55 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bae57654f3779f11c3403f04b1e6edc1160b85b75ec1b7aaeebd3ab918fdb3e`  
		Last Modified: Tue, 01 Nov 2022 19:19:10 GMT  
		Size: 6.8 MB (6806143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ccbb51616839b72199c780dc3fb4b40d6337c1b64a8e503b85e43d17ae6bee`  
		Last Modified: Tue, 01 Nov 2022 19:19:09 GMT  
		Size: 1.2 MB (1162983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8bf63e08652d8b6f6f6f0710daa4bfdfd8cd8a9b63599b309be0e046fb2405`  
		Last Modified: Tue, 01 Nov 2022 19:19:09 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:38e0977df61d81ad978adc5aeff5351e967c86e79faa8b7707674d0ac2e63774
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128321867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0724d3115962e959325f2a9a4a8824cd2292a204ddd5db99808f8c1c3b28610a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 03:11:14 GMT
RUN apk add --no-cache ca-certificates
# Thu, 27 Oct 2022 03:11:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 03:11:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:58:35 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:00:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:00:36 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:00:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:00:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:00:37 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:30:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:30:18 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:30:18 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:30:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:30:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:30:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:30:20 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb4eb882dd734293a28e32a55182efac09a590954d1c7e0ac4e9afd668b950f`  
		Last Modified: Thu, 27 Oct 2022 03:23:31 GMT  
		Size: 283.8 KB (283751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62601eba0f2135ba01bd7632b6cd5858fd87c654ebbd7aa446022efda221518`  
		Last Modified: Thu, 27 Oct 2022 03:23:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f8cf932723cb79c6511c7a4565c26fc3c1a8b195b63a1b4f27567664469b8`  
		Last Modified: Tue, 01 Nov 2022 19:11:07 GMT  
		Size: 118.4 MB (118395001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06295a7c5807cf45167f1a47e93084873628c3417ae38bd41c276b71ba1c46ab`  
		Last Modified: Tue, 01 Nov 2022 19:10:45 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92d8ff62b16b450357e75981f8b6277cddab5a79836683195be024c5b466eb1`  
		Last Modified: Tue, 01 Nov 2022 19:31:14 GMT  
		Size: 6.1 MB (6065387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136c853b146e693b550c1d68b6b6713b79d7befffc79acb1530b83593b8fa935`  
		Last Modified: Tue, 01 Nov 2022 19:31:13 GMT  
		Size: 1.2 MB (1159979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f924d6193ccce35a47a6ee295f40e327abf4a8492374030689faf3f505632e08`  
		Last Modified: Tue, 01 Nov 2022 19:31:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6b8569ece82b11e5f6720884af16dce90859af84c6a9ab271ce05a08435fbd77
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127999797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1543ea235e3a8ec3d0ad049bdc81b95745b72848028c6dbc10cde12da0b876fc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 26 Oct 2022 08:09:57 GMT
RUN apk add --no-cache ca-certificates
# Wed, 26 Oct 2022 08:09:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 Oct 2022 08:09:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:40:17 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:41:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:41:34 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:41:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:41:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:41:35 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:05:53 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:05:53 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:05:53 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:05:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:05:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:05:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:05:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d82f9e3411d2eff49049d09ae871e53b96a0cc7dd335883f1fec28c43f9c86`  
		Last Modified: Wed, 26 Oct 2022 08:17:16 GMT  
		Size: 284.7 KB (284723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e169736571560c1a3278f9971532d55ddc4abfaef12e8c54c05f4644445d5520`  
		Last Modified: Wed, 26 Oct 2022 08:17:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc530f9a61e7c0e16b1cb3d48b70136b625cf624976acc638b9d6aef5525995`  
		Last Modified: Tue, 01 Nov 2022 18:48:07 GMT  
		Size: 116.8 MB (116836732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562d55c2123be45d40bfd4dd4dea65161ad3d83b50153de3cc0b63ec7a061f4b`  
		Last Modified: Tue, 01 Nov 2022 18:47:54 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90594629b6df4d09d221ea3fc570b4944e36520a3503ffa3a838772b0e46561`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 7.0 MB (7049481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e41bd715f5f0d05c59b600661a8f0cfb5145de632b14a77d012cfd1ffeea780`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 1.1 MB (1120483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3da6b029e0d694358fe69ed7435eb464495babb3bc51d3d5f30a5222406935`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:0bfdd9fd29aabe5e64b1c692ef01a8064dc2c4932747c3bf06363fd238817630
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128911035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3d666ccc1132e45cb0e54d7fd1891ab309ad3ae1fa96a20556f67f531c4bcc0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:26:01 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:26:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:26:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:17:13 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:19:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:20:03 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:20:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:20:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:20:05 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:50:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:50:46 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:50:46 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:50:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:50:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:50:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:50:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36899d7325c2c25a7d8e61ef33bb1e93b83f811f462e9ddad81c86df87b0685`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 286.7 KB (286747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9309524edda98df2abd6704c6f56004422a28b63364f028763ea000fc32d6eca`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b608654249afe5c44e2b3f100f6b333302506cd24adc46afa3302bb03ff96e`  
		Last Modified: Tue, 01 Nov 2022 19:31:59 GMT  
		Size: 117.2 MB (117238077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93311758f4ff1a16fa50dab5c51c12dd47a1920496e07493f5452c97e24eff9c`  
		Last Modified: Tue, 01 Nov 2022 19:31:32 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce6b57ae4a73b81094351a45358cebcbfbccd4d0d31ab77e71afc97d675dc63`  
		Last Modified: Tue, 01 Nov 2022 19:51:34 GMT  
		Size: 7.5 MB (7478322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5fa9d97b98179c5269f7f488f5488ec1a31fa543c75dc88705c8ed0a755e1c`  
		Last Modified: Tue, 01 Nov 2022 19:51:33 GMT  
		Size: 1.1 MB (1103853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f6efc0777ee24d394842b20cc0fe8c229ae5fecbb8dbb5537e66f5fc1fcf41`  
		Last Modified: Tue, 01 Nov 2022 19:51:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:660f4e58ece536977f580dad53c004e3fe9b1496a0af262adf93a8480746e615
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131825256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d3b89f5e95a2acfe27efc6ab49664e2a25268891a03b26100d1cca071938a79`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:16:09 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:16:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:16:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:43:10 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:46:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:47:10 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:47:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:47:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:47:13 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:20:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:20:25 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:20:26 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:20:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:20:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:20:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:20:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d31ae2e1f77c70a25e9cbeea435b4ab68149a4e17f9d4668768da8dd5ac68a`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 285.0 KB (284954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2788e533105e3c00ed84523a8f99d7947c0bb8b12932018a3081ecc29964605`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a12f83dfb1b48c3152a859b9b55b4483128b0be37e4877271cbd453b23fb43`  
		Last Modified: Tue, 01 Nov 2022 19:02:36 GMT  
		Size: 120.7 MB (120729474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e663873bb0a71689aee0be3ce5f4195e0b573039585fcc3182fe189e8e8fe05`  
		Last Modified: Tue, 01 Nov 2022 19:02:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802d29971118d482599687d5c1f1c069a8f0b8cb0c96e3ec3d5f550416223491`  
		Last Modified: Tue, 01 Nov 2022 19:21:20 GMT  
		Size: 7.1 MB (7052072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eea39f6b8018dc8d0011d05cdf7f2412b1435fdedc607d0087cfb9c631ccc23`  
		Last Modified: Tue, 01 Nov 2022 19:21:19 GMT  
		Size: 1.2 MB (1167444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a34c766fedcef740b10fddb96cd1ffd7aeae2d9628ddfa2510fedd4bbe64d2b`  
		Last Modified: Tue, 01 Nov 2022 19:21:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:ee5b9081fd81e7adbf4a0c1bf8fd4f9f882e755ac9fc03b24f12c7699aa5b52b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `caddy:2.6.2-builder-windowsservercore-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull caddy@sha256:f279c274451500e517aada07ecabddffd03b23f0b9d81791d2347e369b267a6f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2958579667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c57c677f08a022815e25e725365624f628555a00eab2b42f1830e71794c949`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 12:45:06 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Oct 2022 12:45:07 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Oct 2022 12:45:08 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Oct 2022 12:45:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Oct 2022 12:46:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Oct 2022 12:46:38 GMT
ENV GOPATH=C:\go
# Wed, 12 Oct 2022 12:47:37 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 01 Nov 2022 19:19:52 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:25:48 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 01 Nov 2022 19:25:50 GMT
WORKDIR C:\go
# Tue, 01 Nov 2022 20:18:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 01 Nov 2022 20:18:12 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 20:18:13 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 20:18:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 20:19:33 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 01 Nov 2022 20:19:34 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094a4c27e78f8821517fd551cd9e3d5f4b1e4199bdcd783b3fbda849e4995ad1`  
		Last Modified: Wed, 12 Oct 2022 13:16:26 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e91de5ff2103556b1048388473379f95d41247701f0911ebc7c530a861f3f5e`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52642f9e5e3a52bef8ee5677bcb62a364e07003da51f16eb28b8a4ce34fe9f7d`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26528ba698d400f5680be93457d24581b9e4e7a2399de7bb23cbd549f206613`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c89703eb31300a2a39c85ce287a6b9fe88da033828368275bdbb53c2f7704c`  
		Last Modified: Wed, 12 Oct 2022 13:16:30 GMT  
		Size: 25.4 MB (25439927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8705eaae12fa4840be2d79e376eb1b4b7b18da881acad2892b1c47336e796f46`  
		Last Modified: Wed, 12 Oct 2022 13:16:19 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebda8897c2727e3b971c947385632df6f19de06da75e9f161200d43d1acf714`  
		Last Modified: Wed, 12 Oct 2022 13:16:19 GMT  
		Size: 315.0 KB (315035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8667d37dce62bb077cd534d490f047b61dfe9c30023659258862cada9cbd0ba`  
		Last Modified: Tue, 01 Nov 2022 19:54:40 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac8e32e89f1739964a644b8b8b5b44bbae9752f8ea1f87e93455ca36cc86a7d`  
		Last Modified: Tue, 01 Nov 2022 19:55:33 GMT  
		Size: 157.7 MB (157676844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cabbd4ff51bc72ab20efd9f4eb4ebb788679ef03c2fc9b8a72f711fe3558590`  
		Last Modified: Tue, 01 Nov 2022 19:54:40 GMT  
		Size: 1.5 KB (1459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a7aa6766a51e2f5a5add77b40fd7eafa9d3d5049c3b4506b6b4e6dffb65cd6`  
		Last Modified: Tue, 01 Nov 2022 20:21:08 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54feb136a1e02e5d213be9750ca621c39022ff48f54c1e67daace9a82dd241f1`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7c0ce28f0f06a413d72723dbca806a7b025194983d436501cb04b7b2d7379`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e48594ab78eca9cfe42619a2f721de764c027be8fa22700565227c765b4ed7e`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55feb68cd00871cb13079eb862d65521274326d062594c7522edcc8f9bac23f1`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.6 MB (1631634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d398f623f33e057b5d399473e3ee1243fef32140e9a4411c1f69a913b43acb08`  
		Last Modified: Tue, 01 Nov 2022 20:21:05 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:39520901129debe71fc3b671250e73c438c85ee3435b24c8c8c5bc6293f05800
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1129; amd64

### `caddy:2.6.2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1129; amd64

```console
$ docker pull caddy@sha256:6e35c0ddda3afe05cb015c908260022b09ae192d81ad72f3bf1e32c70d7cb243
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2659936170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:265570f6cf9dffda304fb3a6712c85940e0f8d23ef6d8ffbfd8e1ebdd6d89d85`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 12:40:52 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Oct 2022 12:40:53 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Oct 2022 12:40:54 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Oct 2022 12:40:55 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Oct 2022 12:41:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Oct 2022 12:41:26 GMT
ENV GOPATH=C:\go
# Wed, 12 Oct 2022 12:41:47 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 01 Nov 2022 19:15:18 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:19:35 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 01 Nov 2022 19:19:38 GMT
WORKDIR C:\go
# Tue, 01 Nov 2022 20:19:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 01 Nov 2022 20:19:43 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 20:19:45 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 20:19:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 20:20:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 01 Nov 2022 20:20:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e9b54b31e104f64c9eb8a65ac0af5effd645bd00a77ea297b6015d28022a74`  
		Last Modified: Mon, 17 Oct 2022 21:39:11 GMT  
		Size: 1000.0 MB (1000028645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f8b589252b90e37349f39b9d4495646791b4050d7cd218336fcc4624b0ebe2`  
		Last Modified: Wed, 12 Oct 2022 13:15:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811ef63d5261b55ee6b499dbc7fcd1ed13386326466fb81a0801abbcbcb75d3f`  
		Last Modified: Wed, 12 Oct 2022 13:15:28 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816740cd643a7a4e72aa527cd033d0c95686c9725ff70dac3260b44dce508e73`  
		Last Modified: Wed, 12 Oct 2022 13:15:28 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599e30c8b316e75d786cfd91f97b9fae4c89fb00f3fce0619eb4e66bc3165521`  
		Last Modified: Wed, 12 Oct 2022 13:15:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77a0d37b81c920d4b783c0b2cfad656a4b8733960ba3afd4e0a1f39f202f948`  
		Last Modified: Wed, 12 Oct 2022 13:15:32 GMT  
		Size: 25.7 MB (25689345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b699f53b56e90279b0bb8ce4434f9b68bbc28fa30756476e22c7ef3dc869e24a`  
		Last Modified: Wed, 12 Oct 2022 13:15:21 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57fcf632f60c89dd981a8a7fa084e738f55129b1786fd9a9e9f5ab8aa1e02d82`  
		Last Modified: Wed, 12 Oct 2022 13:15:24 GMT  
		Size: 526.5 KB (526519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8b0d888223c93af8f0c84ad35156f79df9b0d9ae107f61ded320d2a4fed5f3`  
		Last Modified: Tue, 01 Nov 2022 19:53:29 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49602de12fff655f45d03b1befdd7e56321771c65ed690492e4092da51046bb3`  
		Last Modified: Tue, 01 Nov 2022 19:54:22 GMT  
		Size: 157.8 MB (157838831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cb5ede4eaf1f86f7c0957639a8b53a0c6740df6fa395d3d286e32bff6b9195`  
		Last Modified: Tue, 01 Nov 2022 19:53:29 GMT  
		Size: 1.6 KB (1584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d0ae347408d32205a9ca4c0628e814833984ac8c0fbfb6c6687b9c94a733aa`  
		Last Modified: Tue, 01 Nov 2022 20:21:30 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453489637085324b6412fd9d83cc639d7a9f9135fb5db5dec214462b3293c98f`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cc23fcabe43926f14c7d7e786e9175c87fe573e41fc0158bdc02cfc08fb567`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528f2dc5e38ba5bad570845252c13446ea9637f9c7a80590c93c28886ab79803`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd45b40a0e40f3a52f9a7e2e1cf3cf3b0501ca3f8d637ef46596ee30a9193264`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.8 MB (1837122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bd243dcf25ec803b906e53fa263b2803735773f0227c1c4bac5d52654bb8c6`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.2-windowsservercore`

```console
$ docker pull caddy@sha256:a2ab9b4da81fb5793c09308f6353dec3d5aa70255288aa5a9390cf5333e74935
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3532; amd64
	-	windows version 10.0.20348.1129; amd64

### `caddy:2.6.2-windowsservercore` - windows version 10.0.17763.3532; amd64

```console
$ docker pull caddy@sha256:c795b26fccceaa3ea3738c3d086e0c9da9978392aeb6e2c69ae3d71131b88998
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726785951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a0ffc50daa8e99f5d3029bd930601ec939b66a180da1ad5fef783d1fcb69eb3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 16:58:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:14:49 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:16:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:16:10 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:16:11 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:16:12 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:16:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:16:14 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:16:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:16:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:16:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:16:19 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:16:20 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:16:21 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:16:22 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:17:16 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:17:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:028c482fad0f111537a40f65401f65de54c9fd682951a4f8cf9b644d7c128e18`  
		Size: 834.0 MB (833997855 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77462c8fbd8b2782ee2fc5f09bebfb350912f754186b058478ab8d22f50bb047`  
		Last Modified: Wed, 12 Oct 2022 17:04:34 GMT  
		Size: 358.2 KB (358248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a372be4d9f43d4d5884bc4093c44aedf12150f55ea9457baa2fcceb43ef8074`  
		Last Modified: Thu, 13 Oct 2022 23:21:08 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a8993c29bb6d4c31b0be3609bc7fb2af2666435fe70bb2f329784277d629d1`  
		Last Modified: Thu, 13 Oct 2022 23:21:11 GMT  
		Size: 14.9 MB (14947938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98662b730099437011356fa77ef9072054f4ad73d3781e9b02d4750689762162`  
		Last Modified: Thu, 13 Oct 2022 23:21:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7e77f6a080ad6fa8a7320831868ccd7b6385e995988f2e6cca76090a565c99`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec71d29d036cab0bdbc7765216513aad527933ededfec4492a97724c6bab52d`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a11bac4631094c366303dd3c571fe04cf1b543bafba72d8dd1030f8ae2ec185`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4dc588cdabd0672f8b29c59cd9ddc6d927160284a6f6529fbe39b8e34ca766`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f39777f21d48153f681f16b5a1cd2e12440066bc96a665fa3b85a6275b74942`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638736df2ba6ceaed21b97ee12046d2d0494561bd735581618ab505ff602b0da`  
		Last Modified: Thu, 13 Oct 2022 23:21:04 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e0fe53dba785fdf61d7431392d7e15beeebbe5f215d9a2de2ee00975e7b5c4`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb7b8fc42485b0656b2afcb99344cda044ce10d0107cc91955fbe11433c358`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb8f166931be4f8f0b0a07611df01a8e7d1101f8a8ce564144ded43917e1021`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bc6f4b7a114b7722cfc81aa83b74727261766c2cef9bc0787e447435c33d2a`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5563ab3963680a40da3bc2269bbc1e76362b359547dae9705892cf8f54b50dd1`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d300f0320cd2b8ce3f3e58cbb3acb06e24c5f59a342725056a10667329f914`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfb9dfa0b00914a255876439613219f4a74e83734df6b8a197e6e0bb53bf905`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b9233dbf203ca77eea2271813856d219ba7d2f633adf99f3262612edfad738`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 291.8 KB (291836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefde31b509f056641749adae4daa4e0ad3265d260ac1c61b41c8950a10824e6`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2-windowsservercore` - windows version 10.0.20348.1129; amd64

```console
$ docker pull caddy@sha256:e1e15c80e157d71221ec43035cae93b3ea8ba7a6b203428e93159aa6ff5e1463
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2432333411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbd806ca24dfacee0d098f111cc9f6d5f42fdbd9db91a63a8de0d048d3984d5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 17:01:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:17:37 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:18:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:18:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:18:13 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:18:13 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:18:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:18:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:18:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:18:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:18:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:18:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:18:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:18:21 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:18:22 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:18:23 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:18:24 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:18:40 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:18:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ab91661ce2a2a2c14684a2ba0f543a81d7896773f88200b31be0e37c589de38`  
		Size: 979.4 MB (979359717 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cd84a277fd91a008fe0c8fc7d6706544075a294512940b16f57998588ea892`  
		Last Modified: Wed, 12 Oct 2022 17:04:58 GMT  
		Size: 616.9 KB (616893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b069dfbedeca0437916f85fdd78a598955839b91ffc4cba4d6327e5c79487`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5263d846656ffa3662062b1a58d9c6d114e00fa5344edc9b93ea5895c4fa46`  
		Last Modified: Thu, 13 Oct 2022 23:21:34 GMT  
		Size: 15.1 MB (15149356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e378404d94c7fb280c51201d60aef05af3196a0ead3b716521cedbe766ba5e3e`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11749bcf2c3e4097f9a1a30d1fc22184e48c94ab54945730c51c36be175c668d`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cb14f39fa0dce5d6dab4bdd1a896c02b5a6bba01dcd46ed36928c2cce27295`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf622a21cfc36d8958be2f273f52b7d4824d500be08f6a2de791506dcc6c981f`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b246af35953d05f1c4292cb1cf8cfc29215ceac2e013ae2a0759aa2d216516`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08367cd2562c20737156e692dca481f835f4832fabb63602fb5edc78494057ae`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6d70510bf329eff739580f04b59acba9cb4aa74e57bcb6fca996d6df6b6d2c`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc6e963fa5949ceb99519a652299dea21a92c9389aadabedb2deeb4e51855b5`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d175d8244325a62c683c4d1fa6cc266f73231f93142fd0f52c3378da6db1464`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4ce9495075c9b00994ef154c9eb0974ba1853a8244869e35af4eecfca4dce7`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceee07aab1c573de692984f7655da9e6c4aee31260b8df8735344242e6f1ff8`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295041dd24e85177aaf7e1bbd1c0b032d2eafaf3da59213972894238dd5b3d72`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3583f031f13dfd9a933b6e8d4808a3ac7f3e007d2e751af9581b76b08b6e0c4a`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1603973d06c7b0a01ab165d727b40f842361ce898a8e7b8579d6bd9db938c8a6`  
		Last Modified: Thu, 13 Oct 2022 23:21:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c4bf5f410b0a58ef5b477fdf99b90ad01e7deb85b685cf06eaae5c9d83a531`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 319.8 KB (319842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da4c854489e4317220200f8dca47e2335696fe8fa9e7a2aa678467b12b4db7b`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:750ce937e1a109f41cc11cad93540eeb4b7ab051847137267847c104941dfe75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `caddy:2.6.2-windowsservercore-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull caddy@sha256:c795b26fccceaa3ea3738c3d086e0c9da9978392aeb6e2c69ae3d71131b88998
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726785951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a0ffc50daa8e99f5d3029bd930601ec939b66a180da1ad5fef783d1fcb69eb3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 16:58:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:14:49 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:16:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:16:10 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:16:11 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:16:12 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:16:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:16:14 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:16:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:16:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:16:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:16:19 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:16:20 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:16:21 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:16:22 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:17:16 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:17:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:028c482fad0f111537a40f65401f65de54c9fd682951a4f8cf9b644d7c128e18`  
		Size: 834.0 MB (833997855 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77462c8fbd8b2782ee2fc5f09bebfb350912f754186b058478ab8d22f50bb047`  
		Last Modified: Wed, 12 Oct 2022 17:04:34 GMT  
		Size: 358.2 KB (358248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a372be4d9f43d4d5884bc4093c44aedf12150f55ea9457baa2fcceb43ef8074`  
		Last Modified: Thu, 13 Oct 2022 23:21:08 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a8993c29bb6d4c31b0be3609bc7fb2af2666435fe70bb2f329784277d629d1`  
		Last Modified: Thu, 13 Oct 2022 23:21:11 GMT  
		Size: 14.9 MB (14947938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98662b730099437011356fa77ef9072054f4ad73d3781e9b02d4750689762162`  
		Last Modified: Thu, 13 Oct 2022 23:21:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7e77f6a080ad6fa8a7320831868ccd7b6385e995988f2e6cca76090a565c99`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec71d29d036cab0bdbc7765216513aad527933ededfec4492a97724c6bab52d`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a11bac4631094c366303dd3c571fe04cf1b543bafba72d8dd1030f8ae2ec185`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4dc588cdabd0672f8b29c59cd9ddc6d927160284a6f6529fbe39b8e34ca766`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f39777f21d48153f681f16b5a1cd2e12440066bc96a665fa3b85a6275b74942`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638736df2ba6ceaed21b97ee12046d2d0494561bd735581618ab505ff602b0da`  
		Last Modified: Thu, 13 Oct 2022 23:21:04 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e0fe53dba785fdf61d7431392d7e15beeebbe5f215d9a2de2ee00975e7b5c4`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb7b8fc42485b0656b2afcb99344cda044ce10d0107cc91955fbe11433c358`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb8f166931be4f8f0b0a07611df01a8e7d1101f8a8ce564144ded43917e1021`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bc6f4b7a114b7722cfc81aa83b74727261766c2cef9bc0787e447435c33d2a`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5563ab3963680a40da3bc2269bbc1e76362b359547dae9705892cf8f54b50dd1`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d300f0320cd2b8ce3f3e58cbb3acb06e24c5f59a342725056a10667329f914`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfb9dfa0b00914a255876439613219f4a74e83734df6b8a197e6e0bb53bf905`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b9233dbf203ca77eea2271813856d219ba7d2f633adf99f3262612edfad738`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 291.8 KB (291836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefde31b509f056641749adae4daa4e0ad3265d260ac1c61b41c8950a10824e6`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:6a6b89102bf9584016d1a0364792d3cea05585c2fc057b4ffce271b8496a8bc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1129; amd64

### `caddy:2.6.2-windowsservercore-ltsc2022` - windows version 10.0.20348.1129; amd64

```console
$ docker pull caddy@sha256:e1e15c80e157d71221ec43035cae93b3ea8ba7a6b203428e93159aa6ff5e1463
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2432333411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbd806ca24dfacee0d098f111cc9f6d5f42fdbd9db91a63a8de0d048d3984d5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 17:01:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:17:37 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:18:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:18:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:18:13 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:18:13 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:18:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:18:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:18:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:18:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:18:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:18:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:18:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:18:21 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:18:22 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:18:23 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:18:24 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:18:40 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:18:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ab91661ce2a2a2c14684a2ba0f543a81d7896773f88200b31be0e37c589de38`  
		Size: 979.4 MB (979359717 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cd84a277fd91a008fe0c8fc7d6706544075a294512940b16f57998588ea892`  
		Last Modified: Wed, 12 Oct 2022 17:04:58 GMT  
		Size: 616.9 KB (616893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b069dfbedeca0437916f85fdd78a598955839b91ffc4cba4d6327e5c79487`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5263d846656ffa3662062b1a58d9c6d114e00fa5344edc9b93ea5895c4fa46`  
		Last Modified: Thu, 13 Oct 2022 23:21:34 GMT  
		Size: 15.1 MB (15149356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e378404d94c7fb280c51201d60aef05af3196a0ead3b716521cedbe766ba5e3e`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11749bcf2c3e4097f9a1a30d1fc22184e48c94ab54945730c51c36be175c668d`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cb14f39fa0dce5d6dab4bdd1a896c02b5a6bba01dcd46ed36928c2cce27295`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf622a21cfc36d8958be2f273f52b7d4824d500be08f6a2de791506dcc6c981f`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b246af35953d05f1c4292cb1cf8cfc29215ceac2e013ae2a0759aa2d216516`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08367cd2562c20737156e692dca481f835f4832fabb63602fb5edc78494057ae`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6d70510bf329eff739580f04b59acba9cb4aa74e57bcb6fca996d6df6b6d2c`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc6e963fa5949ceb99519a652299dea21a92c9389aadabedb2deeb4e51855b5`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d175d8244325a62c683c4d1fa6cc266f73231f93142fd0f52c3378da6db1464`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4ce9495075c9b00994ef154c9eb0974ba1853a8244869e35af4eecfca4dce7`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceee07aab1c573de692984f7655da9e6c4aee31260b8df8735344242e6f1ff8`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295041dd24e85177aaf7e1bbd1c0b032d2eafaf3da59213972894238dd5b3d72`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3583f031f13dfd9a933b6e8d4808a3ac7f3e007d2e751af9581b76b08b6e0c4a`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1603973d06c7b0a01ab165d727b40f842361ce898a8e7b8579d6bd9db938c8a6`  
		Last Modified: Thu, 13 Oct 2022 23:21:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c4bf5f410b0a58ef5b477fdf99b90ad01e7deb85b685cf06eaae5c9d83a531`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 319.8 KB (319842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da4c854489e4317220200f8dca47e2335696fe8fa9e7a2aa678467b12b4db7b`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:0e3c6d476eb251d2e271c61d12472698e2be1909626d342c405ed58c70772857
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
$ docker pull caddy@sha256:7992b931b7da3cf0840dd69ea74b2c67d423faf03408da8abdc31b7590a239a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17676993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:006d393a4e6a01f82413e41b3e0f06dfb1872d5ca6a37aba315e4ec9e2cc6c4c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:34:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 04:34:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 01:43:19 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 01:43:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 01:43:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 01:43:22 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 01:43:22 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 01:43:22 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 01:43:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 80
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 443
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 01:43:24 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 01:43:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5625668cf98fd3e4d769f18d45f27e34fe3d085cfb9927ff7ad2cdc84d8c493f`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 304.5 KB (304517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675d09b34c5347b62625d31b2a458824240b90e51d18bcc38ad37d317e83d64c`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1747be7065842ba85f86aed65e75608dfd2f546ab9d8ecd4a8842c8f4634795`  
		Last Modified: Fri, 14 Oct 2022 01:43:47 GMT  
		Size: 14.6 MB (14560435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8ee6c4c21d12cd28fcd0e196acb8569f35518dc36c691c91b4c8ca1928bf9d`  
		Last Modified: Fri, 14 Oct 2022 01:43:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:76b70e0dc74358fc1f7ef178c46cc9c047a90cd05e842d26305da1ee04ff3ad8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16834877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cac02415934eaae38be5b122f6a0c760f747e6f50f1551c9a45f4f186454f04`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 19:49:23 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 27 Oct 2022 19:49:25 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 27 Oct 2022 19:49:25 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 27 Oct 2022 19:49:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 27 Oct 2022 19:49:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 19:49:28 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 27 Oct 2022 19:49:28 GMT
ENV XDG_DATA_HOME=/data
# Thu, 27 Oct 2022 19:49:28 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 27 Oct 2022 19:49:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 80
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 443
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 443/udp
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 2019
# Thu, 27 Oct 2022 19:49:30 GMT
WORKDIR /srv
# Thu, 27 Oct 2022 19:49:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7f6197b1f089356a6bff8bf29fdcef692051048bd17db70d72df822c89c04d`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 304.4 KB (304404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc91cb09da181c7973089ccf7aca9c7830c738ac1e614883f86c2eecdcb68002`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 5.8 KB (5751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ffb96b75d9dc6019cfe6202b9fed588b3ff9a91cc89237d6a24c98eb5fd590`  
		Last Modified: Thu, 27 Oct 2022 19:50:36 GMT  
		Size: 13.9 MB (13910603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb4866598fa794379095b277b41d4b0cb626d61cc20c6f6cff7d920bc99330`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9df5bfbadaf5495675c4de47918d3631d439d159681e352069eaa206f664a8ac
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16617541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d61e1121278866d5afee597ba2ac37a9b5bec51b6323b551fe9a89b5d99d63e5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 10:30:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 27 Oct 2022 10:30:41 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 27 Oct 2022 10:30:41 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 27 Oct 2022 10:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 27 Oct 2022 10:30:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 10:30:45 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 27 Oct 2022 10:30:45 GMT
ENV XDG_DATA_HOME=/data
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 27 Oct 2022 10:30:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 80
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 443
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 443/udp
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 2019
# Thu, 27 Oct 2022 10:30:46 GMT
WORKDIR /srv
# Thu, 27 Oct 2022 10:30:46 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9f1011ebc9810d3e61468e7ce6c2866fc65920db06e3bccde2da749f976500`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 303.5 KB (303537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28310071f60503f30048b0cad1abe85c763c57dd4e69715cc57d60560481318`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 5.8 KB (5753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7792abbee8ad8ec28f7e6e2864a9e8ad229de5f701ba4bf04be77cffac8835ac`  
		Last Modified: Thu, 27 Oct 2022 10:31:39 GMT  
		Size: 13.9 MB (13891032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c5be986b3fadf5f34a0a4311ffa6a22b4f1f0ff79c510fb7c58cb93c64e2f3`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f06fb46d2c67f3b7f9447b6c19f5b9909931b603d2b475f647624f577c6d94ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16278669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8876f25c7ec7330d6bf197e452e3a37deeea42e52b8c2b2c9103bc86b26795`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 26 Oct 2022 18:53:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 Oct 2022 18:53:58 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Wed, 26 Oct 2022 18:53:58 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 26 Oct 2022 18:54:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 Oct 2022 18:54:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 Oct 2022 18:54:01 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 Oct 2022 18:54:01 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 80
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 443
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 443/udp
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 2019
# Wed, 26 Oct 2022 18:54:02 GMT
WORKDIR /srv
# Wed, 26 Oct 2022 18:54:02 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5532e6e746eecf0e890ee17251a52841dd55694ae55c919dc6ddf6159e27cd5b`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 304.5 KB (304512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b816658ad2f9debd81f6df21dd733e54fc6eda530080cc3957e6f63d9677b9a`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d7ee92d83c49ca71b5440fd76d22ac6b75304bc48a0183bf392689ae8d5897`  
		Last Modified: Wed, 26 Oct 2022 18:54:26 GMT  
		Size: 13.3 MB (13260508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00da94c60a7ed1fc9acd392aedea2ab7b2bd6a7d67cc83b2d5d85c5cbd40090b`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:9665c6fd33be967b3bdfcdbeeb605e3a92e70080ef5caa8907a6cbdef064be3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (16031232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96553401995800bf37590502c237b4ab8cee57bd3885e83f76dcb42c53a7d7db`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:56:10 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 07:56:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 03:47:38 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 03:47:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 03:47:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 03:47:44 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 03:47:44 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 03:47:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 03:47:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 80
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 443
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 03:47:49 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 03:47:49 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 03:47:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf49ba2a5c90a152d4aef09519c7019835fbf2884d6afb1c85b3353b7d91388e`  
		Last Modified: Fri, 07 Oct 2022 07:57:09 GMT  
		Size: 306.5 KB (306522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dac87aba8912de3ce6fb3ca14bb6833f931fd15d7ec2d7435a18f11e5ddb6fb`  
		Last Modified: Fri, 07 Oct 2022 07:57:08 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea24f9a44c53fbd359328daff2e10e4e3f1c7d7bae21190ea2f6af3be43dd0b`  
		Last Modified: Fri, 14 Oct 2022 03:48:33 GMT  
		Size: 12.9 MB (12915404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4704e2ddccf987da9605ef1c8d4ef68a86cf3e6ba2f8c5d1e80e5915481e25c`  
		Last Modified: Fri, 14 Oct 2022 03:48:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:5702e27172b1bfb5e9930d544d7cf16a83f774419b1aa2078be464351ff5f70b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16967685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05ec4a186bcadcf0e691a443c7edebf42d46cff3997d01a56de43db0ecbab8e2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 10:23:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 10:23:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 00:55:05 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 00:55:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 00:55:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 00:55:15 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 00:55:16 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 00:55:17 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 00:55:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 00:55:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 00:55:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 00:55:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 00:55:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 00:55:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 00:55:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 00:55:22 GMT
EXPOSE 80
# Fri, 14 Oct 2022 00:55:22 GMT
EXPOSE 443
# Fri, 14 Oct 2022 00:55:23 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 00:55:23 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 00:55:24 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 00:55:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5123e0e5a47a6dfbd8cae1e2589df59b198f82ba790c211aeb3eefbbe41a17be`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 304.8 KB (304752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557f08048878eca2f16fd3b05bb138300739b9e74e467509792efc4278e74b3f`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91158060b74650f434cb3419f6ed862b0616480567b651bfae73b297f69b9992`  
		Last Modified: Fri, 14 Oct 2022 00:56:22 GMT  
		Size: 14.1 MB (14066352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511ac9f174e3fed802157937e9192a940800d73835958de90f5a363b5edf46ad`  
		Last Modified: Fri, 14 Oct 2022 00:56:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:9a395d60c9cba0036b919495f7637be3fafb0a97459ee970f1738e0252dfa2f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3532; amd64
	-	windows version 10.0.20348.1129; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:735ad7b9a5ba5baf3df5f93034af5fa90c3554da9725d260df238d2511be6b23
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133519902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4fa387ebb822f454dc9877bfe19aaba627e1b422f476a4952468eb35c419c3f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 21:16:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 21:16:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 21:16:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:20:19 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:21:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:21:57 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:21:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:21:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:21:57 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:49:49 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:49:49 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:49:49 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:49:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:49:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:49:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:49:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4583459ba0371c715f926a9bbd37a9dae909234f4b898220160425131eb53bd4`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 284.7 KB (284734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c1e223e6f2123b855e0c95898eba50cb6a055881ba9023527c0a361761c1cf`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbef1b99e503551b709afdb24ef66954c0792f99d76bb0018afd3a65a1347b5b`  
		Last Modified: Tue, 01 Nov 2022 19:30:19 GMT  
		Size: 122.3 MB (122275572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99825e86aac9391fd3d709522864ff3282479450067b8431df9c4f9e4da4da1`  
		Last Modified: Tue, 01 Nov 2022 19:30:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd6f4fde4a1bb5cc5dd5adba9566a8e0e11ac8cf06adffd9dbefe69a80fc50e`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 6.9 MB (6937644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc2cb786c4d70bac77de2092dd9d3fe5b54e59daa8918ccd6ce64d32929e339`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 1.2 MB (1215184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189da6bcd6c18118e6c5774a9bf9eaba6cde20b87848c17960d265f518beb280`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2b94490e7740d5762996c3f1af82a99c3a298122ab46f5312d75b015ed07fdb3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129501509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:484eab50c7b23327b3246fbfe1577b2cb318df92dd5e1e7695611bc34588a965`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 01 Nov 2022 18:49:34 GMT
RUN apk add --no-cache ca-certificates
# Tue, 01 Nov 2022 18:49:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Nov 2022 18:49:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:49:35 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:51:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:51:57 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:51:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:51:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:51:58 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:18:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:18:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:18:14 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:18:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:18:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:18:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:18:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e34adf14e74afbe714188593430596566b859daec67932063af22ae26cfb41`  
		Last Modified: Tue, 01 Nov 2022 18:59:56 GMT  
		Size: 284.6 KB (284604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30829221241bb1a4c4b78ced30216bd6e772290df6d02b43de82ec13847f2ea`  
		Last Modified: Tue, 01 Nov 2022 18:59:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5175fa50505ed8e1ebb1cc778186a5571aceaf68880fb7f30ce0a002543fde16`  
		Last Modified: Tue, 01 Nov 2022 19:00:18 GMT  
		Size: 118.6 MB (118633129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9462914fb6be31fa7883e2ac24e0b90c77b0dd01eed92e5eb2717d2d58757a21`  
		Last Modified: Tue, 01 Nov 2022 18:59:55 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bae57654f3779f11c3403f04b1e6edc1160b85b75ec1b7aaeebd3ab918fdb3e`  
		Last Modified: Tue, 01 Nov 2022 19:19:10 GMT  
		Size: 6.8 MB (6806143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ccbb51616839b72199c780dc3fb4b40d6337c1b64a8e503b85e43d17ae6bee`  
		Last Modified: Tue, 01 Nov 2022 19:19:09 GMT  
		Size: 1.2 MB (1162983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8bf63e08652d8b6f6f6f0710daa4bfdfd8cd8a9b63599b309be0e046fb2405`  
		Last Modified: Tue, 01 Nov 2022 19:19:09 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:38e0977df61d81ad978adc5aeff5351e967c86e79faa8b7707674d0ac2e63774
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128321867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0724d3115962e959325f2a9a4a8824cd2292a204ddd5db99808f8c1c3b28610a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 03:11:14 GMT
RUN apk add --no-cache ca-certificates
# Thu, 27 Oct 2022 03:11:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 03:11:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:58:35 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:00:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:00:36 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:00:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:00:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:00:37 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:30:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:30:18 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:30:18 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:30:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:30:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:30:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:30:20 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb4eb882dd734293a28e32a55182efac09a590954d1c7e0ac4e9afd668b950f`  
		Last Modified: Thu, 27 Oct 2022 03:23:31 GMT  
		Size: 283.8 KB (283751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62601eba0f2135ba01bd7632b6cd5858fd87c654ebbd7aa446022efda221518`  
		Last Modified: Thu, 27 Oct 2022 03:23:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f8cf932723cb79c6511c7a4565c26fc3c1a8b195b63a1b4f27567664469b8`  
		Last Modified: Tue, 01 Nov 2022 19:11:07 GMT  
		Size: 118.4 MB (118395001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06295a7c5807cf45167f1a47e93084873628c3417ae38bd41c276b71ba1c46ab`  
		Last Modified: Tue, 01 Nov 2022 19:10:45 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92d8ff62b16b450357e75981f8b6277cddab5a79836683195be024c5b466eb1`  
		Last Modified: Tue, 01 Nov 2022 19:31:14 GMT  
		Size: 6.1 MB (6065387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136c853b146e693b550c1d68b6b6713b79d7befffc79acb1530b83593b8fa935`  
		Last Modified: Tue, 01 Nov 2022 19:31:13 GMT  
		Size: 1.2 MB (1159979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f924d6193ccce35a47a6ee295f40e327abf4a8492374030689faf3f505632e08`  
		Last Modified: Tue, 01 Nov 2022 19:31:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6b8569ece82b11e5f6720884af16dce90859af84c6a9ab271ce05a08435fbd77
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127999797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1543ea235e3a8ec3d0ad049bdc81b95745b72848028c6dbc10cde12da0b876fc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 26 Oct 2022 08:09:57 GMT
RUN apk add --no-cache ca-certificates
# Wed, 26 Oct 2022 08:09:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 Oct 2022 08:09:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:40:17 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:41:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:41:34 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:41:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:41:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:41:35 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:05:53 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:05:53 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:05:53 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:05:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:05:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:05:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:05:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d82f9e3411d2eff49049d09ae871e53b96a0cc7dd335883f1fec28c43f9c86`  
		Last Modified: Wed, 26 Oct 2022 08:17:16 GMT  
		Size: 284.7 KB (284723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e169736571560c1a3278f9971532d55ddc4abfaef12e8c54c05f4644445d5520`  
		Last Modified: Wed, 26 Oct 2022 08:17:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc530f9a61e7c0e16b1cb3d48b70136b625cf624976acc638b9d6aef5525995`  
		Last Modified: Tue, 01 Nov 2022 18:48:07 GMT  
		Size: 116.8 MB (116836732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562d55c2123be45d40bfd4dd4dea65161ad3d83b50153de3cc0b63ec7a061f4b`  
		Last Modified: Tue, 01 Nov 2022 18:47:54 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90594629b6df4d09d221ea3fc570b4944e36520a3503ffa3a838772b0e46561`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 7.0 MB (7049481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e41bd715f5f0d05c59b600661a8f0cfb5145de632b14a77d012cfd1ffeea780`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 1.1 MB (1120483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3da6b029e0d694358fe69ed7435eb464495babb3bc51d3d5f30a5222406935`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:0bfdd9fd29aabe5e64b1c692ef01a8064dc2c4932747c3bf06363fd238817630
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128911035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3d666ccc1132e45cb0e54d7fd1891ab309ad3ae1fa96a20556f67f531c4bcc0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:26:01 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:26:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:26:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:17:13 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:19:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:20:03 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:20:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:20:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:20:05 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:50:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:50:46 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:50:46 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:50:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:50:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:50:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:50:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36899d7325c2c25a7d8e61ef33bb1e93b83f811f462e9ddad81c86df87b0685`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 286.7 KB (286747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9309524edda98df2abd6704c6f56004422a28b63364f028763ea000fc32d6eca`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b608654249afe5c44e2b3f100f6b333302506cd24adc46afa3302bb03ff96e`  
		Last Modified: Tue, 01 Nov 2022 19:31:59 GMT  
		Size: 117.2 MB (117238077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93311758f4ff1a16fa50dab5c51c12dd47a1920496e07493f5452c97e24eff9c`  
		Last Modified: Tue, 01 Nov 2022 19:31:32 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce6b57ae4a73b81094351a45358cebcbfbccd4d0d31ab77e71afc97d675dc63`  
		Last Modified: Tue, 01 Nov 2022 19:51:34 GMT  
		Size: 7.5 MB (7478322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5fa9d97b98179c5269f7f488f5488ec1a31fa543c75dc88705c8ed0a755e1c`  
		Last Modified: Tue, 01 Nov 2022 19:51:33 GMT  
		Size: 1.1 MB (1103853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f6efc0777ee24d394842b20cc0fe8c229ae5fecbb8dbb5537e66f5fc1fcf41`  
		Last Modified: Tue, 01 Nov 2022 19:51:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:660f4e58ece536977f580dad53c004e3fe9b1496a0af262adf93a8480746e615
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131825256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d3b89f5e95a2acfe27efc6ab49664e2a25268891a03b26100d1cca071938a79`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:16:09 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:16:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:16:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:43:10 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:46:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:47:10 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:47:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:47:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:47:13 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:20:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:20:25 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:20:26 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:20:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:20:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:20:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:20:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d31ae2e1f77c70a25e9cbeea435b4ab68149a4e17f9d4668768da8dd5ac68a`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 285.0 KB (284954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2788e533105e3c00ed84523a8f99d7947c0bb8b12932018a3081ecc29964605`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a12f83dfb1b48c3152a859b9b55b4483128b0be37e4877271cbd453b23fb43`  
		Last Modified: Tue, 01 Nov 2022 19:02:36 GMT  
		Size: 120.7 MB (120729474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e663873bb0a71689aee0be3ce5f4195e0b573039585fcc3182fe189e8e8fe05`  
		Last Modified: Tue, 01 Nov 2022 19:02:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802d29971118d482599687d5c1f1c069a8f0b8cb0c96e3ec3d5f550416223491`  
		Last Modified: Tue, 01 Nov 2022 19:21:20 GMT  
		Size: 7.1 MB (7052072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eea39f6b8018dc8d0011d05cdf7f2412b1435fdedc607d0087cfb9c631ccc23`  
		Last Modified: Tue, 01 Nov 2022 19:21:19 GMT  
		Size: 1.2 MB (1167444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a34c766fedcef740b10fddb96cd1ffd7aeae2d9628ddfa2510fedd4bbe64d2b`  
		Last Modified: Tue, 01 Nov 2022 19:21:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.3532; amd64

```console
$ docker pull caddy@sha256:f279c274451500e517aada07ecabddffd03b23f0b9d81791d2347e369b267a6f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2958579667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c57c677f08a022815e25e725365624f628555a00eab2b42f1830e71794c949`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 12:45:06 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Oct 2022 12:45:07 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Oct 2022 12:45:08 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Oct 2022 12:45:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Oct 2022 12:46:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Oct 2022 12:46:38 GMT
ENV GOPATH=C:\go
# Wed, 12 Oct 2022 12:47:37 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 01 Nov 2022 19:19:52 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:25:48 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 01 Nov 2022 19:25:50 GMT
WORKDIR C:\go
# Tue, 01 Nov 2022 20:18:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 01 Nov 2022 20:18:12 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 20:18:13 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 20:18:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 20:19:33 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 01 Nov 2022 20:19:34 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094a4c27e78f8821517fd551cd9e3d5f4b1e4199bdcd783b3fbda849e4995ad1`  
		Last Modified: Wed, 12 Oct 2022 13:16:26 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e91de5ff2103556b1048388473379f95d41247701f0911ebc7c530a861f3f5e`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52642f9e5e3a52bef8ee5677bcb62a364e07003da51f16eb28b8a4ce34fe9f7d`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26528ba698d400f5680be93457d24581b9e4e7a2399de7bb23cbd549f206613`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c89703eb31300a2a39c85ce287a6b9fe88da033828368275bdbb53c2f7704c`  
		Last Modified: Wed, 12 Oct 2022 13:16:30 GMT  
		Size: 25.4 MB (25439927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8705eaae12fa4840be2d79e376eb1b4b7b18da881acad2892b1c47336e796f46`  
		Last Modified: Wed, 12 Oct 2022 13:16:19 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebda8897c2727e3b971c947385632df6f19de06da75e9f161200d43d1acf714`  
		Last Modified: Wed, 12 Oct 2022 13:16:19 GMT  
		Size: 315.0 KB (315035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8667d37dce62bb077cd534d490f047b61dfe9c30023659258862cada9cbd0ba`  
		Last Modified: Tue, 01 Nov 2022 19:54:40 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac8e32e89f1739964a644b8b8b5b44bbae9752f8ea1f87e93455ca36cc86a7d`  
		Last Modified: Tue, 01 Nov 2022 19:55:33 GMT  
		Size: 157.7 MB (157676844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cabbd4ff51bc72ab20efd9f4eb4ebb788679ef03c2fc9b8a72f711fe3558590`  
		Last Modified: Tue, 01 Nov 2022 19:54:40 GMT  
		Size: 1.5 KB (1459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a7aa6766a51e2f5a5add77b40fd7eafa9d3d5049c3b4506b6b4e6dffb65cd6`  
		Last Modified: Tue, 01 Nov 2022 20:21:08 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54feb136a1e02e5d213be9750ca621c39022ff48f54c1e67daace9a82dd241f1`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7c0ce28f0f06a413d72723dbca806a7b025194983d436501cb04b7b2d7379`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e48594ab78eca9cfe42619a2f721de764c027be8fa22700565227c765b4ed7e`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55feb68cd00871cb13079eb862d65521274326d062594c7522edcc8f9bac23f1`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.6 MB (1631634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d398f623f33e057b5d399473e3ee1243fef32140e9a4411c1f69a913b43acb08`  
		Last Modified: Tue, 01 Nov 2022 20:21:05 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.20348.1129; amd64

```console
$ docker pull caddy@sha256:6e35c0ddda3afe05cb015c908260022b09ae192d81ad72f3bf1e32c70d7cb243
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2659936170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:265570f6cf9dffda304fb3a6712c85940e0f8d23ef6d8ffbfd8e1ebdd6d89d85`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 12:40:52 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Oct 2022 12:40:53 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Oct 2022 12:40:54 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Oct 2022 12:40:55 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Oct 2022 12:41:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Oct 2022 12:41:26 GMT
ENV GOPATH=C:\go
# Wed, 12 Oct 2022 12:41:47 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 01 Nov 2022 19:15:18 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:19:35 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 01 Nov 2022 19:19:38 GMT
WORKDIR C:\go
# Tue, 01 Nov 2022 20:19:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 01 Nov 2022 20:19:43 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 20:19:45 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 20:19:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 20:20:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 01 Nov 2022 20:20:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e9b54b31e104f64c9eb8a65ac0af5effd645bd00a77ea297b6015d28022a74`  
		Last Modified: Mon, 17 Oct 2022 21:39:11 GMT  
		Size: 1000.0 MB (1000028645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f8b589252b90e37349f39b9d4495646791b4050d7cd218336fcc4624b0ebe2`  
		Last Modified: Wed, 12 Oct 2022 13:15:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811ef63d5261b55ee6b499dbc7fcd1ed13386326466fb81a0801abbcbcb75d3f`  
		Last Modified: Wed, 12 Oct 2022 13:15:28 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816740cd643a7a4e72aa527cd033d0c95686c9725ff70dac3260b44dce508e73`  
		Last Modified: Wed, 12 Oct 2022 13:15:28 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599e30c8b316e75d786cfd91f97b9fae4c89fb00f3fce0619eb4e66bc3165521`  
		Last Modified: Wed, 12 Oct 2022 13:15:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77a0d37b81c920d4b783c0b2cfad656a4b8733960ba3afd4e0a1f39f202f948`  
		Last Modified: Wed, 12 Oct 2022 13:15:32 GMT  
		Size: 25.7 MB (25689345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b699f53b56e90279b0bb8ce4434f9b68bbc28fa30756476e22c7ef3dc869e24a`  
		Last Modified: Wed, 12 Oct 2022 13:15:21 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57fcf632f60c89dd981a8a7fa084e738f55129b1786fd9a9e9f5ab8aa1e02d82`  
		Last Modified: Wed, 12 Oct 2022 13:15:24 GMT  
		Size: 526.5 KB (526519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8b0d888223c93af8f0c84ad35156f79df9b0d9ae107f61ded320d2a4fed5f3`  
		Last Modified: Tue, 01 Nov 2022 19:53:29 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49602de12fff655f45d03b1befdd7e56321771c65ed690492e4092da51046bb3`  
		Last Modified: Tue, 01 Nov 2022 19:54:22 GMT  
		Size: 157.8 MB (157838831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cb5ede4eaf1f86f7c0957639a8b53a0c6740df6fa395d3d286e32bff6b9195`  
		Last Modified: Tue, 01 Nov 2022 19:53:29 GMT  
		Size: 1.6 KB (1584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d0ae347408d32205a9ca4c0628e814833984ac8c0fbfb6c6687b9c94a733aa`  
		Last Modified: Tue, 01 Nov 2022 20:21:30 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453489637085324b6412fd9d83cc639d7a9f9135fb5db5dec214462b3293c98f`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cc23fcabe43926f14c7d7e786e9175c87fe573e41fc0158bdc02cfc08fb567`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528f2dc5e38ba5bad570845252c13446ea9637f9c7a80590c93c28886ab79803`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd45b40a0e40f3a52f9a7e2e1cf3cf3b0501ca3f8d637ef46596ee30a9193264`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.8 MB (1837122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bd243dcf25ec803b906e53fa263b2803735773f0227c1c4bac5d52654bb8c6`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:9a51f1a1098ec283efeb9174633447c4bb3142e5bbc7649c8ced7f8d685da3f4
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
$ docker pull caddy@sha256:735ad7b9a5ba5baf3df5f93034af5fa90c3554da9725d260df238d2511be6b23
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133519902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4fa387ebb822f454dc9877bfe19aaba627e1b422f476a4952468eb35c419c3f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 21:16:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 21:16:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 21:16:53 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:20:19 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:21:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:21:57 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:21:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:21:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:21:57 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:49:49 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:49:49 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:49:49 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:49:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:49:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:49:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:49:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4583459ba0371c715f926a9bbd37a9dae909234f4b898220160425131eb53bd4`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 284.7 KB (284734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c1e223e6f2123b855e0c95898eba50cb6a055881ba9023527c0a361761c1cf`  
		Last Modified: Thu, 06 Oct 2022 21:24:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbef1b99e503551b709afdb24ef66954c0792f99d76bb0018afd3a65a1347b5b`  
		Last Modified: Tue, 01 Nov 2022 19:30:19 GMT  
		Size: 122.3 MB (122275572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99825e86aac9391fd3d709522864ff3282479450067b8431df9c4f9e4da4da1`  
		Last Modified: Tue, 01 Nov 2022 19:30:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd6f4fde4a1bb5cc5dd5adba9566a8e0e11ac8cf06adffd9dbefe69a80fc50e`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 6.9 MB (6937644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc2cb786c4d70bac77de2092dd9d3fe5b54e59daa8918ccd6ce64d32929e339`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 1.2 MB (1215184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189da6bcd6c18118e6c5774a9bf9eaba6cde20b87848c17960d265f518beb280`  
		Last Modified: Tue, 01 Nov 2022 19:50:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2b94490e7740d5762996c3f1af82a99c3a298122ab46f5312d75b015ed07fdb3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129501509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:484eab50c7b23327b3246fbfe1577b2cb318df92dd5e1e7695611bc34588a965`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 01 Nov 2022 18:49:34 GMT
RUN apk add --no-cache ca-certificates
# Tue, 01 Nov 2022 18:49:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Nov 2022 18:49:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:49:35 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:51:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:51:57 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:51:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:51:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:51:58 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:18:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:18:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:18:14 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:18:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:18:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:18:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:18:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e34adf14e74afbe714188593430596566b859daec67932063af22ae26cfb41`  
		Last Modified: Tue, 01 Nov 2022 18:59:56 GMT  
		Size: 284.6 KB (284604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30829221241bb1a4c4b78ced30216bd6e772290df6d02b43de82ec13847f2ea`  
		Last Modified: Tue, 01 Nov 2022 18:59:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5175fa50505ed8e1ebb1cc778186a5571aceaf68880fb7f30ce0a002543fde16`  
		Last Modified: Tue, 01 Nov 2022 19:00:18 GMT  
		Size: 118.6 MB (118633129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9462914fb6be31fa7883e2ac24e0b90c77b0dd01eed92e5eb2717d2d58757a21`  
		Last Modified: Tue, 01 Nov 2022 18:59:55 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bae57654f3779f11c3403f04b1e6edc1160b85b75ec1b7aaeebd3ab918fdb3e`  
		Last Modified: Tue, 01 Nov 2022 19:19:10 GMT  
		Size: 6.8 MB (6806143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ccbb51616839b72199c780dc3fb4b40d6337c1b64a8e503b85e43d17ae6bee`  
		Last Modified: Tue, 01 Nov 2022 19:19:09 GMT  
		Size: 1.2 MB (1162983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8bf63e08652d8b6f6f6f0710daa4bfdfd8cd8a9b63599b309be0e046fb2405`  
		Last Modified: Tue, 01 Nov 2022 19:19:09 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:38e0977df61d81ad978adc5aeff5351e967c86e79faa8b7707674d0ac2e63774
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128321867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0724d3115962e959325f2a9a4a8824cd2292a204ddd5db99808f8c1c3b28610a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 03:11:14 GMT
RUN apk add --no-cache ca-certificates
# Thu, 27 Oct 2022 03:11:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 03:11:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:58:35 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:00:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:00:36 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:00:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:00:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:00:37 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:30:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:30:18 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:30:18 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:30:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:30:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:30:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:30:20 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb4eb882dd734293a28e32a55182efac09a590954d1c7e0ac4e9afd668b950f`  
		Last Modified: Thu, 27 Oct 2022 03:23:31 GMT  
		Size: 283.8 KB (283751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62601eba0f2135ba01bd7632b6cd5858fd87c654ebbd7aa446022efda221518`  
		Last Modified: Thu, 27 Oct 2022 03:23:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f8cf932723cb79c6511c7a4565c26fc3c1a8b195b63a1b4f27567664469b8`  
		Last Modified: Tue, 01 Nov 2022 19:11:07 GMT  
		Size: 118.4 MB (118395001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06295a7c5807cf45167f1a47e93084873628c3417ae38bd41c276b71ba1c46ab`  
		Last Modified: Tue, 01 Nov 2022 19:10:45 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92d8ff62b16b450357e75981f8b6277cddab5a79836683195be024c5b466eb1`  
		Last Modified: Tue, 01 Nov 2022 19:31:14 GMT  
		Size: 6.1 MB (6065387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136c853b146e693b550c1d68b6b6713b79d7befffc79acb1530b83593b8fa935`  
		Last Modified: Tue, 01 Nov 2022 19:31:13 GMT  
		Size: 1.2 MB (1159979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f924d6193ccce35a47a6ee295f40e327abf4a8492374030689faf3f505632e08`  
		Last Modified: Tue, 01 Nov 2022 19:31:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6b8569ece82b11e5f6720884af16dce90859af84c6a9ab271ce05a08435fbd77
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127999797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1543ea235e3a8ec3d0ad049bdc81b95745b72848028c6dbc10cde12da0b876fc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 26 Oct 2022 08:09:57 GMT
RUN apk add --no-cache ca-certificates
# Wed, 26 Oct 2022 08:09:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 Oct 2022 08:09:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:40:17 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:41:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:41:34 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:41:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:41:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:41:35 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:05:53 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:05:53 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:05:53 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:05:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:05:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:05:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:05:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d82f9e3411d2eff49049d09ae871e53b96a0cc7dd335883f1fec28c43f9c86`  
		Last Modified: Wed, 26 Oct 2022 08:17:16 GMT  
		Size: 284.7 KB (284723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e169736571560c1a3278f9971532d55ddc4abfaef12e8c54c05f4644445d5520`  
		Last Modified: Wed, 26 Oct 2022 08:17:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc530f9a61e7c0e16b1cb3d48b70136b625cf624976acc638b9d6aef5525995`  
		Last Modified: Tue, 01 Nov 2022 18:48:07 GMT  
		Size: 116.8 MB (116836732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562d55c2123be45d40bfd4dd4dea65161ad3d83b50153de3cc0b63ec7a061f4b`  
		Last Modified: Tue, 01 Nov 2022 18:47:54 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90594629b6df4d09d221ea3fc570b4944e36520a3503ffa3a838772b0e46561`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 7.0 MB (7049481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e41bd715f5f0d05c59b600661a8f0cfb5145de632b14a77d012cfd1ffeea780`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 1.1 MB (1120483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3da6b029e0d694358fe69ed7435eb464495babb3bc51d3d5f30a5222406935`  
		Last Modified: Tue, 01 Nov 2022 19:06:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:0bfdd9fd29aabe5e64b1c692ef01a8064dc2c4932747c3bf06363fd238817630
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128911035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3d666ccc1132e45cb0e54d7fd1891ab309ad3ae1fa96a20556f67f531c4bcc0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:26:01 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:26:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:26:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:17:13 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:19:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 19:20:03 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 19:20:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 19:20:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 19:20:05 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:50:45 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:50:46 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:50:46 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:50:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:50:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:50:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:50:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36899d7325c2c25a7d8e61ef33bb1e93b83f811f462e9ddad81c86df87b0685`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 286.7 KB (286747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9309524edda98df2abd6704c6f56004422a28b63364f028763ea000fc32d6eca`  
		Last Modified: Thu, 06 Oct 2022 20:39:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b608654249afe5c44e2b3f100f6b333302506cd24adc46afa3302bb03ff96e`  
		Last Modified: Tue, 01 Nov 2022 19:31:59 GMT  
		Size: 117.2 MB (117238077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93311758f4ff1a16fa50dab5c51c12dd47a1920496e07493f5452c97e24eff9c`  
		Last Modified: Tue, 01 Nov 2022 19:31:32 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce6b57ae4a73b81094351a45358cebcbfbccd4d0d31ab77e71afc97d675dc63`  
		Last Modified: Tue, 01 Nov 2022 19:51:34 GMT  
		Size: 7.5 MB (7478322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5fa9d97b98179c5269f7f488f5488ec1a31fa543c75dc88705c8ed0a755e1c`  
		Last Modified: Tue, 01 Nov 2022 19:51:33 GMT  
		Size: 1.1 MB (1103853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f6efc0777ee24d394842b20cc0fe8c229ae5fecbb8dbb5537e66f5fc1fcf41`  
		Last Modified: Tue, 01 Nov 2022 19:51:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:660f4e58ece536977f580dad53c004e3fe9b1496a0af262adf93a8480746e615
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131825256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d3b89f5e95a2acfe27efc6ab49664e2a25268891a03b26100d1cca071938a79`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:16:09 GMT
RUN apk add --no-cache ca-certificates
# Thu, 06 Oct 2022 20:16:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:16:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:43:10 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 18:46:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.3.src.tar.gz'; 		sha256='18ac263e39210bcf68d85f4370e97fb1734166995a1f63fb38b4f6e07d90d212'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 01 Nov 2022 18:47:10 GMT
ENV GOPATH=/go
# Tue, 01 Nov 2022 18:47:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Nov 2022 18:47:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Nov 2022 18:47:13 GMT
WORKDIR /go
# Tue, 01 Nov 2022 19:20:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Nov 2022 19:20:25 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 19:20:26 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 19:20:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 19:20:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='bffe075ac254111ead0238c330a33c7f39f9cc5f7d2b4b3fce48256d79c3f5fb94aec23d816c9ea0e21cd51bda058c05336cfa2849a0d25d821c9280962f9a53' ;; 		armhf)   binArch='armv6'; checksum='6e988c78881bf6463d92e2194a815a243b0b1bb185ff37f321bd74694d55c6ae6490403e99b165fa3548d37340230ef486cba7ff3801d53607d8df4c036baf4c' ;; 		armv7)   binArch='armv7'; checksum='ace94e101d1d1fa368b644043dce5e46a634dd85ecf2a8fcec367281420af48c7609cf451f2930d07fce6238e68dd9848e48aef203dd5c6b4f64c2a67e3010d3' ;; 		aarch64) binArch='arm64'; checksum='97f3d83124846a22080dd1136d066141c0972a31abc4d54aefd9e7c7a4ad0b3deeede5df4e24b190291235c337c06c340bcdc29e302c253a667494c6825d2a0c' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ae8d994dbd1870efb54fcfa7d10b541a01afee482102a5fa0b5852848d88775a54056ecacd96192116cb205bead6a6e3165192a0d1b91f4fc5ef73c9368bc5d0' ;; 		s390x)   binArch='s390x'; checksum='a7ed957d3b9cda7345ae4444302d53c12cf648ec7c354de93c92fbd7a10d104d90cc2b3b41ff357969baaeadb6dab5c074f735bcc41520b7ba35dada87a4ac8f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 01 Nov 2022 19:20:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 01 Nov 2022 19:20:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d31ae2e1f77c70a25e9cbeea435b4ab68149a4e17f9d4668768da8dd5ac68a`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 285.0 KB (284954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2788e533105e3c00ed84523a8f99d7947c0bb8b12932018a3081ecc29964605`  
		Last Modified: Thu, 06 Oct 2022 20:26:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a12f83dfb1b48c3152a859b9b55b4483128b0be37e4877271cbd453b23fb43`  
		Last Modified: Tue, 01 Nov 2022 19:02:36 GMT  
		Size: 120.7 MB (120729474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e663873bb0a71689aee0be3ce5f4195e0b573039585fcc3182fe189e8e8fe05`  
		Last Modified: Tue, 01 Nov 2022 19:02:21 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802d29971118d482599687d5c1f1c069a8f0b8cb0c96e3ec3d5f550416223491`  
		Last Modified: Tue, 01 Nov 2022 19:21:20 GMT  
		Size: 7.1 MB (7052072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eea39f6b8018dc8d0011d05cdf7f2412b1435fdedc607d0087cfb9c631ccc23`  
		Last Modified: Tue, 01 Nov 2022 19:21:19 GMT  
		Size: 1.2 MB (1167444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a34c766fedcef740b10fddb96cd1ffd7aeae2d9628ddfa2510fedd4bbe64d2b`  
		Last Modified: Tue, 01 Nov 2022 19:21:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:ee5b9081fd81e7adbf4a0c1bf8fd4f9f882e755ac9fc03b24f12c7699aa5b52b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull caddy@sha256:f279c274451500e517aada07ecabddffd03b23f0b9d81791d2347e369b267a6f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2958579667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c57c677f08a022815e25e725365624f628555a00eab2b42f1830e71794c949`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 12:45:06 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Oct 2022 12:45:07 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Oct 2022 12:45:08 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Oct 2022 12:45:09 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Oct 2022 12:46:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Oct 2022 12:46:38 GMT
ENV GOPATH=C:\go
# Wed, 12 Oct 2022 12:47:37 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 01 Nov 2022 19:19:52 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:25:48 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 01 Nov 2022 19:25:50 GMT
WORKDIR C:\go
# Tue, 01 Nov 2022 20:18:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 01 Nov 2022 20:18:12 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 20:18:13 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 20:18:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 20:19:33 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 01 Nov 2022 20:19:34 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094a4c27e78f8821517fd551cd9e3d5f4b1e4199bdcd783b3fbda849e4995ad1`  
		Last Modified: Wed, 12 Oct 2022 13:16:26 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e91de5ff2103556b1048388473379f95d41247701f0911ebc7c530a861f3f5e`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52642f9e5e3a52bef8ee5677bcb62a364e07003da51f16eb28b8a4ce34fe9f7d`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26528ba698d400f5680be93457d24581b9e4e7a2399de7bb23cbd549f206613`  
		Last Modified: Wed, 12 Oct 2022 13:16:22 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c89703eb31300a2a39c85ce287a6b9fe88da033828368275bdbb53c2f7704c`  
		Last Modified: Wed, 12 Oct 2022 13:16:30 GMT  
		Size: 25.4 MB (25439927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8705eaae12fa4840be2d79e376eb1b4b7b18da881acad2892b1c47336e796f46`  
		Last Modified: Wed, 12 Oct 2022 13:16:19 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebda8897c2727e3b971c947385632df6f19de06da75e9f161200d43d1acf714`  
		Last Modified: Wed, 12 Oct 2022 13:16:19 GMT  
		Size: 315.0 KB (315035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8667d37dce62bb077cd534d490f047b61dfe9c30023659258862cada9cbd0ba`  
		Last Modified: Tue, 01 Nov 2022 19:54:40 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac8e32e89f1739964a644b8b8b5b44bbae9752f8ea1f87e93455ca36cc86a7d`  
		Last Modified: Tue, 01 Nov 2022 19:55:33 GMT  
		Size: 157.7 MB (157676844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cabbd4ff51bc72ab20efd9f4eb4ebb788679ef03c2fc9b8a72f711fe3558590`  
		Last Modified: Tue, 01 Nov 2022 19:54:40 GMT  
		Size: 1.5 KB (1459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a7aa6766a51e2f5a5add77b40fd7eafa9d3d5049c3b4506b6b4e6dffb65cd6`  
		Last Modified: Tue, 01 Nov 2022 20:21:08 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54feb136a1e02e5d213be9750ca621c39022ff48f54c1e67daace9a82dd241f1`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7c0ce28f0f06a413d72723dbca806a7b025194983d436501cb04b7b2d7379`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e48594ab78eca9cfe42619a2f721de764c027be8fa22700565227c765b4ed7e`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55feb68cd00871cb13079eb862d65521274326d062594c7522edcc8f9bac23f1`  
		Last Modified: Tue, 01 Nov 2022 20:21:06 GMT  
		Size: 1.6 MB (1631634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d398f623f33e057b5d399473e3ee1243fef32140e9a4411c1f69a913b43acb08`  
		Last Modified: Tue, 01 Nov 2022 20:21:05 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:39520901129debe71fc3b671250e73c438c85ee3435b24c8c8c5bc6293f05800
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1129; amd64

### `caddy:builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1129; amd64

```console
$ docker pull caddy@sha256:6e35c0ddda3afe05cb015c908260022b09ae192d81ad72f3bf1e32c70d7cb243
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2659936170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:265570f6cf9dffda304fb3a6712c85940e0f8d23ef6d8ffbfd8e1ebdd6d89d85`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 12:40:52 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Oct 2022 12:40:53 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Oct 2022 12:40:54 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Oct 2022 12:40:55 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Oct 2022 12:41:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Oct 2022 12:41:26 GMT
ENV GOPATH=C:\go
# Wed, 12 Oct 2022 12:41:47 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 01 Nov 2022 19:15:18 GMT
ENV GOLANG_VERSION=1.19.3
# Tue, 01 Nov 2022 19:19:35 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 01 Nov 2022 19:19:38 GMT
WORKDIR C:\go
# Tue, 01 Nov 2022 20:19:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 01 Nov 2022 20:19:43 GMT
ENV XCADDY_VERSION=v0.3.1
# Tue, 01 Nov 2022 20:19:45 GMT
ENV CADDY_VERSION=v2.6.2
# Tue, 01 Nov 2022 20:19:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 01 Nov 2022 20:20:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 01 Nov 2022 20:20:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e9b54b31e104f64c9eb8a65ac0af5effd645bd00a77ea297b6015d28022a74`  
		Last Modified: Mon, 17 Oct 2022 21:39:11 GMT  
		Size: 1000.0 MB (1000028645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f8b589252b90e37349f39b9d4495646791b4050d7cd218336fcc4624b0ebe2`  
		Last Modified: Wed, 12 Oct 2022 13:15:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811ef63d5261b55ee6b499dbc7fcd1ed13386326466fb81a0801abbcbcb75d3f`  
		Last Modified: Wed, 12 Oct 2022 13:15:28 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816740cd643a7a4e72aa527cd033d0c95686c9725ff70dac3260b44dce508e73`  
		Last Modified: Wed, 12 Oct 2022 13:15:28 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599e30c8b316e75d786cfd91f97b9fae4c89fb00f3fce0619eb4e66bc3165521`  
		Last Modified: Wed, 12 Oct 2022 13:15:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77a0d37b81c920d4b783c0b2cfad656a4b8733960ba3afd4e0a1f39f202f948`  
		Last Modified: Wed, 12 Oct 2022 13:15:32 GMT  
		Size: 25.7 MB (25689345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b699f53b56e90279b0bb8ce4434f9b68bbc28fa30756476e22c7ef3dc869e24a`  
		Last Modified: Wed, 12 Oct 2022 13:15:21 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57fcf632f60c89dd981a8a7fa084e738f55129b1786fd9a9e9f5ab8aa1e02d82`  
		Last Modified: Wed, 12 Oct 2022 13:15:24 GMT  
		Size: 526.5 KB (526519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8b0d888223c93af8f0c84ad35156f79df9b0d9ae107f61ded320d2a4fed5f3`  
		Last Modified: Tue, 01 Nov 2022 19:53:29 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49602de12fff655f45d03b1befdd7e56321771c65ed690492e4092da51046bb3`  
		Last Modified: Tue, 01 Nov 2022 19:54:22 GMT  
		Size: 157.8 MB (157838831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cb5ede4eaf1f86f7c0957639a8b53a0c6740df6fa395d3d286e32bff6b9195`  
		Last Modified: Tue, 01 Nov 2022 19:53:29 GMT  
		Size: 1.6 KB (1584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d0ae347408d32205a9ca4c0628e814833984ac8c0fbfb6c6687b9c94a733aa`  
		Last Modified: Tue, 01 Nov 2022 20:21:30 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453489637085324b6412fd9d83cc639d7a9f9135fb5db5dec214462b3293c98f`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cc23fcabe43926f14c7d7e786e9175c87fe573e41fc0158bdc02cfc08fb567`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528f2dc5e38ba5bad570845252c13446ea9637f9c7a80590c93c28886ab79803`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd45b40a0e40f3a52f9a7e2e1cf3cf3b0501ca3f8d637ef46596ee30a9193264`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.8 MB (1837122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bd243dcf25ec803b906e53fa263b2803735773f0227c1c4bac5d52654bb8c6`  
		Last Modified: Tue, 01 Nov 2022 20:21:27 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:d3e5e175b10a2a5b66be9570ed9867aeb77af8eca7a14b6033dcde2c9f6fee6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3532; amd64
	-	windows version 10.0.20348.1129; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:7992b931b7da3cf0840dd69ea74b2c67d423faf03408da8abdc31b7590a239a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17676993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:006d393a4e6a01f82413e41b3e0f06dfb1872d5ca6a37aba315e4ec9e2cc6c4c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:34:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 04:34:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 01:43:19 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 01:43:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 01:43:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 01:43:22 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 01:43:22 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 01:43:22 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 01:43:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 01:43:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 80
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 443
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 01:43:23 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 01:43:24 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 01:43:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5625668cf98fd3e4d769f18d45f27e34fe3d085cfb9927ff7ad2cdc84d8c493f`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 304.5 KB (304517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675d09b34c5347b62625d31b2a458824240b90e51d18bcc38ad37d317e83d64c`  
		Last Modified: Fri, 07 Oct 2022 04:35:24 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1747be7065842ba85f86aed65e75608dfd2f546ab9d8ecd4a8842c8f4634795`  
		Last Modified: Fri, 14 Oct 2022 01:43:47 GMT  
		Size: 14.6 MB (14560435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8ee6c4c21d12cd28fcd0e196acb8569f35518dc36c691c91b4c8ca1928bf9d`  
		Last Modified: Fri, 14 Oct 2022 01:43:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:76b70e0dc74358fc1f7ef178c46cc9c047a90cd05e842d26305da1ee04ff3ad8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16834877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cac02415934eaae38be5b122f6a0c760f747e6f50f1551c9a45f4f186454f04`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 19:49:23 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 27 Oct 2022 19:49:25 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 27 Oct 2022 19:49:25 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 27 Oct 2022 19:49:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 27 Oct 2022 19:49:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 19:49:28 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 27 Oct 2022 19:49:28 GMT
ENV XDG_DATA_HOME=/data
# Thu, 27 Oct 2022 19:49:28 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 27 Oct 2022 19:49:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 27 Oct 2022 19:49:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 80
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 443
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 443/udp
# Thu, 27 Oct 2022 19:49:29 GMT
EXPOSE 2019
# Thu, 27 Oct 2022 19:49:30 GMT
WORKDIR /srv
# Thu, 27 Oct 2022 19:49:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7f6197b1f089356a6bff8bf29fdcef692051048bd17db70d72df822c89c04d`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 304.4 KB (304404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc91cb09da181c7973089ccf7aca9c7830c738ac1e614883f86c2eecdcb68002`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 5.8 KB (5751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ffb96b75d9dc6019cfe6202b9fed588b3ff9a91cc89237d6a24c98eb5fd590`  
		Last Modified: Thu, 27 Oct 2022 19:50:36 GMT  
		Size: 13.9 MB (13910603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb4866598fa794379095b277b41d4b0cb626d61cc20c6f6cff7d920bc99330`  
		Last Modified: Thu, 27 Oct 2022 19:50:33 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9df5bfbadaf5495675c4de47918d3631d439d159681e352069eaa206f664a8ac
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16617541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d61e1121278866d5afee597ba2ac37a9b5bec51b6323b551fe9a89b5d99d63e5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Thu, 27 Oct 2022 10:30:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 27 Oct 2022 10:30:41 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 27 Oct 2022 10:30:41 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 27 Oct 2022 10:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 27 Oct 2022 10:30:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 Oct 2022 10:30:45 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 27 Oct 2022 10:30:45 GMT
ENV XDG_DATA_HOME=/data
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 27 Oct 2022 10:30:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 27 Oct 2022 10:30:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 80
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 443
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 443/udp
# Thu, 27 Oct 2022 10:30:46 GMT
EXPOSE 2019
# Thu, 27 Oct 2022 10:30:46 GMT
WORKDIR /srv
# Thu, 27 Oct 2022 10:30:46 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9f1011ebc9810d3e61468e7ce6c2866fc65920db06e3bccde2da749f976500`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 303.5 KB (303537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28310071f60503f30048b0cad1abe85c763c57dd4e69715cc57d60560481318`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 5.8 KB (5753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7792abbee8ad8ec28f7e6e2864a9e8ad229de5f701ba4bf04be77cffac8835ac`  
		Last Modified: Thu, 27 Oct 2022 10:31:39 GMT  
		Size: 13.9 MB (13891032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c5be986b3fadf5f34a0a4311ffa6a22b4f1f0ff79c510fb7c58cb93c64e2f3`  
		Last Modified: Thu, 27 Oct 2022 10:31:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f06fb46d2c67f3b7f9447b6c19f5b9909931b603d2b475f647624f577c6d94ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16278669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8876f25c7ec7330d6bf197e452e3a37deeea42e52b8c2b2c9103bc86b26795`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 26 Oct 2022 18:53:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 26 Oct 2022 18:53:58 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Wed, 26 Oct 2022 18:53:58 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 26 Oct 2022 18:54:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 26 Oct 2022 18:54:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 26 Oct 2022 18:54:01 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 26 Oct 2022 18:54:01 GMT
ENV XDG_DATA_HOME=/data
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Oct 2022 18:54:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Oct 2022 18:54:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 80
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 443
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 443/udp
# Wed, 26 Oct 2022 18:54:02 GMT
EXPOSE 2019
# Wed, 26 Oct 2022 18:54:02 GMT
WORKDIR /srv
# Wed, 26 Oct 2022 18:54:02 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5532e6e746eecf0e890ee17251a52841dd55694ae55c919dc6ddf6159e27cd5b`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 304.5 KB (304512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b816658ad2f9debd81f6df21dd733e54fc6eda530080cc3957e6f63d9677b9a`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d7ee92d83c49ca71b5440fd76d22ac6b75304bc48a0183bf392689ae8d5897`  
		Last Modified: Wed, 26 Oct 2022 18:54:26 GMT  
		Size: 13.3 MB (13260508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00da94c60a7ed1fc9acd392aedea2ab7b2bd6a7d67cc83b2d5d85c5cbd40090b`  
		Last Modified: Wed, 26 Oct 2022 18:54:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:9665c6fd33be967b3bdfcdbeeb605e3a92e70080ef5caa8907a6cbdef064be3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (16031232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96553401995800bf37590502c237b4ab8cee57bd3885e83f76dcb42c53a7d7db`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:56:10 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 07:56:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 03:47:38 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 03:47:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 03:47:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 03:47:44 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 03:47:44 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 03:47:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 03:47:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 03:47:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 03:47:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 80
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 443
# Fri, 14 Oct 2022 03:47:48 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 03:47:49 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 03:47:49 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 03:47:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf49ba2a5c90a152d4aef09519c7019835fbf2884d6afb1c85b3353b7d91388e`  
		Last Modified: Fri, 07 Oct 2022 07:57:09 GMT  
		Size: 306.5 KB (306522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dac87aba8912de3ce6fb3ca14bb6833f931fd15d7ec2d7435a18f11e5ddb6fb`  
		Last Modified: Fri, 07 Oct 2022 07:57:08 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea24f9a44c53fbd359328daff2e10e4e3f1c7d7bae21190ea2f6af3be43dd0b`  
		Last Modified: Fri, 14 Oct 2022 03:48:33 GMT  
		Size: 12.9 MB (12915404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4704e2ddccf987da9605ef1c8d4ef68a86cf3e6ba2f8c5d1e80e5915481e25c`  
		Last Modified: Fri, 14 Oct 2022 03:48:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:5702e27172b1bfb5e9930d544d7cf16a83f774419b1aa2078be464351ff5f70b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16967685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05ec4a186bcadcf0e691a443c7edebf42d46cff3997d01a56de43db0ecbab8e2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 10:23:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 07 Oct 2022 10:23:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 14 Oct 2022 00:55:05 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 14 Oct 2022 00:55:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 14 Oct 2022 00:55:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 14 Oct 2022 00:55:15 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 14 Oct 2022 00:55:16 GMT
ENV XDG_DATA_HOME=/data
# Fri, 14 Oct 2022 00:55:17 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 14 Oct 2022 00:55:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 14 Oct 2022 00:55:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 14 Oct 2022 00:55:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 14 Oct 2022 00:55:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 14 Oct 2022 00:55:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 14 Oct 2022 00:55:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 14 Oct 2022 00:55:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 14 Oct 2022 00:55:22 GMT
EXPOSE 80
# Fri, 14 Oct 2022 00:55:22 GMT
EXPOSE 443
# Fri, 14 Oct 2022 00:55:23 GMT
EXPOSE 443/udp
# Fri, 14 Oct 2022 00:55:23 GMT
EXPOSE 2019
# Fri, 14 Oct 2022 00:55:24 GMT
WORKDIR /srv
# Fri, 14 Oct 2022 00:55:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5123e0e5a47a6dfbd8cae1e2589df59b198f82ba790c211aeb3eefbbe41a17be`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 304.8 KB (304752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557f08048878eca2f16fd3b05bb138300739b9e74e467509792efc4278e74b3f`  
		Last Modified: Fri, 07 Oct 2022 10:25:11 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91158060b74650f434cb3419f6ed862b0616480567b651bfae73b297f69b9992`  
		Last Modified: Fri, 14 Oct 2022 00:56:22 GMT  
		Size: 14.1 MB (14066352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511ac9f174e3fed802157937e9192a940800d73835958de90f5a363b5edf46ad`  
		Last Modified: Fri, 14 Oct 2022 00:56:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.3532; amd64

```console
$ docker pull caddy@sha256:c795b26fccceaa3ea3738c3d086e0c9da9978392aeb6e2c69ae3d71131b88998
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726785951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a0ffc50daa8e99f5d3029bd930601ec939b66a180da1ad5fef783d1fcb69eb3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 16:58:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:14:49 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:16:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:16:10 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:16:11 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:16:12 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:16:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:16:14 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:16:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:16:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:16:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:16:19 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:16:20 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:16:21 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:16:22 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:17:16 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:17:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:028c482fad0f111537a40f65401f65de54c9fd682951a4f8cf9b644d7c128e18`  
		Size: 834.0 MB (833997855 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77462c8fbd8b2782ee2fc5f09bebfb350912f754186b058478ab8d22f50bb047`  
		Last Modified: Wed, 12 Oct 2022 17:04:34 GMT  
		Size: 358.2 KB (358248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a372be4d9f43d4d5884bc4093c44aedf12150f55ea9457baa2fcceb43ef8074`  
		Last Modified: Thu, 13 Oct 2022 23:21:08 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a8993c29bb6d4c31b0be3609bc7fb2af2666435fe70bb2f329784277d629d1`  
		Last Modified: Thu, 13 Oct 2022 23:21:11 GMT  
		Size: 14.9 MB (14947938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98662b730099437011356fa77ef9072054f4ad73d3781e9b02d4750689762162`  
		Last Modified: Thu, 13 Oct 2022 23:21:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7e77f6a080ad6fa8a7320831868ccd7b6385e995988f2e6cca76090a565c99`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec71d29d036cab0bdbc7765216513aad527933ededfec4492a97724c6bab52d`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a11bac4631094c366303dd3c571fe04cf1b543bafba72d8dd1030f8ae2ec185`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4dc588cdabd0672f8b29c59cd9ddc6d927160284a6f6529fbe39b8e34ca766`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f39777f21d48153f681f16b5a1cd2e12440066bc96a665fa3b85a6275b74942`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638736df2ba6ceaed21b97ee12046d2d0494561bd735581618ab505ff602b0da`  
		Last Modified: Thu, 13 Oct 2022 23:21:04 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e0fe53dba785fdf61d7431392d7e15beeebbe5f215d9a2de2ee00975e7b5c4`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb7b8fc42485b0656b2afcb99344cda044ce10d0107cc91955fbe11433c358`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb8f166931be4f8f0b0a07611df01a8e7d1101f8a8ce564144ded43917e1021`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bc6f4b7a114b7722cfc81aa83b74727261766c2cef9bc0787e447435c33d2a`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5563ab3963680a40da3bc2269bbc1e76362b359547dae9705892cf8f54b50dd1`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d300f0320cd2b8ce3f3e58cbb3acb06e24c5f59a342725056a10667329f914`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfb9dfa0b00914a255876439613219f4a74e83734df6b8a197e6e0bb53bf905`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b9233dbf203ca77eea2271813856d219ba7d2f633adf99f3262612edfad738`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 291.8 KB (291836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefde31b509f056641749adae4daa4e0ad3265d260ac1c61b41c8950a10824e6`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.20348.1129; amd64

```console
$ docker pull caddy@sha256:e1e15c80e157d71221ec43035cae93b3ea8ba7a6b203428e93159aa6ff5e1463
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2432333411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbd806ca24dfacee0d098f111cc9f6d5f42fdbd9db91a63a8de0d048d3984d5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 17:01:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:17:37 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:18:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:18:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:18:13 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:18:13 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:18:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:18:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:18:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:18:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:18:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:18:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:18:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:18:21 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:18:22 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:18:23 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:18:24 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:18:40 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:18:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ab91661ce2a2a2c14684a2ba0f543a81d7896773f88200b31be0e37c589de38`  
		Size: 979.4 MB (979359717 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cd84a277fd91a008fe0c8fc7d6706544075a294512940b16f57998588ea892`  
		Last Modified: Wed, 12 Oct 2022 17:04:58 GMT  
		Size: 616.9 KB (616893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b069dfbedeca0437916f85fdd78a598955839b91ffc4cba4d6327e5c79487`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5263d846656ffa3662062b1a58d9c6d114e00fa5344edc9b93ea5895c4fa46`  
		Last Modified: Thu, 13 Oct 2022 23:21:34 GMT  
		Size: 15.1 MB (15149356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e378404d94c7fb280c51201d60aef05af3196a0ead3b716521cedbe766ba5e3e`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11749bcf2c3e4097f9a1a30d1fc22184e48c94ab54945730c51c36be175c668d`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cb14f39fa0dce5d6dab4bdd1a896c02b5a6bba01dcd46ed36928c2cce27295`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf622a21cfc36d8958be2f273f52b7d4824d500be08f6a2de791506dcc6c981f`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b246af35953d05f1c4292cb1cf8cfc29215ceac2e013ae2a0759aa2d216516`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08367cd2562c20737156e692dca481f835f4832fabb63602fb5edc78494057ae`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6d70510bf329eff739580f04b59acba9cb4aa74e57bcb6fca996d6df6b6d2c`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc6e963fa5949ceb99519a652299dea21a92c9389aadabedb2deeb4e51855b5`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d175d8244325a62c683c4d1fa6cc266f73231f93142fd0f52c3378da6db1464`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4ce9495075c9b00994ef154c9eb0974ba1853a8244869e35af4eecfca4dce7`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceee07aab1c573de692984f7655da9e6c4aee31260b8df8735344242e6f1ff8`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295041dd24e85177aaf7e1bbd1c0b032d2eafaf3da59213972894238dd5b3d72`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3583f031f13dfd9a933b6e8d4808a3ac7f3e007d2e751af9581b76b08b6e0c4a`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1603973d06c7b0a01ab165d727b40f842361ce898a8e7b8579d6bd9db938c8a6`  
		Last Modified: Thu, 13 Oct 2022 23:21:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c4bf5f410b0a58ef5b477fdf99b90ad01e7deb85b685cf06eaae5c9d83a531`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 319.8 KB (319842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da4c854489e4317220200f8dca47e2335696fe8fa9e7a2aa678467b12b4db7b`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:a2ab9b4da81fb5793c09308f6353dec3d5aa70255288aa5a9390cf5333e74935
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3532; amd64
	-	windows version 10.0.20348.1129; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.3532; amd64

```console
$ docker pull caddy@sha256:c795b26fccceaa3ea3738c3d086e0c9da9978392aeb6e2c69ae3d71131b88998
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726785951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a0ffc50daa8e99f5d3029bd930601ec939b66a180da1ad5fef783d1fcb69eb3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 16:58:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:14:49 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:16:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:16:10 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:16:11 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:16:12 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:16:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:16:14 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:16:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:16:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:16:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:16:19 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:16:20 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:16:21 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:16:22 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:17:16 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:17:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:028c482fad0f111537a40f65401f65de54c9fd682951a4f8cf9b644d7c128e18`  
		Size: 834.0 MB (833997855 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77462c8fbd8b2782ee2fc5f09bebfb350912f754186b058478ab8d22f50bb047`  
		Last Modified: Wed, 12 Oct 2022 17:04:34 GMT  
		Size: 358.2 KB (358248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a372be4d9f43d4d5884bc4093c44aedf12150f55ea9457baa2fcceb43ef8074`  
		Last Modified: Thu, 13 Oct 2022 23:21:08 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a8993c29bb6d4c31b0be3609bc7fb2af2666435fe70bb2f329784277d629d1`  
		Last Modified: Thu, 13 Oct 2022 23:21:11 GMT  
		Size: 14.9 MB (14947938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98662b730099437011356fa77ef9072054f4ad73d3781e9b02d4750689762162`  
		Last Modified: Thu, 13 Oct 2022 23:21:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7e77f6a080ad6fa8a7320831868ccd7b6385e995988f2e6cca76090a565c99`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec71d29d036cab0bdbc7765216513aad527933ededfec4492a97724c6bab52d`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a11bac4631094c366303dd3c571fe04cf1b543bafba72d8dd1030f8ae2ec185`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4dc588cdabd0672f8b29c59cd9ddc6d927160284a6f6529fbe39b8e34ca766`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f39777f21d48153f681f16b5a1cd2e12440066bc96a665fa3b85a6275b74942`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638736df2ba6ceaed21b97ee12046d2d0494561bd735581618ab505ff602b0da`  
		Last Modified: Thu, 13 Oct 2022 23:21:04 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e0fe53dba785fdf61d7431392d7e15beeebbe5f215d9a2de2ee00975e7b5c4`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb7b8fc42485b0656b2afcb99344cda044ce10d0107cc91955fbe11433c358`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb8f166931be4f8f0b0a07611df01a8e7d1101f8a8ce564144ded43917e1021`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bc6f4b7a114b7722cfc81aa83b74727261766c2cef9bc0787e447435c33d2a`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5563ab3963680a40da3bc2269bbc1e76362b359547dae9705892cf8f54b50dd1`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d300f0320cd2b8ce3f3e58cbb3acb06e24c5f59a342725056a10667329f914`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfb9dfa0b00914a255876439613219f4a74e83734df6b8a197e6e0bb53bf905`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b9233dbf203ca77eea2271813856d219ba7d2f633adf99f3262612edfad738`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 291.8 KB (291836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefde31b509f056641749adae4daa4e0ad3265d260ac1c61b41c8950a10824e6`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.20348.1129; amd64

```console
$ docker pull caddy@sha256:e1e15c80e157d71221ec43035cae93b3ea8ba7a6b203428e93159aa6ff5e1463
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2432333411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbd806ca24dfacee0d098f111cc9f6d5f42fdbd9db91a63a8de0d048d3984d5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 17:01:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:17:37 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:18:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:18:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:18:13 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:18:13 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:18:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:18:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:18:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:18:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:18:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:18:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:18:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:18:21 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:18:22 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:18:23 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:18:24 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:18:40 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:18:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ab91661ce2a2a2c14684a2ba0f543a81d7896773f88200b31be0e37c589de38`  
		Size: 979.4 MB (979359717 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cd84a277fd91a008fe0c8fc7d6706544075a294512940b16f57998588ea892`  
		Last Modified: Wed, 12 Oct 2022 17:04:58 GMT  
		Size: 616.9 KB (616893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b069dfbedeca0437916f85fdd78a598955839b91ffc4cba4d6327e5c79487`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5263d846656ffa3662062b1a58d9c6d114e00fa5344edc9b93ea5895c4fa46`  
		Last Modified: Thu, 13 Oct 2022 23:21:34 GMT  
		Size: 15.1 MB (15149356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e378404d94c7fb280c51201d60aef05af3196a0ead3b716521cedbe766ba5e3e`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11749bcf2c3e4097f9a1a30d1fc22184e48c94ab54945730c51c36be175c668d`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cb14f39fa0dce5d6dab4bdd1a896c02b5a6bba01dcd46ed36928c2cce27295`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf622a21cfc36d8958be2f273f52b7d4824d500be08f6a2de791506dcc6c981f`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b246af35953d05f1c4292cb1cf8cfc29215ceac2e013ae2a0759aa2d216516`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08367cd2562c20737156e692dca481f835f4832fabb63602fb5edc78494057ae`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6d70510bf329eff739580f04b59acba9cb4aa74e57bcb6fca996d6df6b6d2c`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc6e963fa5949ceb99519a652299dea21a92c9389aadabedb2deeb4e51855b5`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d175d8244325a62c683c4d1fa6cc266f73231f93142fd0f52c3378da6db1464`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4ce9495075c9b00994ef154c9eb0974ba1853a8244869e35af4eecfca4dce7`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceee07aab1c573de692984f7655da9e6c4aee31260b8df8735344242e6f1ff8`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295041dd24e85177aaf7e1bbd1c0b032d2eafaf3da59213972894238dd5b3d72`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3583f031f13dfd9a933b6e8d4808a3ac7f3e007d2e751af9581b76b08b6e0c4a`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1603973d06c7b0a01ab165d727b40f842361ce898a8e7b8579d6bd9db938c8a6`  
		Last Modified: Thu, 13 Oct 2022 23:21:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c4bf5f410b0a58ef5b477fdf99b90ad01e7deb85b685cf06eaae5c9d83a531`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 319.8 KB (319842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da4c854489e4317220200f8dca47e2335696fe8fa9e7a2aa678467b12b4db7b`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:750ce937e1a109f41cc11cad93540eeb4b7ab051847137267847c104941dfe75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull caddy@sha256:c795b26fccceaa3ea3738c3d086e0c9da9978392aeb6e2c69ae3d71131b88998
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726785951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a0ffc50daa8e99f5d3029bd930601ec939b66a180da1ad5fef783d1fcb69eb3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 16:58:31 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:14:49 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:16:09 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:16:10 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:16:11 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:16:12 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:16:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:16:14 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:16:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:16:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:16:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:16:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:16:19 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:16:20 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:16:21 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:16:22 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:17:16 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:17:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:028c482fad0f111537a40f65401f65de54c9fd682951a4f8cf9b644d7c128e18`  
		Size: 834.0 MB (833997855 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77462c8fbd8b2782ee2fc5f09bebfb350912f754186b058478ab8d22f50bb047`  
		Last Modified: Wed, 12 Oct 2022 17:04:34 GMT  
		Size: 358.2 KB (358248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a372be4d9f43d4d5884bc4093c44aedf12150f55ea9457baa2fcceb43ef8074`  
		Last Modified: Thu, 13 Oct 2022 23:21:08 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a8993c29bb6d4c31b0be3609bc7fb2af2666435fe70bb2f329784277d629d1`  
		Last Modified: Thu, 13 Oct 2022 23:21:11 GMT  
		Size: 14.9 MB (14947938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98662b730099437011356fa77ef9072054f4ad73d3781e9b02d4750689762162`  
		Last Modified: Thu, 13 Oct 2022 23:21:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7e77f6a080ad6fa8a7320831868ccd7b6385e995988f2e6cca76090a565c99`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec71d29d036cab0bdbc7765216513aad527933ededfec4492a97724c6bab52d`  
		Last Modified: Thu, 13 Oct 2022 23:21:06 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a11bac4631094c366303dd3c571fe04cf1b543bafba72d8dd1030f8ae2ec185`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4dc588cdabd0672f8b29c59cd9ddc6d927160284a6f6529fbe39b8e34ca766`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f39777f21d48153f681f16b5a1cd2e12440066bc96a665fa3b85a6275b74942`  
		Last Modified: Thu, 13 Oct 2022 23:21:05 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638736df2ba6ceaed21b97ee12046d2d0494561bd735581618ab505ff602b0da`  
		Last Modified: Thu, 13 Oct 2022 23:21:04 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e0fe53dba785fdf61d7431392d7e15beeebbe5f215d9a2de2ee00975e7b5c4`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb7b8fc42485b0656b2afcb99344cda044ce10d0107cc91955fbe11433c358`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb8f166931be4f8f0b0a07611df01a8e7d1101f8a8ce564144ded43917e1021`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bc6f4b7a114b7722cfc81aa83b74727261766c2cef9bc0787e447435c33d2a`  
		Last Modified: Thu, 13 Oct 2022 23:21:03 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5563ab3963680a40da3bc2269bbc1e76362b359547dae9705892cf8f54b50dd1`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d300f0320cd2b8ce3f3e58cbb3acb06e24c5f59a342725056a10667329f914`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfb9dfa0b00914a255876439613219f4a74e83734df6b8a197e6e0bb53bf905`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b9233dbf203ca77eea2271813856d219ba7d2f633adf99f3262612edfad738`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 291.8 KB (291836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefde31b509f056641749adae4daa4e0ad3265d260ac1c61b41c8950a10824e6`  
		Last Modified: Thu, 13 Oct 2022 23:21:01 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:6a6b89102bf9584016d1a0364792d3cea05585c2fc057b4ffce271b8496a8bc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1129; amd64

### `caddy:windowsservercore-ltsc2022` - windows version 10.0.20348.1129; amd64

```console
$ docker pull caddy@sha256:e1e15c80e157d71221ec43035cae93b3ea8ba7a6b203428e93159aa6ff5e1463
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2432333411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbd806ca24dfacee0d098f111cc9f6d5f42fdbd9db91a63a8de0d048d3984d5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 17:01:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 13 Oct 2022 23:17:37 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 13 Oct 2022 23:18:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 13 Oct 2022 23:18:12 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 13 Oct 2022 23:18:13 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 13 Oct 2022 23:18:13 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 13 Oct 2022 23:18:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 13 Oct 2022 23:18:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 13 Oct 2022 23:18:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 13 Oct 2022 23:18:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 13 Oct 2022 23:18:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 13 Oct 2022 23:18:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 13 Oct 2022 23:18:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 13 Oct 2022 23:18:21 GMT
EXPOSE 80
# Thu, 13 Oct 2022 23:18:22 GMT
EXPOSE 443
# Thu, 13 Oct 2022 23:18:23 GMT
EXPOSE 443/udp
# Thu, 13 Oct 2022 23:18:24 GMT
EXPOSE 2019
# Thu, 13 Oct 2022 23:18:40 GMT
RUN caddy version
# Thu, 13 Oct 2022 23:18:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ab91661ce2a2a2c14684a2ba0f543a81d7896773f88200b31be0e37c589de38`  
		Size: 979.4 MB (979359717 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cd84a277fd91a008fe0c8fc7d6706544075a294512940b16f57998588ea892`  
		Last Modified: Wed, 12 Oct 2022 17:04:58 GMT  
		Size: 616.9 KB (616893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b069dfbedeca0437916f85fdd78a598955839b91ffc4cba4d6327e5c79487`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5263d846656ffa3662062b1a58d9c6d114e00fa5344edc9b93ea5895c4fa46`  
		Last Modified: Thu, 13 Oct 2022 23:21:34 GMT  
		Size: 15.1 MB (15149356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e378404d94c7fb280c51201d60aef05af3196a0ead3b716521cedbe766ba5e3e`  
		Last Modified: Thu, 13 Oct 2022 23:21:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11749bcf2c3e4097f9a1a30d1fc22184e48c94ab54945730c51c36be175c668d`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cb14f39fa0dce5d6dab4bdd1a896c02b5a6bba01dcd46ed36928c2cce27295`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf622a21cfc36d8958be2f273f52b7d4824d500be08f6a2de791506dcc6c981f`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b246af35953d05f1c4292cb1cf8cfc29215ceac2e013ae2a0759aa2d216516`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08367cd2562c20737156e692dca481f835f4832fabb63602fb5edc78494057ae`  
		Last Modified: Thu, 13 Oct 2022 23:21:29 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6d70510bf329eff739580f04b59acba9cb4aa74e57bcb6fca996d6df6b6d2c`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc6e963fa5949ceb99519a652299dea21a92c9389aadabedb2deeb4e51855b5`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d175d8244325a62c683c4d1fa6cc266f73231f93142fd0f52c3378da6db1464`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4ce9495075c9b00994ef154c9eb0974ba1853a8244869e35af4eecfca4dce7`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceee07aab1c573de692984f7655da9e6c4aee31260b8df8735344242e6f1ff8`  
		Last Modified: Thu, 13 Oct 2022 23:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295041dd24e85177aaf7e1bbd1c0b032d2eafaf3da59213972894238dd5b3d72`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3583f031f13dfd9a933b6e8d4808a3ac7f3e007d2e751af9581b76b08b6e0c4a`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1603973d06c7b0a01ab165d727b40f842361ce898a8e7b8579d6bd9db938c8a6`  
		Last Modified: Thu, 13 Oct 2022 23:21:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c4bf5f410b0a58ef5b477fdf99b90ad01e7deb85b685cf06eaae5c9d83a531`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 319.8 KB (319842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da4c854489e4317220200f8dca47e2335696fe8fa9e7a2aa678467b12b4db7b`  
		Last Modified: Thu, 13 Oct 2022 23:21:25 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
