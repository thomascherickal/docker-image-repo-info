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
$ docker pull caddy@sha256:50743fc6130295e9e8feccd8b2f437d8c472f626bf277dc873734ed98219f44f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3650; amd64
	-	windows version 10.0.20348.1249; amd64

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
$ docker pull caddy@sha256:b12b313a563011ab587b862567334b5f1e510002b8e013bc40af1ae4377e032d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16834898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48e1e3f680dff812573b72d098360058ddd668873bde28a22261f68c876822fa`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:27 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Thu, 10 Nov 2022 20:49:27 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:32:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 10 Nov 2022 21:32:43 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 10 Nov 2022 21:32:43 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 10 Nov 2022 21:32:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 10 Nov 2022 21:32:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:32:49 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 10 Nov 2022 21:32:49 GMT
ENV XDG_DATA_HOME=/data
# Thu, 10 Nov 2022 21:32:50 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 10 Nov 2022 21:32:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Nov 2022 21:32:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Nov 2022 21:32:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Nov 2022 21:32:52 GMT
EXPOSE 80
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 443
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 443/udp
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 2019
# Thu, 10 Nov 2022 21:32:54 GMT
WORKDIR /srv
# Thu, 10 Nov 2022 21:32:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6f07846270a9d34a7f4e9dda7d81a5b081ba30588b9e3486c62b5cdcbc1405`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 304.4 KB (304400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5465143f5f5b00ed906a73fc1ac3b86f9deaee0c21b275408cf309fef94a4041`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 5.8 KB (5754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47d9833dc35b7555f175e85c7c0fba471ad40d97a949f6b0f80bfc19605f383`  
		Last Modified: Thu, 10 Nov 2022 21:34:01 GMT  
		Size: 13.9 MB (13910625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662ebf5c4140b8798aa93a33fe7539f17a6eafc57111e615a4634561648b9e23`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a49a9fa13cf6792de98f5351389c9fdad662db85ca244483c7b515f2f1ed87d0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16617549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32dee3a3e8e899357be2b1b4428f62f334dec2af23a51967830b837e25ae896d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 06:34:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Nov 2022 06:34:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 11 Nov 2022 06:34:17 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 11 Nov 2022 06:34:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Nov 2022 06:34:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Nov 2022 06:34:20 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Nov 2022 06:34:20 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Nov 2022 06:34:21 GMT
EXPOSE 80
# Fri, 11 Nov 2022 06:34:21 GMT
EXPOSE 443
# Fri, 11 Nov 2022 06:34:22 GMT
EXPOSE 443/udp
# Fri, 11 Nov 2022 06:34:22 GMT
EXPOSE 2019
# Fri, 11 Nov 2022 06:34:22 GMT
WORKDIR /srv
# Fri, 11 Nov 2022 06:34:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ccfb174b467ecb8cc057263afb9939d1b3e15b9bc1c515179694d952fbf851`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 303.5 KB (303527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c1861352af6dba0e4cb99dd7060c884cd671d012e014dba05a612be38386a9`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 5.8 KB (5752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d37c36eede286e9554ac6d4beb0c577e4b2d285a0127336fefda6484662c65e`  
		Last Modified: Fri, 11 Nov 2022 06:35:23 GMT  
		Size: 13.9 MB (13891052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66529f6b32306fba04edbc38d87e496b1a1141951b2861b2be6fbd339dc40264`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:313fb401ecc2c6a4428f9abdcb87f7a3bd48769cbeca02e6e096d00b67329554
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16278672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c799e3816961c596d5c1fb50aae78395f4fd343fc77bf3122e0d396d510fe83`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Thu, 10 Nov 2022 20:39:41 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:30:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 10 Nov 2022 21:30:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 10 Nov 2022 21:30:10 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 10 Nov 2022 21:30:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 10 Nov 2022 21:30:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:30:12 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 10 Nov 2022 21:30:12 GMT
ENV XDG_DATA_HOME=/data
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 80
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 443
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 443/udp
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 2019
# Thu, 10 Nov 2022 21:30:14 GMT
WORKDIR /srv
# Thu, 10 Nov 2022 21:30:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480d8737fa00cd91dd0632e620ecb371ff8e7fbb7792619315f962bd74ac78b0`  
		Last Modified: Thu, 10 Nov 2022 21:30:38 GMT  
		Size: 304.5 KB (304513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8b251ca0b51f9a0e2defca59988fe0d152662e2a155d0861aa02e2a7257dd1`  
		Last Modified: Thu, 10 Nov 2022 21:30:38 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9543d07ca7897910ddae9b3fb026b4004353b71f3342f8889a2ecf194358ef65`  
		Last Modified: Thu, 10 Nov 2022 21:30:39 GMT  
		Size: 13.3 MB (13260509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e0320d2afc0181e222e9018c3ce159603f04d94ac7754b2c57e2a2f198a477`  
		Last Modified: Thu, 10 Nov 2022 21:30:37 GMT  
		Size: 154.0 B  
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

### `caddy:2` - windows version 10.0.17763.3650; amd64

```console
$ docker pull caddy@sha256:1bb072f445e9d5154311ff5502f598bc04f8f3a39962ba84935c924372254023
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2794246589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09e5adcd59d9a3cef6ebbe389ca4ba29c5fd69972ae3e411b8be53d7267ce1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:09:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:09:11 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:10:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:10:28 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:10:29 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:10:30 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:10:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:10:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:10:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:10:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:10:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:10:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:10:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:10:38 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:10:39 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:10:40 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:10:41 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:11:42 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:11:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c991125a18c41d60a99d6ec86c4c38917cda31bdc78ae2b19547118e64c3130`  
		Last Modified: Wed, 09 Nov 2022 19:42:43 GMT  
		Size: 376.0 KB (375983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c44dcec78b9053b83e9d2b0b85793a2d6dd9f7882eda9b68af412bfc561ae59`  
		Last Modified: Wed, 09 Nov 2022 19:42:42 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679594f71e58468aa9805558e75d701d34727227835b6f244c3227d0e8b3fc51`  
		Last Modified: Wed, 09 Nov 2022 19:42:45 GMT  
		Size: 15.0 MB (14954096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ec8fe5018705645312e2f15ddeff4193348e2d162b522e3d89004171e32611`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de52b8df46e754f4b7a96b07b9fcec10bba34c5203824f45ad667524e900442`  
		Last Modified: Wed, 09 Nov 2022 19:42:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de92b977c1ec3484f7ec22f1caf0af85a365785ef5a626cd1306e02ba2d78514`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14440e034f493a00a52bd65e46382b25e372630456a4bab3984ef60887bd4b2`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7fa7a9304ad99e65a0da0a731b88f220461e17a0a0aefd95e4388273c22107`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4688f22612a7a65254ccf95adb7b14eb333413e66689770a1b2ee648df6ae7a`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04f66e90a6de69b5c69c165ab290a0f792549149c911eef51f26380bdac82f2`  
		Last Modified: Wed, 09 Nov 2022 19:42:38 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a779763f5c2179feba42c73a1b4ac83edb90462493ee5b369908d6e839520f8`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d1d0c12a2c947c8a5a1942711ea238b6899cbbde6dc2d4c32401e2f336ebc5`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9267ecd850272decf95a74353e3505335d6ca458bd2d604cf6fd08f36b42b36d`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0daba2c50a467fa60cd066c4a707a46479815f75be8ccee29e3ffd74089e29c`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3399f861f6994eed02f962f0dfe8919ff2c59d392b5ee7cf1a2374a3e42892`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b97c99b6c4d5675b3327c5f3a35c918b75ab8fb154b22797764b4620b444c0`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634fc965a18e1d74efa1e1e64a43388feca61231913a4e4b3784b0955c81d4ec`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a7f978fb624cd5a777948f956d64e0e5688bd12864fc178bad1fa89cdf12f5`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 305.8 KB (305758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8494101343a0a636a7e1246e9ac5417edfd30766fa9cc3accad02c260ae99e3`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.20348.1249; amd64

```console
$ docker pull caddy@sha256:df26460add1714658ae82eb674ccba73fd3781a29eb1c742153d7f848ba77b03
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2497915476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf8cd6c30b11c2e211f77bf1bd355ab239d0405d001159b36bf501643b70145`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:12:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:12:22 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:12:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:12:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:12:51 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:12:52 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:12:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:12:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:12:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:12:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:12:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:12:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:12:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:13:00 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:13:01 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:13:18 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:13:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1dc6b6b8064ce6aa320f7658f5ddc1b7eafa5e7b7ed6eaa07e0d8a1c990256`  
		Last Modified: Wed, 09 Nov 2022 19:43:12 GMT  
		Size: 617.3 KB (617258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad0e2bc53452df09c89858e4b2f54e4b23c0c8bb58733f05d9b0b3a5f39b1e8`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa3455b7b8e4ed55199abb0ad62eea75ab0ab47616504b3758f35aed63ccbc8`  
		Last Modified: Wed, 09 Nov 2022 19:43:15 GMT  
		Size: 15.2 MB (15168482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d64bc11b8e88956f2cdb7f937525a2fb1c986000887f4dc88dc1eea98446d81`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8502309666e15b454660c5bfd9d1ebd352e18c945b8b2ede9afe9269a5937b`  
		Last Modified: Wed, 09 Nov 2022 19:43:10 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906c51626faa981aaf141adb1be3e8e65cbe12d592fa3c640dc829d28abd4d00`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ee5c1d8d0fd98304b819d90c4adb33feb485f3f47dcf390bee532f8d6b57f4`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63fc79d12f01d2fad54fd51f43571f0aaef608b2d7be31823c881667cb5e41e`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad24427c4c7dcb96616f4886c985d9252699bbaf01bb7f1551a776f57ac3080`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce3623edb8a858ba8a0f7f2184802487aa72c8332935270dbb0308fbbd70c0`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8180ccb35cb5b71974dc1c9130892b1c8ab0f20309906215682be61e553596c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b759234e6db3ee8b177b51b148eeb2a3ef89bc496e3098d56322d6e17a269f3c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc80653154d31f3fad6c8977be60b10618022311edaf9a0cba8a6eee3428aa1`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19a3de5a545f51fc5ee391f49dc670b30e5d6814b0bd8195075243d1d5d2d52`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d26ee259e1db29592ba9e5d679d72c081eab360aed0add981ddf4a44d7c7b2`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732e7368e5a0068535b80c136d98d840daeba6d9dd5d7fe90bb39b10c9fab27f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da48319bd36cb22c79804c6e3e5efa4abb652e22c993fe7a5c98efc0d651240f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8bd93b51837b04ade762d05a59d24ed1f68d2a4cd612020a5915736d43aa6f`  
		Last Modified: Wed, 09 Nov 2022 19:43:05 GMT  
		Size: 337.0 KB (336999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51903721c05174a5370399be9cfbcdfafdc616c28d0599d67308b9a44b07d5d9`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:25a0097607868fb05a89a5ab9fea2f2ea4cecdc89d887d7dcee8c778a21b9e1f
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
$ docker pull caddy@sha256:b12b313a563011ab587b862567334b5f1e510002b8e013bc40af1ae4377e032d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16834898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48e1e3f680dff812573b72d098360058ddd668873bde28a22261f68c876822fa`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:27 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Thu, 10 Nov 2022 20:49:27 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:32:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 10 Nov 2022 21:32:43 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 10 Nov 2022 21:32:43 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 10 Nov 2022 21:32:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 10 Nov 2022 21:32:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:32:49 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 10 Nov 2022 21:32:49 GMT
ENV XDG_DATA_HOME=/data
# Thu, 10 Nov 2022 21:32:50 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 10 Nov 2022 21:32:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Nov 2022 21:32:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Nov 2022 21:32:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Nov 2022 21:32:52 GMT
EXPOSE 80
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 443
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 443/udp
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 2019
# Thu, 10 Nov 2022 21:32:54 GMT
WORKDIR /srv
# Thu, 10 Nov 2022 21:32:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6f07846270a9d34a7f4e9dda7d81a5b081ba30588b9e3486c62b5cdcbc1405`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 304.4 KB (304400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5465143f5f5b00ed906a73fc1ac3b86f9deaee0c21b275408cf309fef94a4041`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 5.8 KB (5754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47d9833dc35b7555f175e85c7c0fba471ad40d97a949f6b0f80bfc19605f383`  
		Last Modified: Thu, 10 Nov 2022 21:34:01 GMT  
		Size: 13.9 MB (13910625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662ebf5c4140b8798aa93a33fe7539f17a6eafc57111e615a4634561648b9e23`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a49a9fa13cf6792de98f5351389c9fdad662db85ca244483c7b515f2f1ed87d0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16617549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32dee3a3e8e899357be2b1b4428f62f334dec2af23a51967830b837e25ae896d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 06:34:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Nov 2022 06:34:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 11 Nov 2022 06:34:17 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 11 Nov 2022 06:34:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Nov 2022 06:34:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Nov 2022 06:34:20 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Nov 2022 06:34:20 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Nov 2022 06:34:21 GMT
EXPOSE 80
# Fri, 11 Nov 2022 06:34:21 GMT
EXPOSE 443
# Fri, 11 Nov 2022 06:34:22 GMT
EXPOSE 443/udp
# Fri, 11 Nov 2022 06:34:22 GMT
EXPOSE 2019
# Fri, 11 Nov 2022 06:34:22 GMT
WORKDIR /srv
# Fri, 11 Nov 2022 06:34:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ccfb174b467ecb8cc057263afb9939d1b3e15b9bc1c515179694d952fbf851`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 303.5 KB (303527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c1861352af6dba0e4cb99dd7060c884cd671d012e014dba05a612be38386a9`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 5.8 KB (5752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d37c36eede286e9554ac6d4beb0c577e4b2d285a0127336fefda6484662c65e`  
		Last Modified: Fri, 11 Nov 2022 06:35:23 GMT  
		Size: 13.9 MB (13891052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66529f6b32306fba04edbc38d87e496b1a1141951b2861b2be6fbd339dc40264`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:313fb401ecc2c6a4428f9abdcb87f7a3bd48769cbeca02e6e096d00b67329554
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16278672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c799e3816961c596d5c1fb50aae78395f4fd343fc77bf3122e0d396d510fe83`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Thu, 10 Nov 2022 20:39:41 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:30:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 10 Nov 2022 21:30:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 10 Nov 2022 21:30:10 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 10 Nov 2022 21:30:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 10 Nov 2022 21:30:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:30:12 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 10 Nov 2022 21:30:12 GMT
ENV XDG_DATA_HOME=/data
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 80
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 443
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 443/udp
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 2019
# Thu, 10 Nov 2022 21:30:14 GMT
WORKDIR /srv
# Thu, 10 Nov 2022 21:30:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480d8737fa00cd91dd0632e620ecb371ff8e7fbb7792619315f962bd74ac78b0`  
		Last Modified: Thu, 10 Nov 2022 21:30:38 GMT  
		Size: 304.5 KB (304513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8b251ca0b51f9a0e2defca59988fe0d152662e2a155d0861aa02e2a7257dd1`  
		Last Modified: Thu, 10 Nov 2022 21:30:38 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9543d07ca7897910ddae9b3fb026b4004353b71f3342f8889a2ecf194358ef65`  
		Last Modified: Thu, 10 Nov 2022 21:30:39 GMT  
		Size: 13.3 MB (13260509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e0320d2afc0181e222e9018c3ce159603f04d94ac7754b2c57e2a2f198a477`  
		Last Modified: Thu, 10 Nov 2022 21:30:37 GMT  
		Size: 154.0 B  
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
$ docker pull caddy@sha256:1bfbc30b9fa0fe174661a0c039680b75fee83c3fdbeb8504faa1a4de574addce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3650; amd64
	-	windows version 10.0.20348.1249; amd64

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

### `caddy:2-builder` - windows version 10.0.17763.3650; amd64

```console
$ docker pull caddy@sha256:6cf653a2a7b8de4f339602e03c9c86540b02072e8b96e35878e007f769d7da16
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2963661660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cb2be08bd918187f9f5ad1fe999f73a7b423260e1205806377b8dc44e688751`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 13:56:03 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Nov 2022 13:56:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Nov 2022 13:56:05 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Nov 2022 13:56:06 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Nov 2022 13:57:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:57:58 GMT
ENV GOPATH=C:\go
# Wed, 09 Nov 2022 13:59:24 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Nov 2022 13:59:25 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 09 Nov 2022 14:03:31 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 14:03:33 GMT
WORKDIR C:\go
# Wed, 09 Nov 2022 18:13:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:13:29 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 09 Nov 2022 18:13:30 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:13:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Nov 2022 18:14:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Nov 2022 18:14:56 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a2b0ba4717890a5f71c35ff277f846f8f9b6668e0e7bb61c09c7be2ae6fa2b`  
		Last Modified: Wed, 09 Nov 2022 14:33:12 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ea601fe915f260a37aa95fd46906a58c4828c48a181f7fec434c255461bc3c`  
		Last Modified: Wed, 09 Nov 2022 14:33:07 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0a12f7377f09e1e60b8f98ba68c21900eb3bd8da74b27356717b7b531b1f19`  
		Last Modified: Wed, 09 Nov 2022 14:33:06 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96720d70c884dea5fd72c530b456770bdc779483b7f1d752e386360daffe6e4e`  
		Last Modified: Wed, 09 Nov 2022 14:33:06 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10a1ec572d19d510940ad8ddec14084b9e4d8300ef36b3ef50f23b477df789d`  
		Last Modified: Wed, 09 Nov 2022 14:33:16 GMT  
		Size: 25.5 MB (25457961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378cf1d27c9b1599652ca2d1c09cf3196ecbd22b40ee08813574a0fc119440d7`  
		Last Modified: Wed, 09 Nov 2022 14:33:04 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561cd622fdb3c0fabfcb202894dc24ba2a9491bf349e487be308fb6315c43c1d`  
		Last Modified: Wed, 09 Nov 2022 14:33:04 GMT  
		Size: 326.0 KB (326032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe2ec77bf4f0673d2620baa4e0302b768acebce02398e710036bf3f656c0ecc`  
		Last Modified: Wed, 09 Nov 2022 14:33:03 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eaf4d425600774d03d9f467838fe1b18d6a9460b749c91c1024aa8904b0e334`  
		Last Modified: Wed, 09 Nov 2022 14:33:58 GMT  
		Size: 157.6 MB (157648264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6413639a75ce7d233f32964ef57abd38fc992a742736bc7e7a163fa8aa5b4b0`  
		Last Modified: Wed, 09 Nov 2022 14:33:03 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614f1b9006d1823d89a42263057e769283383c54144a3dc50d4ea64dec74b5c7`  
		Last Modified: Wed, 09 Nov 2022 19:43:36 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184c91cb508dbf30520922b855e98043d4c3ea2479805b179085847628631e9b`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5127f06a739ff0fd5c240314901aa7fc16f2c5c55c07d10ab007bc1a4b1364dc`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b199d92416df53de1551d66e029f372db1c76a2afe75ea4afa7288ca8a3ab775`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbce37404bc1695c1f7d35e9732764388cfbd8391f96cf201053cb30562029fe`  
		Last Modified: Wed, 09 Nov 2022 19:43:34 GMT  
		Size: 1.6 MB (1624203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ed8f4a92cb5e13a8092652093226fe12e30e288d191f6b727f7fd79c9ad414`  
		Last Modified: Wed, 09 Nov 2022 19:43:34 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.20348.1249; amd64

```console
$ docker pull caddy@sha256:9ed32ae59f8639230dc09e89512d25258e2550fcf519495c20c1e2622b311772
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2667713878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aa94e32ea39d538bc848f49a88694ed5bff88005fcd74e8700db5a7e7befaee`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 13:51:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Nov 2022 13:51:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Nov 2022 13:51:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Nov 2022 13:51:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Nov 2022 13:52:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:52:12 GMT
ENV GOPATH=C:\go
# Wed, 09 Nov 2022 13:52:36 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Nov 2022 13:52:37 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 09 Nov 2022 13:55:50 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:55:52 GMT
WORKDIR C:\go
# Wed, 09 Nov 2022 18:15:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:15:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 09 Nov 2022 18:15:15 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:15:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Nov 2022 18:15:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Nov 2022 18:15:45 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea79272e8d2a572a4d212450946bce415296eae87b6ce74df5b622cdfee02c67`  
		Last Modified: Wed, 09 Nov 2022 14:31:56 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a776f73cd30b265202025b98515575e21f757c88c6361190224cf46c2b7d1d`  
		Last Modified: Wed, 09 Nov 2022 14:31:53 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5268ccf7578edb6ae20eccf50b8be8c8da75b9054711b531062a365dc4fdca4`  
		Last Modified: Wed, 09 Nov 2022 14:31:52 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c9e4ebbf21dbe0a28faabe67fd74fca79784fefc03a56fae2e25366742aa37`  
		Last Modified: Wed, 09 Nov 2022 14:31:51 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671be4304252589ad8fea639a28234c14a6aeab6a0913d98704928824b355f28`  
		Last Modified: Wed, 09 Nov 2022 14:32:01 GMT  
		Size: 25.7 MB (25693161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131c64f4139ebfed8185c51abad4bbb44ad9830a76a221307d83acc03b579f2e`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceec23424e6d501387ce0ab8f96b2349ac91551e8ff768a658f97eb07430e76`  
		Last Modified: Wed, 09 Nov 2022 14:31:49 GMT  
		Size: 548.2 KB (548156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9475cb31b9e6aa94b3c8bac11dad0e1d052709c8d931bf0ae9373371ad4d7bf`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f00ac483de739170f945938526dd868499e135b2661edf64b64a35e533d0ae`  
		Last Modified: Wed, 09 Nov 2022 14:32:45 GMT  
		Size: 157.8 MB (157844340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973945315f37c2cee022dc1f6b25fe2d420fa96edd876cad28a507515f40c18d`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.6 KB (1589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b243f67c60aae1519ab6b4211d6746d958ebdaded4297ea7378794c35d8683`  
		Last Modified: Wed, 09 Nov 2022 19:43:58 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd79a73ed810cffb30c91e80d20bf903af3dea7476f04d503d7051f1bdbe2be4`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd66ad327482a3d8d053309d10877a72859caaef7ed99c3841bf985c63d8164e`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c37cb6737d74657ec2c98ddb8bfaf994aa881104b47b2a3230edc36f93fe9f`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aef28670eb8e61758e89572ed759fc8b57fe8f1e3d40c8021cf21e0c80f3103`  
		Last Modified: Wed, 09 Nov 2022 19:43:57 GMT  
		Size: 1.8 MB (1841412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f961cc28a480ceb15a0e0c07284ecb8e251842282e48ee1695adb121939e3c`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1422 bytes)  
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
$ docker pull caddy@sha256:ed2c53e8bf858c413d1112ec78dad49683b6963cb6a6d43a02d3877afee50eb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull caddy@sha256:6cf653a2a7b8de4f339602e03c9c86540b02072e8b96e35878e007f769d7da16
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2963661660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cb2be08bd918187f9f5ad1fe999f73a7b423260e1205806377b8dc44e688751`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 13:56:03 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Nov 2022 13:56:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Nov 2022 13:56:05 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Nov 2022 13:56:06 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Nov 2022 13:57:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:57:58 GMT
ENV GOPATH=C:\go
# Wed, 09 Nov 2022 13:59:24 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Nov 2022 13:59:25 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 09 Nov 2022 14:03:31 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 14:03:33 GMT
WORKDIR C:\go
# Wed, 09 Nov 2022 18:13:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:13:29 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 09 Nov 2022 18:13:30 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:13:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Nov 2022 18:14:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Nov 2022 18:14:56 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a2b0ba4717890a5f71c35ff277f846f8f9b6668e0e7bb61c09c7be2ae6fa2b`  
		Last Modified: Wed, 09 Nov 2022 14:33:12 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ea601fe915f260a37aa95fd46906a58c4828c48a181f7fec434c255461bc3c`  
		Last Modified: Wed, 09 Nov 2022 14:33:07 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0a12f7377f09e1e60b8f98ba68c21900eb3bd8da74b27356717b7b531b1f19`  
		Last Modified: Wed, 09 Nov 2022 14:33:06 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96720d70c884dea5fd72c530b456770bdc779483b7f1d752e386360daffe6e4e`  
		Last Modified: Wed, 09 Nov 2022 14:33:06 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10a1ec572d19d510940ad8ddec14084b9e4d8300ef36b3ef50f23b477df789d`  
		Last Modified: Wed, 09 Nov 2022 14:33:16 GMT  
		Size: 25.5 MB (25457961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378cf1d27c9b1599652ca2d1c09cf3196ecbd22b40ee08813574a0fc119440d7`  
		Last Modified: Wed, 09 Nov 2022 14:33:04 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561cd622fdb3c0fabfcb202894dc24ba2a9491bf349e487be308fb6315c43c1d`  
		Last Modified: Wed, 09 Nov 2022 14:33:04 GMT  
		Size: 326.0 KB (326032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe2ec77bf4f0673d2620baa4e0302b768acebce02398e710036bf3f656c0ecc`  
		Last Modified: Wed, 09 Nov 2022 14:33:03 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eaf4d425600774d03d9f467838fe1b18d6a9460b749c91c1024aa8904b0e334`  
		Last Modified: Wed, 09 Nov 2022 14:33:58 GMT  
		Size: 157.6 MB (157648264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6413639a75ce7d233f32964ef57abd38fc992a742736bc7e7a163fa8aa5b4b0`  
		Last Modified: Wed, 09 Nov 2022 14:33:03 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614f1b9006d1823d89a42263057e769283383c54144a3dc50d4ea64dec74b5c7`  
		Last Modified: Wed, 09 Nov 2022 19:43:36 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184c91cb508dbf30520922b855e98043d4c3ea2479805b179085847628631e9b`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5127f06a739ff0fd5c240314901aa7fc16f2c5c55c07d10ab007bc1a4b1364dc`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b199d92416df53de1551d66e029f372db1c76a2afe75ea4afa7288ca8a3ab775`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbce37404bc1695c1f7d35e9732764388cfbd8391f96cf201053cb30562029fe`  
		Last Modified: Wed, 09 Nov 2022 19:43:34 GMT  
		Size: 1.6 MB (1624203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ed8f4a92cb5e13a8092652093226fe12e30e288d191f6b727f7fd79c9ad414`  
		Last Modified: Wed, 09 Nov 2022 19:43:34 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:8f08b39d3c846f5fe51158683dd4062da0fed911c1d6a09f372c510316df9486
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1249; amd64

### `caddy:2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1249; amd64

```console
$ docker pull caddy@sha256:9ed32ae59f8639230dc09e89512d25258e2550fcf519495c20c1e2622b311772
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2667713878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aa94e32ea39d538bc848f49a88694ed5bff88005fcd74e8700db5a7e7befaee`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 13:51:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Nov 2022 13:51:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Nov 2022 13:51:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Nov 2022 13:51:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Nov 2022 13:52:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:52:12 GMT
ENV GOPATH=C:\go
# Wed, 09 Nov 2022 13:52:36 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Nov 2022 13:52:37 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 09 Nov 2022 13:55:50 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:55:52 GMT
WORKDIR C:\go
# Wed, 09 Nov 2022 18:15:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:15:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 09 Nov 2022 18:15:15 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:15:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Nov 2022 18:15:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Nov 2022 18:15:45 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea79272e8d2a572a4d212450946bce415296eae87b6ce74df5b622cdfee02c67`  
		Last Modified: Wed, 09 Nov 2022 14:31:56 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a776f73cd30b265202025b98515575e21f757c88c6361190224cf46c2b7d1d`  
		Last Modified: Wed, 09 Nov 2022 14:31:53 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5268ccf7578edb6ae20eccf50b8be8c8da75b9054711b531062a365dc4fdca4`  
		Last Modified: Wed, 09 Nov 2022 14:31:52 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c9e4ebbf21dbe0a28faabe67fd74fca79784fefc03a56fae2e25366742aa37`  
		Last Modified: Wed, 09 Nov 2022 14:31:51 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671be4304252589ad8fea639a28234c14a6aeab6a0913d98704928824b355f28`  
		Last Modified: Wed, 09 Nov 2022 14:32:01 GMT  
		Size: 25.7 MB (25693161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131c64f4139ebfed8185c51abad4bbb44ad9830a76a221307d83acc03b579f2e`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceec23424e6d501387ce0ab8f96b2349ac91551e8ff768a658f97eb07430e76`  
		Last Modified: Wed, 09 Nov 2022 14:31:49 GMT  
		Size: 548.2 KB (548156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9475cb31b9e6aa94b3c8bac11dad0e1d052709c8d931bf0ae9373371ad4d7bf`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f00ac483de739170f945938526dd868499e135b2661edf64b64a35e533d0ae`  
		Last Modified: Wed, 09 Nov 2022 14:32:45 GMT  
		Size: 157.8 MB (157844340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973945315f37c2cee022dc1f6b25fe2d420fa96edd876cad28a507515f40c18d`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.6 KB (1589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b243f67c60aae1519ab6b4211d6746d958ebdaded4297ea7378794c35d8683`  
		Last Modified: Wed, 09 Nov 2022 19:43:58 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd79a73ed810cffb30c91e80d20bf903af3dea7476f04d503d7051f1bdbe2be4`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd66ad327482a3d8d053309d10877a72859caaef7ed99c3841bf985c63d8164e`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c37cb6737d74657ec2c98ddb8bfaf994aa881104b47b2a3230edc36f93fe9f`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aef28670eb8e61758e89572ed759fc8b57fe8f1e3d40c8021cf21e0c80f3103`  
		Last Modified: Wed, 09 Nov 2022 19:43:57 GMT  
		Size: 1.8 MB (1841412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f961cc28a480ceb15a0e0c07284ecb8e251842282e48ee1695adb121939e3c`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:0a8af8e78d210109370f648e45b709e478abcdb65b491151144dc00c66fa5d39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3650; amd64
	-	windows version 10.0.20348.1249; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.3650; amd64

```console
$ docker pull caddy@sha256:1bb072f445e9d5154311ff5502f598bc04f8f3a39962ba84935c924372254023
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2794246589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09e5adcd59d9a3cef6ebbe389ca4ba29c5fd69972ae3e411b8be53d7267ce1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:09:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:09:11 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:10:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:10:28 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:10:29 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:10:30 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:10:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:10:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:10:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:10:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:10:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:10:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:10:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:10:38 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:10:39 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:10:40 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:10:41 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:11:42 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:11:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c991125a18c41d60a99d6ec86c4c38917cda31bdc78ae2b19547118e64c3130`  
		Last Modified: Wed, 09 Nov 2022 19:42:43 GMT  
		Size: 376.0 KB (375983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c44dcec78b9053b83e9d2b0b85793a2d6dd9f7882eda9b68af412bfc561ae59`  
		Last Modified: Wed, 09 Nov 2022 19:42:42 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679594f71e58468aa9805558e75d701d34727227835b6f244c3227d0e8b3fc51`  
		Last Modified: Wed, 09 Nov 2022 19:42:45 GMT  
		Size: 15.0 MB (14954096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ec8fe5018705645312e2f15ddeff4193348e2d162b522e3d89004171e32611`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de52b8df46e754f4b7a96b07b9fcec10bba34c5203824f45ad667524e900442`  
		Last Modified: Wed, 09 Nov 2022 19:42:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de92b977c1ec3484f7ec22f1caf0af85a365785ef5a626cd1306e02ba2d78514`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14440e034f493a00a52bd65e46382b25e372630456a4bab3984ef60887bd4b2`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7fa7a9304ad99e65a0da0a731b88f220461e17a0a0aefd95e4388273c22107`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4688f22612a7a65254ccf95adb7b14eb333413e66689770a1b2ee648df6ae7a`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04f66e90a6de69b5c69c165ab290a0f792549149c911eef51f26380bdac82f2`  
		Last Modified: Wed, 09 Nov 2022 19:42:38 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a779763f5c2179feba42c73a1b4ac83edb90462493ee5b369908d6e839520f8`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d1d0c12a2c947c8a5a1942711ea238b6899cbbde6dc2d4c32401e2f336ebc5`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9267ecd850272decf95a74353e3505335d6ca458bd2d604cf6fd08f36b42b36d`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0daba2c50a467fa60cd066c4a707a46479815f75be8ccee29e3ffd74089e29c`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3399f861f6994eed02f962f0dfe8919ff2c59d392b5ee7cf1a2374a3e42892`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b97c99b6c4d5675b3327c5f3a35c918b75ab8fb154b22797764b4620b444c0`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634fc965a18e1d74efa1e1e64a43388feca61231913a4e4b3784b0955c81d4ec`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a7f978fb624cd5a777948f956d64e0e5688bd12864fc178bad1fa89cdf12f5`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 305.8 KB (305758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8494101343a0a636a7e1246e9ac5417edfd30766fa9cc3accad02c260ae99e3`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.20348.1249; amd64

```console
$ docker pull caddy@sha256:df26460add1714658ae82eb674ccba73fd3781a29eb1c742153d7f848ba77b03
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2497915476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf8cd6c30b11c2e211f77bf1bd355ab239d0405d001159b36bf501643b70145`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:12:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:12:22 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:12:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:12:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:12:51 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:12:52 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:12:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:12:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:12:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:12:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:12:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:12:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:12:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:13:00 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:13:01 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:13:18 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:13:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1dc6b6b8064ce6aa320f7658f5ddc1b7eafa5e7b7ed6eaa07e0d8a1c990256`  
		Last Modified: Wed, 09 Nov 2022 19:43:12 GMT  
		Size: 617.3 KB (617258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad0e2bc53452df09c89858e4b2f54e4b23c0c8bb58733f05d9b0b3a5f39b1e8`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa3455b7b8e4ed55199abb0ad62eea75ab0ab47616504b3758f35aed63ccbc8`  
		Last Modified: Wed, 09 Nov 2022 19:43:15 GMT  
		Size: 15.2 MB (15168482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d64bc11b8e88956f2cdb7f937525a2fb1c986000887f4dc88dc1eea98446d81`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8502309666e15b454660c5bfd9d1ebd352e18c945b8b2ede9afe9269a5937b`  
		Last Modified: Wed, 09 Nov 2022 19:43:10 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906c51626faa981aaf141adb1be3e8e65cbe12d592fa3c640dc829d28abd4d00`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ee5c1d8d0fd98304b819d90c4adb33feb485f3f47dcf390bee532f8d6b57f4`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63fc79d12f01d2fad54fd51f43571f0aaef608b2d7be31823c881667cb5e41e`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad24427c4c7dcb96616f4886c985d9252699bbaf01bb7f1551a776f57ac3080`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce3623edb8a858ba8a0f7f2184802487aa72c8332935270dbb0308fbbd70c0`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8180ccb35cb5b71974dc1c9130892b1c8ab0f20309906215682be61e553596c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b759234e6db3ee8b177b51b148eeb2a3ef89bc496e3098d56322d6e17a269f3c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc80653154d31f3fad6c8977be60b10618022311edaf9a0cba8a6eee3428aa1`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19a3de5a545f51fc5ee391f49dc670b30e5d6814b0bd8195075243d1d5d2d52`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d26ee259e1db29592ba9e5d679d72c081eab360aed0add981ddf4a44d7c7b2`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732e7368e5a0068535b80c136d98d840daeba6d9dd5d7fe90bb39b10c9fab27f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da48319bd36cb22c79804c6e3e5efa4abb652e22c993fe7a5c98efc0d651240f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8bd93b51837b04ade762d05a59d24ed1f68d2a4cd612020a5915736d43aa6f`  
		Last Modified: Wed, 09 Nov 2022 19:43:05 GMT  
		Size: 337.0 KB (336999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51903721c05174a5370399be9cfbcdfafdc616c28d0599d67308b9a44b07d5d9`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:7d8fa3f8a84211c6129b53d25df161f198e739bb5f6e676467db0eafca8cda29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull caddy@sha256:1bb072f445e9d5154311ff5502f598bc04f8f3a39962ba84935c924372254023
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2794246589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09e5adcd59d9a3cef6ebbe389ca4ba29c5fd69972ae3e411b8be53d7267ce1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:09:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:09:11 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:10:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:10:28 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:10:29 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:10:30 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:10:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:10:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:10:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:10:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:10:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:10:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:10:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:10:38 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:10:39 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:10:40 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:10:41 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:11:42 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:11:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c991125a18c41d60a99d6ec86c4c38917cda31bdc78ae2b19547118e64c3130`  
		Last Modified: Wed, 09 Nov 2022 19:42:43 GMT  
		Size: 376.0 KB (375983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c44dcec78b9053b83e9d2b0b85793a2d6dd9f7882eda9b68af412bfc561ae59`  
		Last Modified: Wed, 09 Nov 2022 19:42:42 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679594f71e58468aa9805558e75d701d34727227835b6f244c3227d0e8b3fc51`  
		Last Modified: Wed, 09 Nov 2022 19:42:45 GMT  
		Size: 15.0 MB (14954096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ec8fe5018705645312e2f15ddeff4193348e2d162b522e3d89004171e32611`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de52b8df46e754f4b7a96b07b9fcec10bba34c5203824f45ad667524e900442`  
		Last Modified: Wed, 09 Nov 2022 19:42:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de92b977c1ec3484f7ec22f1caf0af85a365785ef5a626cd1306e02ba2d78514`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14440e034f493a00a52bd65e46382b25e372630456a4bab3984ef60887bd4b2`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7fa7a9304ad99e65a0da0a731b88f220461e17a0a0aefd95e4388273c22107`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4688f22612a7a65254ccf95adb7b14eb333413e66689770a1b2ee648df6ae7a`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04f66e90a6de69b5c69c165ab290a0f792549149c911eef51f26380bdac82f2`  
		Last Modified: Wed, 09 Nov 2022 19:42:38 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a779763f5c2179feba42c73a1b4ac83edb90462493ee5b369908d6e839520f8`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d1d0c12a2c947c8a5a1942711ea238b6899cbbde6dc2d4c32401e2f336ebc5`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9267ecd850272decf95a74353e3505335d6ca458bd2d604cf6fd08f36b42b36d`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0daba2c50a467fa60cd066c4a707a46479815f75be8ccee29e3ffd74089e29c`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3399f861f6994eed02f962f0dfe8919ff2c59d392b5ee7cf1a2374a3e42892`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b97c99b6c4d5675b3327c5f3a35c918b75ab8fb154b22797764b4620b444c0`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634fc965a18e1d74efa1e1e64a43388feca61231913a4e4b3784b0955c81d4ec`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a7f978fb624cd5a777948f956d64e0e5688bd12864fc178bad1fa89cdf12f5`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 305.8 KB (305758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8494101343a0a636a7e1246e9ac5417edfd30766fa9cc3accad02c260ae99e3`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:618d9f501fb56f3d12f4566a58de1afafc1a3920ba686c84cc2e1134d1bf41e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1249; amd64

### `caddy:2-windowsservercore-ltsc2022` - windows version 10.0.20348.1249; amd64

```console
$ docker pull caddy@sha256:df26460add1714658ae82eb674ccba73fd3781a29eb1c742153d7f848ba77b03
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2497915476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf8cd6c30b11c2e211f77bf1bd355ab239d0405d001159b36bf501643b70145`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:12:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:12:22 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:12:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:12:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:12:51 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:12:52 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:12:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:12:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:12:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:12:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:12:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:12:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:12:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:13:00 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:13:01 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:13:18 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:13:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1dc6b6b8064ce6aa320f7658f5ddc1b7eafa5e7b7ed6eaa07e0d8a1c990256`  
		Last Modified: Wed, 09 Nov 2022 19:43:12 GMT  
		Size: 617.3 KB (617258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad0e2bc53452df09c89858e4b2f54e4b23c0c8bb58733f05d9b0b3a5f39b1e8`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa3455b7b8e4ed55199abb0ad62eea75ab0ab47616504b3758f35aed63ccbc8`  
		Last Modified: Wed, 09 Nov 2022 19:43:15 GMT  
		Size: 15.2 MB (15168482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d64bc11b8e88956f2cdb7f937525a2fb1c986000887f4dc88dc1eea98446d81`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8502309666e15b454660c5bfd9d1ebd352e18c945b8b2ede9afe9269a5937b`  
		Last Modified: Wed, 09 Nov 2022 19:43:10 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906c51626faa981aaf141adb1be3e8e65cbe12d592fa3c640dc829d28abd4d00`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ee5c1d8d0fd98304b819d90c4adb33feb485f3f47dcf390bee532f8d6b57f4`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63fc79d12f01d2fad54fd51f43571f0aaef608b2d7be31823c881667cb5e41e`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad24427c4c7dcb96616f4886c985d9252699bbaf01bb7f1551a776f57ac3080`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce3623edb8a858ba8a0f7f2184802487aa72c8332935270dbb0308fbbd70c0`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8180ccb35cb5b71974dc1c9130892b1c8ab0f20309906215682be61e553596c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b759234e6db3ee8b177b51b148eeb2a3ef89bc496e3098d56322d6e17a269f3c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc80653154d31f3fad6c8977be60b10618022311edaf9a0cba8a6eee3428aa1`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19a3de5a545f51fc5ee391f49dc670b30e5d6814b0bd8195075243d1d5d2d52`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d26ee259e1db29592ba9e5d679d72c081eab360aed0add981ddf4a44d7c7b2`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732e7368e5a0068535b80c136d98d840daeba6d9dd5d7fe90bb39b10c9fab27f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da48319bd36cb22c79804c6e3e5efa4abb652e22c993fe7a5c98efc0d651240f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8bd93b51837b04ade762d05a59d24ed1f68d2a4cd612020a5915736d43aa6f`  
		Last Modified: Wed, 09 Nov 2022 19:43:05 GMT  
		Size: 337.0 KB (336999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51903721c05174a5370399be9cfbcdfafdc616c28d0599d67308b9a44b07d5d9`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6`

```console
$ docker pull caddy@sha256:50743fc6130295e9e8feccd8b2f437d8c472f626bf277dc873734ed98219f44f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3650; amd64
	-	windows version 10.0.20348.1249; amd64

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
$ docker pull caddy@sha256:b12b313a563011ab587b862567334b5f1e510002b8e013bc40af1ae4377e032d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16834898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48e1e3f680dff812573b72d098360058ddd668873bde28a22261f68c876822fa`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:27 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Thu, 10 Nov 2022 20:49:27 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:32:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 10 Nov 2022 21:32:43 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 10 Nov 2022 21:32:43 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 10 Nov 2022 21:32:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 10 Nov 2022 21:32:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:32:49 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 10 Nov 2022 21:32:49 GMT
ENV XDG_DATA_HOME=/data
# Thu, 10 Nov 2022 21:32:50 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 10 Nov 2022 21:32:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Nov 2022 21:32:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Nov 2022 21:32:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Nov 2022 21:32:52 GMT
EXPOSE 80
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 443
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 443/udp
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 2019
# Thu, 10 Nov 2022 21:32:54 GMT
WORKDIR /srv
# Thu, 10 Nov 2022 21:32:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6f07846270a9d34a7f4e9dda7d81a5b081ba30588b9e3486c62b5cdcbc1405`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 304.4 KB (304400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5465143f5f5b00ed906a73fc1ac3b86f9deaee0c21b275408cf309fef94a4041`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 5.8 KB (5754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47d9833dc35b7555f175e85c7c0fba471ad40d97a949f6b0f80bfc19605f383`  
		Last Modified: Thu, 10 Nov 2022 21:34:01 GMT  
		Size: 13.9 MB (13910625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662ebf5c4140b8798aa93a33fe7539f17a6eafc57111e615a4634561648b9e23`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a49a9fa13cf6792de98f5351389c9fdad662db85ca244483c7b515f2f1ed87d0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16617549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32dee3a3e8e899357be2b1b4428f62f334dec2af23a51967830b837e25ae896d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 06:34:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Nov 2022 06:34:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 11 Nov 2022 06:34:17 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 11 Nov 2022 06:34:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Nov 2022 06:34:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Nov 2022 06:34:20 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Nov 2022 06:34:20 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Nov 2022 06:34:21 GMT
EXPOSE 80
# Fri, 11 Nov 2022 06:34:21 GMT
EXPOSE 443
# Fri, 11 Nov 2022 06:34:22 GMT
EXPOSE 443/udp
# Fri, 11 Nov 2022 06:34:22 GMT
EXPOSE 2019
# Fri, 11 Nov 2022 06:34:22 GMT
WORKDIR /srv
# Fri, 11 Nov 2022 06:34:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ccfb174b467ecb8cc057263afb9939d1b3e15b9bc1c515179694d952fbf851`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 303.5 KB (303527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c1861352af6dba0e4cb99dd7060c884cd671d012e014dba05a612be38386a9`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 5.8 KB (5752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d37c36eede286e9554ac6d4beb0c577e4b2d285a0127336fefda6484662c65e`  
		Last Modified: Fri, 11 Nov 2022 06:35:23 GMT  
		Size: 13.9 MB (13891052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66529f6b32306fba04edbc38d87e496b1a1141951b2861b2be6fbd339dc40264`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:313fb401ecc2c6a4428f9abdcb87f7a3bd48769cbeca02e6e096d00b67329554
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16278672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c799e3816961c596d5c1fb50aae78395f4fd343fc77bf3122e0d396d510fe83`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Thu, 10 Nov 2022 20:39:41 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:30:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 10 Nov 2022 21:30:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 10 Nov 2022 21:30:10 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 10 Nov 2022 21:30:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 10 Nov 2022 21:30:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:30:12 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 10 Nov 2022 21:30:12 GMT
ENV XDG_DATA_HOME=/data
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 80
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 443
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 443/udp
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 2019
# Thu, 10 Nov 2022 21:30:14 GMT
WORKDIR /srv
# Thu, 10 Nov 2022 21:30:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480d8737fa00cd91dd0632e620ecb371ff8e7fbb7792619315f962bd74ac78b0`  
		Last Modified: Thu, 10 Nov 2022 21:30:38 GMT  
		Size: 304.5 KB (304513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8b251ca0b51f9a0e2defca59988fe0d152662e2a155d0861aa02e2a7257dd1`  
		Last Modified: Thu, 10 Nov 2022 21:30:38 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9543d07ca7897910ddae9b3fb026b4004353b71f3342f8889a2ecf194358ef65`  
		Last Modified: Thu, 10 Nov 2022 21:30:39 GMT  
		Size: 13.3 MB (13260509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e0320d2afc0181e222e9018c3ce159603f04d94ac7754b2c57e2a2f198a477`  
		Last Modified: Thu, 10 Nov 2022 21:30:37 GMT  
		Size: 154.0 B  
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

### `caddy:2.6` - windows version 10.0.17763.3650; amd64

```console
$ docker pull caddy@sha256:1bb072f445e9d5154311ff5502f598bc04f8f3a39962ba84935c924372254023
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2794246589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09e5adcd59d9a3cef6ebbe389ca4ba29c5fd69972ae3e411b8be53d7267ce1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:09:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:09:11 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:10:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:10:28 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:10:29 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:10:30 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:10:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:10:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:10:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:10:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:10:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:10:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:10:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:10:38 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:10:39 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:10:40 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:10:41 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:11:42 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:11:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c991125a18c41d60a99d6ec86c4c38917cda31bdc78ae2b19547118e64c3130`  
		Last Modified: Wed, 09 Nov 2022 19:42:43 GMT  
		Size: 376.0 KB (375983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c44dcec78b9053b83e9d2b0b85793a2d6dd9f7882eda9b68af412bfc561ae59`  
		Last Modified: Wed, 09 Nov 2022 19:42:42 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679594f71e58468aa9805558e75d701d34727227835b6f244c3227d0e8b3fc51`  
		Last Modified: Wed, 09 Nov 2022 19:42:45 GMT  
		Size: 15.0 MB (14954096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ec8fe5018705645312e2f15ddeff4193348e2d162b522e3d89004171e32611`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de52b8df46e754f4b7a96b07b9fcec10bba34c5203824f45ad667524e900442`  
		Last Modified: Wed, 09 Nov 2022 19:42:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de92b977c1ec3484f7ec22f1caf0af85a365785ef5a626cd1306e02ba2d78514`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14440e034f493a00a52bd65e46382b25e372630456a4bab3984ef60887bd4b2`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7fa7a9304ad99e65a0da0a731b88f220461e17a0a0aefd95e4388273c22107`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4688f22612a7a65254ccf95adb7b14eb333413e66689770a1b2ee648df6ae7a`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04f66e90a6de69b5c69c165ab290a0f792549149c911eef51f26380bdac82f2`  
		Last Modified: Wed, 09 Nov 2022 19:42:38 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a779763f5c2179feba42c73a1b4ac83edb90462493ee5b369908d6e839520f8`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d1d0c12a2c947c8a5a1942711ea238b6899cbbde6dc2d4c32401e2f336ebc5`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9267ecd850272decf95a74353e3505335d6ca458bd2d604cf6fd08f36b42b36d`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0daba2c50a467fa60cd066c4a707a46479815f75be8ccee29e3ffd74089e29c`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3399f861f6994eed02f962f0dfe8919ff2c59d392b5ee7cf1a2374a3e42892`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b97c99b6c4d5675b3327c5f3a35c918b75ab8fb154b22797764b4620b444c0`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634fc965a18e1d74efa1e1e64a43388feca61231913a4e4b3784b0955c81d4ec`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a7f978fb624cd5a777948f956d64e0e5688bd12864fc178bad1fa89cdf12f5`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 305.8 KB (305758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8494101343a0a636a7e1246e9ac5417edfd30766fa9cc3accad02c260ae99e3`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - windows version 10.0.20348.1249; amd64

```console
$ docker pull caddy@sha256:df26460add1714658ae82eb674ccba73fd3781a29eb1c742153d7f848ba77b03
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2497915476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf8cd6c30b11c2e211f77bf1bd355ab239d0405d001159b36bf501643b70145`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:12:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:12:22 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:12:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:12:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:12:51 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:12:52 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:12:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:12:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:12:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:12:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:12:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:12:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:12:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:13:00 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:13:01 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:13:18 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:13:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1dc6b6b8064ce6aa320f7658f5ddc1b7eafa5e7b7ed6eaa07e0d8a1c990256`  
		Last Modified: Wed, 09 Nov 2022 19:43:12 GMT  
		Size: 617.3 KB (617258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad0e2bc53452df09c89858e4b2f54e4b23c0c8bb58733f05d9b0b3a5f39b1e8`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa3455b7b8e4ed55199abb0ad62eea75ab0ab47616504b3758f35aed63ccbc8`  
		Last Modified: Wed, 09 Nov 2022 19:43:15 GMT  
		Size: 15.2 MB (15168482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d64bc11b8e88956f2cdb7f937525a2fb1c986000887f4dc88dc1eea98446d81`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8502309666e15b454660c5bfd9d1ebd352e18c945b8b2ede9afe9269a5937b`  
		Last Modified: Wed, 09 Nov 2022 19:43:10 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906c51626faa981aaf141adb1be3e8e65cbe12d592fa3c640dc829d28abd4d00`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ee5c1d8d0fd98304b819d90c4adb33feb485f3f47dcf390bee532f8d6b57f4`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63fc79d12f01d2fad54fd51f43571f0aaef608b2d7be31823c881667cb5e41e`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad24427c4c7dcb96616f4886c985d9252699bbaf01bb7f1551a776f57ac3080`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce3623edb8a858ba8a0f7f2184802487aa72c8332935270dbb0308fbbd70c0`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8180ccb35cb5b71974dc1c9130892b1c8ab0f20309906215682be61e553596c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b759234e6db3ee8b177b51b148eeb2a3ef89bc496e3098d56322d6e17a269f3c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc80653154d31f3fad6c8977be60b10618022311edaf9a0cba8a6eee3428aa1`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19a3de5a545f51fc5ee391f49dc670b30e5d6814b0bd8195075243d1d5d2d52`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d26ee259e1db29592ba9e5d679d72c081eab360aed0add981ddf4a44d7c7b2`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732e7368e5a0068535b80c136d98d840daeba6d9dd5d7fe90bb39b10c9fab27f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da48319bd36cb22c79804c6e3e5efa4abb652e22c993fe7a5c98efc0d651240f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8bd93b51837b04ade762d05a59d24ed1f68d2a4cd612020a5915736d43aa6f`  
		Last Modified: Wed, 09 Nov 2022 19:43:05 GMT  
		Size: 337.0 KB (336999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51903721c05174a5370399be9cfbcdfafdc616c28d0599d67308b9a44b07d5d9`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-alpine`

```console
$ docker pull caddy@sha256:25a0097607868fb05a89a5ab9fea2f2ea4cecdc89d887d7dcee8c778a21b9e1f
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
$ docker pull caddy@sha256:b12b313a563011ab587b862567334b5f1e510002b8e013bc40af1ae4377e032d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16834898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48e1e3f680dff812573b72d098360058ddd668873bde28a22261f68c876822fa`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:27 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Thu, 10 Nov 2022 20:49:27 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:32:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 10 Nov 2022 21:32:43 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 10 Nov 2022 21:32:43 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 10 Nov 2022 21:32:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 10 Nov 2022 21:32:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:32:49 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 10 Nov 2022 21:32:49 GMT
ENV XDG_DATA_HOME=/data
# Thu, 10 Nov 2022 21:32:50 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 10 Nov 2022 21:32:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Nov 2022 21:32:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Nov 2022 21:32:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Nov 2022 21:32:52 GMT
EXPOSE 80
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 443
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 443/udp
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 2019
# Thu, 10 Nov 2022 21:32:54 GMT
WORKDIR /srv
# Thu, 10 Nov 2022 21:32:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6f07846270a9d34a7f4e9dda7d81a5b081ba30588b9e3486c62b5cdcbc1405`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 304.4 KB (304400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5465143f5f5b00ed906a73fc1ac3b86f9deaee0c21b275408cf309fef94a4041`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 5.8 KB (5754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47d9833dc35b7555f175e85c7c0fba471ad40d97a949f6b0f80bfc19605f383`  
		Last Modified: Thu, 10 Nov 2022 21:34:01 GMT  
		Size: 13.9 MB (13910625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662ebf5c4140b8798aa93a33fe7539f17a6eafc57111e615a4634561648b9e23`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a49a9fa13cf6792de98f5351389c9fdad662db85ca244483c7b515f2f1ed87d0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16617549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32dee3a3e8e899357be2b1b4428f62f334dec2af23a51967830b837e25ae896d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 06:34:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Nov 2022 06:34:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 11 Nov 2022 06:34:17 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 11 Nov 2022 06:34:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Nov 2022 06:34:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Nov 2022 06:34:20 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Nov 2022 06:34:20 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Nov 2022 06:34:21 GMT
EXPOSE 80
# Fri, 11 Nov 2022 06:34:21 GMT
EXPOSE 443
# Fri, 11 Nov 2022 06:34:22 GMT
EXPOSE 443/udp
# Fri, 11 Nov 2022 06:34:22 GMT
EXPOSE 2019
# Fri, 11 Nov 2022 06:34:22 GMT
WORKDIR /srv
# Fri, 11 Nov 2022 06:34:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ccfb174b467ecb8cc057263afb9939d1b3e15b9bc1c515179694d952fbf851`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 303.5 KB (303527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c1861352af6dba0e4cb99dd7060c884cd671d012e014dba05a612be38386a9`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 5.8 KB (5752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d37c36eede286e9554ac6d4beb0c577e4b2d285a0127336fefda6484662c65e`  
		Last Modified: Fri, 11 Nov 2022 06:35:23 GMT  
		Size: 13.9 MB (13891052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66529f6b32306fba04edbc38d87e496b1a1141951b2861b2be6fbd339dc40264`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:313fb401ecc2c6a4428f9abdcb87f7a3bd48769cbeca02e6e096d00b67329554
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16278672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c799e3816961c596d5c1fb50aae78395f4fd343fc77bf3122e0d396d510fe83`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Thu, 10 Nov 2022 20:39:41 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:30:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 10 Nov 2022 21:30:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 10 Nov 2022 21:30:10 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 10 Nov 2022 21:30:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 10 Nov 2022 21:30:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:30:12 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 10 Nov 2022 21:30:12 GMT
ENV XDG_DATA_HOME=/data
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 80
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 443
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 443/udp
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 2019
# Thu, 10 Nov 2022 21:30:14 GMT
WORKDIR /srv
# Thu, 10 Nov 2022 21:30:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480d8737fa00cd91dd0632e620ecb371ff8e7fbb7792619315f962bd74ac78b0`  
		Last Modified: Thu, 10 Nov 2022 21:30:38 GMT  
		Size: 304.5 KB (304513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8b251ca0b51f9a0e2defca59988fe0d152662e2a155d0861aa02e2a7257dd1`  
		Last Modified: Thu, 10 Nov 2022 21:30:38 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9543d07ca7897910ddae9b3fb026b4004353b71f3342f8889a2ecf194358ef65`  
		Last Modified: Thu, 10 Nov 2022 21:30:39 GMT  
		Size: 13.3 MB (13260509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e0320d2afc0181e222e9018c3ce159603f04d94ac7754b2c57e2a2f198a477`  
		Last Modified: Thu, 10 Nov 2022 21:30:37 GMT  
		Size: 154.0 B  
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
$ docker pull caddy@sha256:1bfbc30b9fa0fe174661a0c039680b75fee83c3fdbeb8504faa1a4de574addce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3650; amd64
	-	windows version 10.0.20348.1249; amd64

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

### `caddy:2.6-builder` - windows version 10.0.17763.3650; amd64

```console
$ docker pull caddy@sha256:6cf653a2a7b8de4f339602e03c9c86540b02072e8b96e35878e007f769d7da16
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2963661660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cb2be08bd918187f9f5ad1fe999f73a7b423260e1205806377b8dc44e688751`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 13:56:03 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Nov 2022 13:56:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Nov 2022 13:56:05 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Nov 2022 13:56:06 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Nov 2022 13:57:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:57:58 GMT
ENV GOPATH=C:\go
# Wed, 09 Nov 2022 13:59:24 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Nov 2022 13:59:25 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 09 Nov 2022 14:03:31 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 14:03:33 GMT
WORKDIR C:\go
# Wed, 09 Nov 2022 18:13:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:13:29 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 09 Nov 2022 18:13:30 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:13:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Nov 2022 18:14:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Nov 2022 18:14:56 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a2b0ba4717890a5f71c35ff277f846f8f9b6668e0e7bb61c09c7be2ae6fa2b`  
		Last Modified: Wed, 09 Nov 2022 14:33:12 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ea601fe915f260a37aa95fd46906a58c4828c48a181f7fec434c255461bc3c`  
		Last Modified: Wed, 09 Nov 2022 14:33:07 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0a12f7377f09e1e60b8f98ba68c21900eb3bd8da74b27356717b7b531b1f19`  
		Last Modified: Wed, 09 Nov 2022 14:33:06 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96720d70c884dea5fd72c530b456770bdc779483b7f1d752e386360daffe6e4e`  
		Last Modified: Wed, 09 Nov 2022 14:33:06 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10a1ec572d19d510940ad8ddec14084b9e4d8300ef36b3ef50f23b477df789d`  
		Last Modified: Wed, 09 Nov 2022 14:33:16 GMT  
		Size: 25.5 MB (25457961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378cf1d27c9b1599652ca2d1c09cf3196ecbd22b40ee08813574a0fc119440d7`  
		Last Modified: Wed, 09 Nov 2022 14:33:04 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561cd622fdb3c0fabfcb202894dc24ba2a9491bf349e487be308fb6315c43c1d`  
		Last Modified: Wed, 09 Nov 2022 14:33:04 GMT  
		Size: 326.0 KB (326032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe2ec77bf4f0673d2620baa4e0302b768acebce02398e710036bf3f656c0ecc`  
		Last Modified: Wed, 09 Nov 2022 14:33:03 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eaf4d425600774d03d9f467838fe1b18d6a9460b749c91c1024aa8904b0e334`  
		Last Modified: Wed, 09 Nov 2022 14:33:58 GMT  
		Size: 157.6 MB (157648264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6413639a75ce7d233f32964ef57abd38fc992a742736bc7e7a163fa8aa5b4b0`  
		Last Modified: Wed, 09 Nov 2022 14:33:03 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614f1b9006d1823d89a42263057e769283383c54144a3dc50d4ea64dec74b5c7`  
		Last Modified: Wed, 09 Nov 2022 19:43:36 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184c91cb508dbf30520922b855e98043d4c3ea2479805b179085847628631e9b`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5127f06a739ff0fd5c240314901aa7fc16f2c5c55c07d10ab007bc1a4b1364dc`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b199d92416df53de1551d66e029f372db1c76a2afe75ea4afa7288ca8a3ab775`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbce37404bc1695c1f7d35e9732764388cfbd8391f96cf201053cb30562029fe`  
		Last Modified: Wed, 09 Nov 2022 19:43:34 GMT  
		Size: 1.6 MB (1624203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ed8f4a92cb5e13a8092652093226fe12e30e288d191f6b727f7fd79c9ad414`  
		Last Modified: Wed, 09 Nov 2022 19:43:34 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - windows version 10.0.20348.1249; amd64

```console
$ docker pull caddy@sha256:9ed32ae59f8639230dc09e89512d25258e2550fcf519495c20c1e2622b311772
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2667713878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aa94e32ea39d538bc848f49a88694ed5bff88005fcd74e8700db5a7e7befaee`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 13:51:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Nov 2022 13:51:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Nov 2022 13:51:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Nov 2022 13:51:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Nov 2022 13:52:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:52:12 GMT
ENV GOPATH=C:\go
# Wed, 09 Nov 2022 13:52:36 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Nov 2022 13:52:37 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 09 Nov 2022 13:55:50 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:55:52 GMT
WORKDIR C:\go
# Wed, 09 Nov 2022 18:15:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:15:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 09 Nov 2022 18:15:15 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:15:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Nov 2022 18:15:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Nov 2022 18:15:45 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea79272e8d2a572a4d212450946bce415296eae87b6ce74df5b622cdfee02c67`  
		Last Modified: Wed, 09 Nov 2022 14:31:56 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a776f73cd30b265202025b98515575e21f757c88c6361190224cf46c2b7d1d`  
		Last Modified: Wed, 09 Nov 2022 14:31:53 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5268ccf7578edb6ae20eccf50b8be8c8da75b9054711b531062a365dc4fdca4`  
		Last Modified: Wed, 09 Nov 2022 14:31:52 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c9e4ebbf21dbe0a28faabe67fd74fca79784fefc03a56fae2e25366742aa37`  
		Last Modified: Wed, 09 Nov 2022 14:31:51 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671be4304252589ad8fea639a28234c14a6aeab6a0913d98704928824b355f28`  
		Last Modified: Wed, 09 Nov 2022 14:32:01 GMT  
		Size: 25.7 MB (25693161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131c64f4139ebfed8185c51abad4bbb44ad9830a76a221307d83acc03b579f2e`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceec23424e6d501387ce0ab8f96b2349ac91551e8ff768a658f97eb07430e76`  
		Last Modified: Wed, 09 Nov 2022 14:31:49 GMT  
		Size: 548.2 KB (548156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9475cb31b9e6aa94b3c8bac11dad0e1d052709c8d931bf0ae9373371ad4d7bf`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f00ac483de739170f945938526dd868499e135b2661edf64b64a35e533d0ae`  
		Last Modified: Wed, 09 Nov 2022 14:32:45 GMT  
		Size: 157.8 MB (157844340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973945315f37c2cee022dc1f6b25fe2d420fa96edd876cad28a507515f40c18d`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.6 KB (1589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b243f67c60aae1519ab6b4211d6746d958ebdaded4297ea7378794c35d8683`  
		Last Modified: Wed, 09 Nov 2022 19:43:58 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd79a73ed810cffb30c91e80d20bf903af3dea7476f04d503d7051f1bdbe2be4`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd66ad327482a3d8d053309d10877a72859caaef7ed99c3841bf985c63d8164e`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c37cb6737d74657ec2c98ddb8bfaf994aa881104b47b2a3230edc36f93fe9f`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aef28670eb8e61758e89572ed759fc8b57fe8f1e3d40c8021cf21e0c80f3103`  
		Last Modified: Wed, 09 Nov 2022 19:43:57 GMT  
		Size: 1.8 MB (1841412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f961cc28a480ceb15a0e0c07284ecb8e251842282e48ee1695adb121939e3c`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1422 bytes)  
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
$ docker pull caddy@sha256:ed2c53e8bf858c413d1112ec78dad49683b6963cb6a6d43a02d3877afee50eb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `caddy:2.6-builder-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull caddy@sha256:6cf653a2a7b8de4f339602e03c9c86540b02072e8b96e35878e007f769d7da16
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2963661660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cb2be08bd918187f9f5ad1fe999f73a7b423260e1205806377b8dc44e688751`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 13:56:03 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Nov 2022 13:56:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Nov 2022 13:56:05 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Nov 2022 13:56:06 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Nov 2022 13:57:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:57:58 GMT
ENV GOPATH=C:\go
# Wed, 09 Nov 2022 13:59:24 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Nov 2022 13:59:25 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 09 Nov 2022 14:03:31 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 14:03:33 GMT
WORKDIR C:\go
# Wed, 09 Nov 2022 18:13:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:13:29 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 09 Nov 2022 18:13:30 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:13:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Nov 2022 18:14:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Nov 2022 18:14:56 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a2b0ba4717890a5f71c35ff277f846f8f9b6668e0e7bb61c09c7be2ae6fa2b`  
		Last Modified: Wed, 09 Nov 2022 14:33:12 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ea601fe915f260a37aa95fd46906a58c4828c48a181f7fec434c255461bc3c`  
		Last Modified: Wed, 09 Nov 2022 14:33:07 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0a12f7377f09e1e60b8f98ba68c21900eb3bd8da74b27356717b7b531b1f19`  
		Last Modified: Wed, 09 Nov 2022 14:33:06 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96720d70c884dea5fd72c530b456770bdc779483b7f1d752e386360daffe6e4e`  
		Last Modified: Wed, 09 Nov 2022 14:33:06 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10a1ec572d19d510940ad8ddec14084b9e4d8300ef36b3ef50f23b477df789d`  
		Last Modified: Wed, 09 Nov 2022 14:33:16 GMT  
		Size: 25.5 MB (25457961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378cf1d27c9b1599652ca2d1c09cf3196ecbd22b40ee08813574a0fc119440d7`  
		Last Modified: Wed, 09 Nov 2022 14:33:04 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561cd622fdb3c0fabfcb202894dc24ba2a9491bf349e487be308fb6315c43c1d`  
		Last Modified: Wed, 09 Nov 2022 14:33:04 GMT  
		Size: 326.0 KB (326032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe2ec77bf4f0673d2620baa4e0302b768acebce02398e710036bf3f656c0ecc`  
		Last Modified: Wed, 09 Nov 2022 14:33:03 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eaf4d425600774d03d9f467838fe1b18d6a9460b749c91c1024aa8904b0e334`  
		Last Modified: Wed, 09 Nov 2022 14:33:58 GMT  
		Size: 157.6 MB (157648264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6413639a75ce7d233f32964ef57abd38fc992a742736bc7e7a163fa8aa5b4b0`  
		Last Modified: Wed, 09 Nov 2022 14:33:03 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614f1b9006d1823d89a42263057e769283383c54144a3dc50d4ea64dec74b5c7`  
		Last Modified: Wed, 09 Nov 2022 19:43:36 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184c91cb508dbf30520922b855e98043d4c3ea2479805b179085847628631e9b`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5127f06a739ff0fd5c240314901aa7fc16f2c5c55c07d10ab007bc1a4b1364dc`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b199d92416df53de1551d66e029f372db1c76a2afe75ea4afa7288ca8a3ab775`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbce37404bc1695c1f7d35e9732764388cfbd8391f96cf201053cb30562029fe`  
		Last Modified: Wed, 09 Nov 2022 19:43:34 GMT  
		Size: 1.6 MB (1624203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ed8f4a92cb5e13a8092652093226fe12e30e288d191f6b727f7fd79c9ad414`  
		Last Modified: Wed, 09 Nov 2022 19:43:34 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:8f08b39d3c846f5fe51158683dd4062da0fed911c1d6a09f372c510316df9486
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1249; amd64

### `caddy:2.6-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1249; amd64

```console
$ docker pull caddy@sha256:9ed32ae59f8639230dc09e89512d25258e2550fcf519495c20c1e2622b311772
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2667713878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aa94e32ea39d538bc848f49a88694ed5bff88005fcd74e8700db5a7e7befaee`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 13:51:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Nov 2022 13:51:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Nov 2022 13:51:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Nov 2022 13:51:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Nov 2022 13:52:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:52:12 GMT
ENV GOPATH=C:\go
# Wed, 09 Nov 2022 13:52:36 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Nov 2022 13:52:37 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 09 Nov 2022 13:55:50 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:55:52 GMT
WORKDIR C:\go
# Wed, 09 Nov 2022 18:15:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:15:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 09 Nov 2022 18:15:15 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:15:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Nov 2022 18:15:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Nov 2022 18:15:45 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea79272e8d2a572a4d212450946bce415296eae87b6ce74df5b622cdfee02c67`  
		Last Modified: Wed, 09 Nov 2022 14:31:56 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a776f73cd30b265202025b98515575e21f757c88c6361190224cf46c2b7d1d`  
		Last Modified: Wed, 09 Nov 2022 14:31:53 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5268ccf7578edb6ae20eccf50b8be8c8da75b9054711b531062a365dc4fdca4`  
		Last Modified: Wed, 09 Nov 2022 14:31:52 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c9e4ebbf21dbe0a28faabe67fd74fca79784fefc03a56fae2e25366742aa37`  
		Last Modified: Wed, 09 Nov 2022 14:31:51 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671be4304252589ad8fea639a28234c14a6aeab6a0913d98704928824b355f28`  
		Last Modified: Wed, 09 Nov 2022 14:32:01 GMT  
		Size: 25.7 MB (25693161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131c64f4139ebfed8185c51abad4bbb44ad9830a76a221307d83acc03b579f2e`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceec23424e6d501387ce0ab8f96b2349ac91551e8ff768a658f97eb07430e76`  
		Last Modified: Wed, 09 Nov 2022 14:31:49 GMT  
		Size: 548.2 KB (548156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9475cb31b9e6aa94b3c8bac11dad0e1d052709c8d931bf0ae9373371ad4d7bf`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f00ac483de739170f945938526dd868499e135b2661edf64b64a35e533d0ae`  
		Last Modified: Wed, 09 Nov 2022 14:32:45 GMT  
		Size: 157.8 MB (157844340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973945315f37c2cee022dc1f6b25fe2d420fa96edd876cad28a507515f40c18d`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.6 KB (1589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b243f67c60aae1519ab6b4211d6746d958ebdaded4297ea7378794c35d8683`  
		Last Modified: Wed, 09 Nov 2022 19:43:58 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd79a73ed810cffb30c91e80d20bf903af3dea7476f04d503d7051f1bdbe2be4`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd66ad327482a3d8d053309d10877a72859caaef7ed99c3841bf985c63d8164e`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c37cb6737d74657ec2c98ddb8bfaf994aa881104b47b2a3230edc36f93fe9f`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aef28670eb8e61758e89572ed759fc8b57fe8f1e3d40c8021cf21e0c80f3103`  
		Last Modified: Wed, 09 Nov 2022 19:43:57 GMT  
		Size: 1.8 MB (1841412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f961cc28a480ceb15a0e0c07284ecb8e251842282e48ee1695adb121939e3c`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-windowsservercore`

```console
$ docker pull caddy@sha256:0a8af8e78d210109370f648e45b709e478abcdb65b491151144dc00c66fa5d39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3650; amd64
	-	windows version 10.0.20348.1249; amd64

### `caddy:2.6-windowsservercore` - windows version 10.0.17763.3650; amd64

```console
$ docker pull caddy@sha256:1bb072f445e9d5154311ff5502f598bc04f8f3a39962ba84935c924372254023
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2794246589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09e5adcd59d9a3cef6ebbe389ca4ba29c5fd69972ae3e411b8be53d7267ce1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:09:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:09:11 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:10:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:10:28 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:10:29 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:10:30 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:10:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:10:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:10:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:10:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:10:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:10:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:10:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:10:38 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:10:39 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:10:40 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:10:41 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:11:42 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:11:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c991125a18c41d60a99d6ec86c4c38917cda31bdc78ae2b19547118e64c3130`  
		Last Modified: Wed, 09 Nov 2022 19:42:43 GMT  
		Size: 376.0 KB (375983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c44dcec78b9053b83e9d2b0b85793a2d6dd9f7882eda9b68af412bfc561ae59`  
		Last Modified: Wed, 09 Nov 2022 19:42:42 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679594f71e58468aa9805558e75d701d34727227835b6f244c3227d0e8b3fc51`  
		Last Modified: Wed, 09 Nov 2022 19:42:45 GMT  
		Size: 15.0 MB (14954096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ec8fe5018705645312e2f15ddeff4193348e2d162b522e3d89004171e32611`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de52b8df46e754f4b7a96b07b9fcec10bba34c5203824f45ad667524e900442`  
		Last Modified: Wed, 09 Nov 2022 19:42:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de92b977c1ec3484f7ec22f1caf0af85a365785ef5a626cd1306e02ba2d78514`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14440e034f493a00a52bd65e46382b25e372630456a4bab3984ef60887bd4b2`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7fa7a9304ad99e65a0da0a731b88f220461e17a0a0aefd95e4388273c22107`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4688f22612a7a65254ccf95adb7b14eb333413e66689770a1b2ee648df6ae7a`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04f66e90a6de69b5c69c165ab290a0f792549149c911eef51f26380bdac82f2`  
		Last Modified: Wed, 09 Nov 2022 19:42:38 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a779763f5c2179feba42c73a1b4ac83edb90462493ee5b369908d6e839520f8`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d1d0c12a2c947c8a5a1942711ea238b6899cbbde6dc2d4c32401e2f336ebc5`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9267ecd850272decf95a74353e3505335d6ca458bd2d604cf6fd08f36b42b36d`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0daba2c50a467fa60cd066c4a707a46479815f75be8ccee29e3ffd74089e29c`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3399f861f6994eed02f962f0dfe8919ff2c59d392b5ee7cf1a2374a3e42892`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b97c99b6c4d5675b3327c5f3a35c918b75ab8fb154b22797764b4620b444c0`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634fc965a18e1d74efa1e1e64a43388feca61231913a4e4b3784b0955c81d4ec`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a7f978fb624cd5a777948f956d64e0e5688bd12864fc178bad1fa89cdf12f5`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 305.8 KB (305758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8494101343a0a636a7e1246e9ac5417edfd30766fa9cc3accad02c260ae99e3`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-windowsservercore` - windows version 10.0.20348.1249; amd64

```console
$ docker pull caddy@sha256:df26460add1714658ae82eb674ccba73fd3781a29eb1c742153d7f848ba77b03
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2497915476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf8cd6c30b11c2e211f77bf1bd355ab239d0405d001159b36bf501643b70145`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:12:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:12:22 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:12:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:12:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:12:51 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:12:52 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:12:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:12:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:12:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:12:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:12:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:12:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:12:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:13:00 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:13:01 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:13:18 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:13:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1dc6b6b8064ce6aa320f7658f5ddc1b7eafa5e7b7ed6eaa07e0d8a1c990256`  
		Last Modified: Wed, 09 Nov 2022 19:43:12 GMT  
		Size: 617.3 KB (617258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad0e2bc53452df09c89858e4b2f54e4b23c0c8bb58733f05d9b0b3a5f39b1e8`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa3455b7b8e4ed55199abb0ad62eea75ab0ab47616504b3758f35aed63ccbc8`  
		Last Modified: Wed, 09 Nov 2022 19:43:15 GMT  
		Size: 15.2 MB (15168482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d64bc11b8e88956f2cdb7f937525a2fb1c986000887f4dc88dc1eea98446d81`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8502309666e15b454660c5bfd9d1ebd352e18c945b8b2ede9afe9269a5937b`  
		Last Modified: Wed, 09 Nov 2022 19:43:10 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906c51626faa981aaf141adb1be3e8e65cbe12d592fa3c640dc829d28abd4d00`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ee5c1d8d0fd98304b819d90c4adb33feb485f3f47dcf390bee532f8d6b57f4`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63fc79d12f01d2fad54fd51f43571f0aaef608b2d7be31823c881667cb5e41e`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad24427c4c7dcb96616f4886c985d9252699bbaf01bb7f1551a776f57ac3080`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce3623edb8a858ba8a0f7f2184802487aa72c8332935270dbb0308fbbd70c0`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8180ccb35cb5b71974dc1c9130892b1c8ab0f20309906215682be61e553596c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b759234e6db3ee8b177b51b148eeb2a3ef89bc496e3098d56322d6e17a269f3c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc80653154d31f3fad6c8977be60b10618022311edaf9a0cba8a6eee3428aa1`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19a3de5a545f51fc5ee391f49dc670b30e5d6814b0bd8195075243d1d5d2d52`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d26ee259e1db29592ba9e5d679d72c081eab360aed0add981ddf4a44d7c7b2`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732e7368e5a0068535b80c136d98d840daeba6d9dd5d7fe90bb39b10c9fab27f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da48319bd36cb22c79804c6e3e5efa4abb652e22c993fe7a5c98efc0d651240f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8bd93b51837b04ade762d05a59d24ed1f68d2a4cd612020a5915736d43aa6f`  
		Last Modified: Wed, 09 Nov 2022 19:43:05 GMT  
		Size: 337.0 KB (336999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51903721c05174a5370399be9cfbcdfafdc616c28d0599d67308b9a44b07d5d9`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-windowsservercore-1809`

```console
$ docker pull caddy@sha256:7d8fa3f8a84211c6129b53d25df161f198e739bb5f6e676467db0eafca8cda29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `caddy:2.6-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull caddy@sha256:1bb072f445e9d5154311ff5502f598bc04f8f3a39962ba84935c924372254023
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2794246589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09e5adcd59d9a3cef6ebbe389ca4ba29c5fd69972ae3e411b8be53d7267ce1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:09:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:09:11 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:10:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:10:28 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:10:29 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:10:30 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:10:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:10:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:10:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:10:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:10:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:10:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:10:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:10:38 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:10:39 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:10:40 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:10:41 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:11:42 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:11:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c991125a18c41d60a99d6ec86c4c38917cda31bdc78ae2b19547118e64c3130`  
		Last Modified: Wed, 09 Nov 2022 19:42:43 GMT  
		Size: 376.0 KB (375983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c44dcec78b9053b83e9d2b0b85793a2d6dd9f7882eda9b68af412bfc561ae59`  
		Last Modified: Wed, 09 Nov 2022 19:42:42 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679594f71e58468aa9805558e75d701d34727227835b6f244c3227d0e8b3fc51`  
		Last Modified: Wed, 09 Nov 2022 19:42:45 GMT  
		Size: 15.0 MB (14954096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ec8fe5018705645312e2f15ddeff4193348e2d162b522e3d89004171e32611`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de52b8df46e754f4b7a96b07b9fcec10bba34c5203824f45ad667524e900442`  
		Last Modified: Wed, 09 Nov 2022 19:42:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de92b977c1ec3484f7ec22f1caf0af85a365785ef5a626cd1306e02ba2d78514`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14440e034f493a00a52bd65e46382b25e372630456a4bab3984ef60887bd4b2`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7fa7a9304ad99e65a0da0a731b88f220461e17a0a0aefd95e4388273c22107`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4688f22612a7a65254ccf95adb7b14eb333413e66689770a1b2ee648df6ae7a`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04f66e90a6de69b5c69c165ab290a0f792549149c911eef51f26380bdac82f2`  
		Last Modified: Wed, 09 Nov 2022 19:42:38 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a779763f5c2179feba42c73a1b4ac83edb90462493ee5b369908d6e839520f8`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d1d0c12a2c947c8a5a1942711ea238b6899cbbde6dc2d4c32401e2f336ebc5`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9267ecd850272decf95a74353e3505335d6ca458bd2d604cf6fd08f36b42b36d`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0daba2c50a467fa60cd066c4a707a46479815f75be8ccee29e3ffd74089e29c`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3399f861f6994eed02f962f0dfe8919ff2c59d392b5ee7cf1a2374a3e42892`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b97c99b6c4d5675b3327c5f3a35c918b75ab8fb154b22797764b4620b444c0`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634fc965a18e1d74efa1e1e64a43388feca61231913a4e4b3784b0955c81d4ec`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a7f978fb624cd5a777948f956d64e0e5688bd12864fc178bad1fa89cdf12f5`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 305.8 KB (305758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8494101343a0a636a7e1246e9ac5417edfd30766fa9cc3accad02c260ae99e3`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:618d9f501fb56f3d12f4566a58de1afafc1a3920ba686c84cc2e1134d1bf41e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1249; amd64

### `caddy:2.6-windowsservercore-ltsc2022` - windows version 10.0.20348.1249; amd64

```console
$ docker pull caddy@sha256:df26460add1714658ae82eb674ccba73fd3781a29eb1c742153d7f848ba77b03
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2497915476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf8cd6c30b11c2e211f77bf1bd355ab239d0405d001159b36bf501643b70145`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:12:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:12:22 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:12:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:12:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:12:51 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:12:52 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:12:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:12:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:12:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:12:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:12:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:12:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:12:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:13:00 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:13:01 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:13:18 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:13:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1dc6b6b8064ce6aa320f7658f5ddc1b7eafa5e7b7ed6eaa07e0d8a1c990256`  
		Last Modified: Wed, 09 Nov 2022 19:43:12 GMT  
		Size: 617.3 KB (617258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad0e2bc53452df09c89858e4b2f54e4b23c0c8bb58733f05d9b0b3a5f39b1e8`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa3455b7b8e4ed55199abb0ad62eea75ab0ab47616504b3758f35aed63ccbc8`  
		Last Modified: Wed, 09 Nov 2022 19:43:15 GMT  
		Size: 15.2 MB (15168482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d64bc11b8e88956f2cdb7f937525a2fb1c986000887f4dc88dc1eea98446d81`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8502309666e15b454660c5bfd9d1ebd352e18c945b8b2ede9afe9269a5937b`  
		Last Modified: Wed, 09 Nov 2022 19:43:10 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906c51626faa981aaf141adb1be3e8e65cbe12d592fa3c640dc829d28abd4d00`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ee5c1d8d0fd98304b819d90c4adb33feb485f3f47dcf390bee532f8d6b57f4`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63fc79d12f01d2fad54fd51f43571f0aaef608b2d7be31823c881667cb5e41e`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad24427c4c7dcb96616f4886c985d9252699bbaf01bb7f1551a776f57ac3080`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce3623edb8a858ba8a0f7f2184802487aa72c8332935270dbb0308fbbd70c0`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8180ccb35cb5b71974dc1c9130892b1c8ab0f20309906215682be61e553596c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b759234e6db3ee8b177b51b148eeb2a3ef89bc496e3098d56322d6e17a269f3c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc80653154d31f3fad6c8977be60b10618022311edaf9a0cba8a6eee3428aa1`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19a3de5a545f51fc5ee391f49dc670b30e5d6814b0bd8195075243d1d5d2d52`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d26ee259e1db29592ba9e5d679d72c081eab360aed0add981ddf4a44d7c7b2`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732e7368e5a0068535b80c136d98d840daeba6d9dd5d7fe90bb39b10c9fab27f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da48319bd36cb22c79804c6e3e5efa4abb652e22c993fe7a5c98efc0d651240f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8bd93b51837b04ade762d05a59d24ed1f68d2a4cd612020a5915736d43aa6f`  
		Last Modified: Wed, 09 Nov 2022 19:43:05 GMT  
		Size: 337.0 KB (336999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51903721c05174a5370399be9cfbcdfafdc616c28d0599d67308b9a44b07d5d9`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.2`

```console
$ docker pull caddy@sha256:50743fc6130295e9e8feccd8b2f437d8c472f626bf277dc873734ed98219f44f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3650; amd64
	-	windows version 10.0.20348.1249; amd64

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
$ docker pull caddy@sha256:b12b313a563011ab587b862567334b5f1e510002b8e013bc40af1ae4377e032d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16834898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48e1e3f680dff812573b72d098360058ddd668873bde28a22261f68c876822fa`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:27 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Thu, 10 Nov 2022 20:49:27 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:32:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 10 Nov 2022 21:32:43 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 10 Nov 2022 21:32:43 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 10 Nov 2022 21:32:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 10 Nov 2022 21:32:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:32:49 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 10 Nov 2022 21:32:49 GMT
ENV XDG_DATA_HOME=/data
# Thu, 10 Nov 2022 21:32:50 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 10 Nov 2022 21:32:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Nov 2022 21:32:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Nov 2022 21:32:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Nov 2022 21:32:52 GMT
EXPOSE 80
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 443
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 443/udp
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 2019
# Thu, 10 Nov 2022 21:32:54 GMT
WORKDIR /srv
# Thu, 10 Nov 2022 21:32:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6f07846270a9d34a7f4e9dda7d81a5b081ba30588b9e3486c62b5cdcbc1405`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 304.4 KB (304400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5465143f5f5b00ed906a73fc1ac3b86f9deaee0c21b275408cf309fef94a4041`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 5.8 KB (5754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47d9833dc35b7555f175e85c7c0fba471ad40d97a949f6b0f80bfc19605f383`  
		Last Modified: Thu, 10 Nov 2022 21:34:01 GMT  
		Size: 13.9 MB (13910625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662ebf5c4140b8798aa93a33fe7539f17a6eafc57111e615a4634561648b9e23`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a49a9fa13cf6792de98f5351389c9fdad662db85ca244483c7b515f2f1ed87d0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16617549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32dee3a3e8e899357be2b1b4428f62f334dec2af23a51967830b837e25ae896d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 06:34:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Nov 2022 06:34:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 11 Nov 2022 06:34:17 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 11 Nov 2022 06:34:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Nov 2022 06:34:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Nov 2022 06:34:20 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Nov 2022 06:34:20 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Nov 2022 06:34:21 GMT
EXPOSE 80
# Fri, 11 Nov 2022 06:34:21 GMT
EXPOSE 443
# Fri, 11 Nov 2022 06:34:22 GMT
EXPOSE 443/udp
# Fri, 11 Nov 2022 06:34:22 GMT
EXPOSE 2019
# Fri, 11 Nov 2022 06:34:22 GMT
WORKDIR /srv
# Fri, 11 Nov 2022 06:34:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ccfb174b467ecb8cc057263afb9939d1b3e15b9bc1c515179694d952fbf851`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 303.5 KB (303527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c1861352af6dba0e4cb99dd7060c884cd671d012e014dba05a612be38386a9`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 5.8 KB (5752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d37c36eede286e9554ac6d4beb0c577e4b2d285a0127336fefda6484662c65e`  
		Last Modified: Fri, 11 Nov 2022 06:35:23 GMT  
		Size: 13.9 MB (13891052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66529f6b32306fba04edbc38d87e496b1a1141951b2861b2be6fbd339dc40264`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:313fb401ecc2c6a4428f9abdcb87f7a3bd48769cbeca02e6e096d00b67329554
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16278672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c799e3816961c596d5c1fb50aae78395f4fd343fc77bf3122e0d396d510fe83`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Thu, 10 Nov 2022 20:39:41 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:30:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 10 Nov 2022 21:30:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 10 Nov 2022 21:30:10 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 10 Nov 2022 21:30:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 10 Nov 2022 21:30:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:30:12 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 10 Nov 2022 21:30:12 GMT
ENV XDG_DATA_HOME=/data
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 80
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 443
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 443/udp
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 2019
# Thu, 10 Nov 2022 21:30:14 GMT
WORKDIR /srv
# Thu, 10 Nov 2022 21:30:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480d8737fa00cd91dd0632e620ecb371ff8e7fbb7792619315f962bd74ac78b0`  
		Last Modified: Thu, 10 Nov 2022 21:30:38 GMT  
		Size: 304.5 KB (304513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8b251ca0b51f9a0e2defca59988fe0d152662e2a155d0861aa02e2a7257dd1`  
		Last Modified: Thu, 10 Nov 2022 21:30:38 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9543d07ca7897910ddae9b3fb026b4004353b71f3342f8889a2ecf194358ef65`  
		Last Modified: Thu, 10 Nov 2022 21:30:39 GMT  
		Size: 13.3 MB (13260509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e0320d2afc0181e222e9018c3ce159603f04d94ac7754b2c57e2a2f198a477`  
		Last Modified: Thu, 10 Nov 2022 21:30:37 GMT  
		Size: 154.0 B  
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

### `caddy:2.6.2` - windows version 10.0.17763.3650; amd64

```console
$ docker pull caddy@sha256:1bb072f445e9d5154311ff5502f598bc04f8f3a39962ba84935c924372254023
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2794246589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09e5adcd59d9a3cef6ebbe389ca4ba29c5fd69972ae3e411b8be53d7267ce1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:09:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:09:11 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:10:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:10:28 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:10:29 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:10:30 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:10:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:10:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:10:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:10:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:10:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:10:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:10:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:10:38 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:10:39 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:10:40 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:10:41 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:11:42 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:11:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c991125a18c41d60a99d6ec86c4c38917cda31bdc78ae2b19547118e64c3130`  
		Last Modified: Wed, 09 Nov 2022 19:42:43 GMT  
		Size: 376.0 KB (375983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c44dcec78b9053b83e9d2b0b85793a2d6dd9f7882eda9b68af412bfc561ae59`  
		Last Modified: Wed, 09 Nov 2022 19:42:42 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679594f71e58468aa9805558e75d701d34727227835b6f244c3227d0e8b3fc51`  
		Last Modified: Wed, 09 Nov 2022 19:42:45 GMT  
		Size: 15.0 MB (14954096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ec8fe5018705645312e2f15ddeff4193348e2d162b522e3d89004171e32611`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de52b8df46e754f4b7a96b07b9fcec10bba34c5203824f45ad667524e900442`  
		Last Modified: Wed, 09 Nov 2022 19:42:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de92b977c1ec3484f7ec22f1caf0af85a365785ef5a626cd1306e02ba2d78514`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14440e034f493a00a52bd65e46382b25e372630456a4bab3984ef60887bd4b2`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7fa7a9304ad99e65a0da0a731b88f220461e17a0a0aefd95e4388273c22107`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4688f22612a7a65254ccf95adb7b14eb333413e66689770a1b2ee648df6ae7a`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04f66e90a6de69b5c69c165ab290a0f792549149c911eef51f26380bdac82f2`  
		Last Modified: Wed, 09 Nov 2022 19:42:38 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a779763f5c2179feba42c73a1b4ac83edb90462493ee5b369908d6e839520f8`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d1d0c12a2c947c8a5a1942711ea238b6899cbbde6dc2d4c32401e2f336ebc5`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9267ecd850272decf95a74353e3505335d6ca458bd2d604cf6fd08f36b42b36d`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0daba2c50a467fa60cd066c4a707a46479815f75be8ccee29e3ffd74089e29c`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3399f861f6994eed02f962f0dfe8919ff2c59d392b5ee7cf1a2374a3e42892`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b97c99b6c4d5675b3327c5f3a35c918b75ab8fb154b22797764b4620b444c0`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634fc965a18e1d74efa1e1e64a43388feca61231913a4e4b3784b0955c81d4ec`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a7f978fb624cd5a777948f956d64e0e5688bd12864fc178bad1fa89cdf12f5`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 305.8 KB (305758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8494101343a0a636a7e1246e9ac5417edfd30766fa9cc3accad02c260ae99e3`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2` - windows version 10.0.20348.1249; amd64

```console
$ docker pull caddy@sha256:df26460add1714658ae82eb674ccba73fd3781a29eb1c742153d7f848ba77b03
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2497915476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf8cd6c30b11c2e211f77bf1bd355ab239d0405d001159b36bf501643b70145`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:12:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:12:22 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:12:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:12:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:12:51 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:12:52 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:12:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:12:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:12:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:12:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:12:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:12:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:12:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:13:00 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:13:01 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:13:18 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:13:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1dc6b6b8064ce6aa320f7658f5ddc1b7eafa5e7b7ed6eaa07e0d8a1c990256`  
		Last Modified: Wed, 09 Nov 2022 19:43:12 GMT  
		Size: 617.3 KB (617258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad0e2bc53452df09c89858e4b2f54e4b23c0c8bb58733f05d9b0b3a5f39b1e8`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa3455b7b8e4ed55199abb0ad62eea75ab0ab47616504b3758f35aed63ccbc8`  
		Last Modified: Wed, 09 Nov 2022 19:43:15 GMT  
		Size: 15.2 MB (15168482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d64bc11b8e88956f2cdb7f937525a2fb1c986000887f4dc88dc1eea98446d81`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8502309666e15b454660c5bfd9d1ebd352e18c945b8b2ede9afe9269a5937b`  
		Last Modified: Wed, 09 Nov 2022 19:43:10 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906c51626faa981aaf141adb1be3e8e65cbe12d592fa3c640dc829d28abd4d00`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ee5c1d8d0fd98304b819d90c4adb33feb485f3f47dcf390bee532f8d6b57f4`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63fc79d12f01d2fad54fd51f43571f0aaef608b2d7be31823c881667cb5e41e`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad24427c4c7dcb96616f4886c985d9252699bbaf01bb7f1551a776f57ac3080`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce3623edb8a858ba8a0f7f2184802487aa72c8332935270dbb0308fbbd70c0`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8180ccb35cb5b71974dc1c9130892b1c8ab0f20309906215682be61e553596c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b759234e6db3ee8b177b51b148eeb2a3ef89bc496e3098d56322d6e17a269f3c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc80653154d31f3fad6c8977be60b10618022311edaf9a0cba8a6eee3428aa1`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19a3de5a545f51fc5ee391f49dc670b30e5d6814b0bd8195075243d1d5d2d52`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d26ee259e1db29592ba9e5d679d72c081eab360aed0add981ddf4a44d7c7b2`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732e7368e5a0068535b80c136d98d840daeba6d9dd5d7fe90bb39b10c9fab27f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da48319bd36cb22c79804c6e3e5efa4abb652e22c993fe7a5c98efc0d651240f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8bd93b51837b04ade762d05a59d24ed1f68d2a4cd612020a5915736d43aa6f`  
		Last Modified: Wed, 09 Nov 2022 19:43:05 GMT  
		Size: 337.0 KB (336999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51903721c05174a5370399be9cfbcdfafdc616c28d0599d67308b9a44b07d5d9`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.2-alpine`

```console
$ docker pull caddy@sha256:25a0097607868fb05a89a5ab9fea2f2ea4cecdc89d887d7dcee8c778a21b9e1f
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
$ docker pull caddy@sha256:b12b313a563011ab587b862567334b5f1e510002b8e013bc40af1ae4377e032d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16834898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48e1e3f680dff812573b72d098360058ddd668873bde28a22261f68c876822fa`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:27 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Thu, 10 Nov 2022 20:49:27 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:32:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 10 Nov 2022 21:32:43 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 10 Nov 2022 21:32:43 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 10 Nov 2022 21:32:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 10 Nov 2022 21:32:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:32:49 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 10 Nov 2022 21:32:49 GMT
ENV XDG_DATA_HOME=/data
# Thu, 10 Nov 2022 21:32:50 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 10 Nov 2022 21:32:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Nov 2022 21:32:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Nov 2022 21:32:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Nov 2022 21:32:52 GMT
EXPOSE 80
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 443
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 443/udp
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 2019
# Thu, 10 Nov 2022 21:32:54 GMT
WORKDIR /srv
# Thu, 10 Nov 2022 21:32:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6f07846270a9d34a7f4e9dda7d81a5b081ba30588b9e3486c62b5cdcbc1405`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 304.4 KB (304400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5465143f5f5b00ed906a73fc1ac3b86f9deaee0c21b275408cf309fef94a4041`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 5.8 KB (5754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47d9833dc35b7555f175e85c7c0fba471ad40d97a949f6b0f80bfc19605f383`  
		Last Modified: Thu, 10 Nov 2022 21:34:01 GMT  
		Size: 13.9 MB (13910625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662ebf5c4140b8798aa93a33fe7539f17a6eafc57111e615a4634561648b9e23`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a49a9fa13cf6792de98f5351389c9fdad662db85ca244483c7b515f2f1ed87d0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16617549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32dee3a3e8e899357be2b1b4428f62f334dec2af23a51967830b837e25ae896d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 06:34:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Nov 2022 06:34:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 11 Nov 2022 06:34:17 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 11 Nov 2022 06:34:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Nov 2022 06:34:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Nov 2022 06:34:20 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Nov 2022 06:34:20 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Nov 2022 06:34:21 GMT
EXPOSE 80
# Fri, 11 Nov 2022 06:34:21 GMT
EXPOSE 443
# Fri, 11 Nov 2022 06:34:22 GMT
EXPOSE 443/udp
# Fri, 11 Nov 2022 06:34:22 GMT
EXPOSE 2019
# Fri, 11 Nov 2022 06:34:22 GMT
WORKDIR /srv
# Fri, 11 Nov 2022 06:34:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ccfb174b467ecb8cc057263afb9939d1b3e15b9bc1c515179694d952fbf851`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 303.5 KB (303527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c1861352af6dba0e4cb99dd7060c884cd671d012e014dba05a612be38386a9`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 5.8 KB (5752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d37c36eede286e9554ac6d4beb0c577e4b2d285a0127336fefda6484662c65e`  
		Last Modified: Fri, 11 Nov 2022 06:35:23 GMT  
		Size: 13.9 MB (13891052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66529f6b32306fba04edbc38d87e496b1a1141951b2861b2be6fbd339dc40264`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:313fb401ecc2c6a4428f9abdcb87f7a3bd48769cbeca02e6e096d00b67329554
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16278672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c799e3816961c596d5c1fb50aae78395f4fd343fc77bf3122e0d396d510fe83`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Thu, 10 Nov 2022 20:39:41 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:30:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 10 Nov 2022 21:30:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 10 Nov 2022 21:30:10 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 10 Nov 2022 21:30:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 10 Nov 2022 21:30:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:30:12 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 10 Nov 2022 21:30:12 GMT
ENV XDG_DATA_HOME=/data
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 80
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 443
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 443/udp
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 2019
# Thu, 10 Nov 2022 21:30:14 GMT
WORKDIR /srv
# Thu, 10 Nov 2022 21:30:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480d8737fa00cd91dd0632e620ecb371ff8e7fbb7792619315f962bd74ac78b0`  
		Last Modified: Thu, 10 Nov 2022 21:30:38 GMT  
		Size: 304.5 KB (304513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8b251ca0b51f9a0e2defca59988fe0d152662e2a155d0861aa02e2a7257dd1`  
		Last Modified: Thu, 10 Nov 2022 21:30:38 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9543d07ca7897910ddae9b3fb026b4004353b71f3342f8889a2ecf194358ef65`  
		Last Modified: Thu, 10 Nov 2022 21:30:39 GMT  
		Size: 13.3 MB (13260509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e0320d2afc0181e222e9018c3ce159603f04d94ac7754b2c57e2a2f198a477`  
		Last Modified: Thu, 10 Nov 2022 21:30:37 GMT  
		Size: 154.0 B  
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
$ docker pull caddy@sha256:1bfbc30b9fa0fe174661a0c039680b75fee83c3fdbeb8504faa1a4de574addce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3650; amd64
	-	windows version 10.0.20348.1249; amd64

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

### `caddy:2.6.2-builder` - windows version 10.0.17763.3650; amd64

```console
$ docker pull caddy@sha256:6cf653a2a7b8de4f339602e03c9c86540b02072e8b96e35878e007f769d7da16
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2963661660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cb2be08bd918187f9f5ad1fe999f73a7b423260e1205806377b8dc44e688751`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 13:56:03 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Nov 2022 13:56:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Nov 2022 13:56:05 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Nov 2022 13:56:06 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Nov 2022 13:57:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:57:58 GMT
ENV GOPATH=C:\go
# Wed, 09 Nov 2022 13:59:24 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Nov 2022 13:59:25 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 09 Nov 2022 14:03:31 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 14:03:33 GMT
WORKDIR C:\go
# Wed, 09 Nov 2022 18:13:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:13:29 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 09 Nov 2022 18:13:30 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:13:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Nov 2022 18:14:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Nov 2022 18:14:56 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a2b0ba4717890a5f71c35ff277f846f8f9b6668e0e7bb61c09c7be2ae6fa2b`  
		Last Modified: Wed, 09 Nov 2022 14:33:12 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ea601fe915f260a37aa95fd46906a58c4828c48a181f7fec434c255461bc3c`  
		Last Modified: Wed, 09 Nov 2022 14:33:07 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0a12f7377f09e1e60b8f98ba68c21900eb3bd8da74b27356717b7b531b1f19`  
		Last Modified: Wed, 09 Nov 2022 14:33:06 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96720d70c884dea5fd72c530b456770bdc779483b7f1d752e386360daffe6e4e`  
		Last Modified: Wed, 09 Nov 2022 14:33:06 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10a1ec572d19d510940ad8ddec14084b9e4d8300ef36b3ef50f23b477df789d`  
		Last Modified: Wed, 09 Nov 2022 14:33:16 GMT  
		Size: 25.5 MB (25457961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378cf1d27c9b1599652ca2d1c09cf3196ecbd22b40ee08813574a0fc119440d7`  
		Last Modified: Wed, 09 Nov 2022 14:33:04 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561cd622fdb3c0fabfcb202894dc24ba2a9491bf349e487be308fb6315c43c1d`  
		Last Modified: Wed, 09 Nov 2022 14:33:04 GMT  
		Size: 326.0 KB (326032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe2ec77bf4f0673d2620baa4e0302b768acebce02398e710036bf3f656c0ecc`  
		Last Modified: Wed, 09 Nov 2022 14:33:03 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eaf4d425600774d03d9f467838fe1b18d6a9460b749c91c1024aa8904b0e334`  
		Last Modified: Wed, 09 Nov 2022 14:33:58 GMT  
		Size: 157.6 MB (157648264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6413639a75ce7d233f32964ef57abd38fc992a742736bc7e7a163fa8aa5b4b0`  
		Last Modified: Wed, 09 Nov 2022 14:33:03 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614f1b9006d1823d89a42263057e769283383c54144a3dc50d4ea64dec74b5c7`  
		Last Modified: Wed, 09 Nov 2022 19:43:36 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184c91cb508dbf30520922b855e98043d4c3ea2479805b179085847628631e9b`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5127f06a739ff0fd5c240314901aa7fc16f2c5c55c07d10ab007bc1a4b1364dc`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b199d92416df53de1551d66e029f372db1c76a2afe75ea4afa7288ca8a3ab775`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbce37404bc1695c1f7d35e9732764388cfbd8391f96cf201053cb30562029fe`  
		Last Modified: Wed, 09 Nov 2022 19:43:34 GMT  
		Size: 1.6 MB (1624203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ed8f4a92cb5e13a8092652093226fe12e30e288d191f6b727f7fd79c9ad414`  
		Last Modified: Wed, 09 Nov 2022 19:43:34 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2-builder` - windows version 10.0.20348.1249; amd64

```console
$ docker pull caddy@sha256:9ed32ae59f8639230dc09e89512d25258e2550fcf519495c20c1e2622b311772
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2667713878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aa94e32ea39d538bc848f49a88694ed5bff88005fcd74e8700db5a7e7befaee`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 13:51:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Nov 2022 13:51:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Nov 2022 13:51:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Nov 2022 13:51:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Nov 2022 13:52:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:52:12 GMT
ENV GOPATH=C:\go
# Wed, 09 Nov 2022 13:52:36 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Nov 2022 13:52:37 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 09 Nov 2022 13:55:50 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:55:52 GMT
WORKDIR C:\go
# Wed, 09 Nov 2022 18:15:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:15:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 09 Nov 2022 18:15:15 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:15:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Nov 2022 18:15:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Nov 2022 18:15:45 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea79272e8d2a572a4d212450946bce415296eae87b6ce74df5b622cdfee02c67`  
		Last Modified: Wed, 09 Nov 2022 14:31:56 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a776f73cd30b265202025b98515575e21f757c88c6361190224cf46c2b7d1d`  
		Last Modified: Wed, 09 Nov 2022 14:31:53 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5268ccf7578edb6ae20eccf50b8be8c8da75b9054711b531062a365dc4fdca4`  
		Last Modified: Wed, 09 Nov 2022 14:31:52 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c9e4ebbf21dbe0a28faabe67fd74fca79784fefc03a56fae2e25366742aa37`  
		Last Modified: Wed, 09 Nov 2022 14:31:51 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671be4304252589ad8fea639a28234c14a6aeab6a0913d98704928824b355f28`  
		Last Modified: Wed, 09 Nov 2022 14:32:01 GMT  
		Size: 25.7 MB (25693161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131c64f4139ebfed8185c51abad4bbb44ad9830a76a221307d83acc03b579f2e`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceec23424e6d501387ce0ab8f96b2349ac91551e8ff768a658f97eb07430e76`  
		Last Modified: Wed, 09 Nov 2022 14:31:49 GMT  
		Size: 548.2 KB (548156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9475cb31b9e6aa94b3c8bac11dad0e1d052709c8d931bf0ae9373371ad4d7bf`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f00ac483de739170f945938526dd868499e135b2661edf64b64a35e533d0ae`  
		Last Modified: Wed, 09 Nov 2022 14:32:45 GMT  
		Size: 157.8 MB (157844340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973945315f37c2cee022dc1f6b25fe2d420fa96edd876cad28a507515f40c18d`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.6 KB (1589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b243f67c60aae1519ab6b4211d6746d958ebdaded4297ea7378794c35d8683`  
		Last Modified: Wed, 09 Nov 2022 19:43:58 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd79a73ed810cffb30c91e80d20bf903af3dea7476f04d503d7051f1bdbe2be4`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd66ad327482a3d8d053309d10877a72859caaef7ed99c3841bf985c63d8164e`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c37cb6737d74657ec2c98ddb8bfaf994aa881104b47b2a3230edc36f93fe9f`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aef28670eb8e61758e89572ed759fc8b57fe8f1e3d40c8021cf21e0c80f3103`  
		Last Modified: Wed, 09 Nov 2022 19:43:57 GMT  
		Size: 1.8 MB (1841412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f961cc28a480ceb15a0e0c07284ecb8e251842282e48ee1695adb121939e3c`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1422 bytes)  
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
$ docker pull caddy@sha256:ed2c53e8bf858c413d1112ec78dad49683b6963cb6a6d43a02d3877afee50eb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `caddy:2.6.2-builder-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull caddy@sha256:6cf653a2a7b8de4f339602e03c9c86540b02072e8b96e35878e007f769d7da16
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2963661660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cb2be08bd918187f9f5ad1fe999f73a7b423260e1205806377b8dc44e688751`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 13:56:03 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Nov 2022 13:56:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Nov 2022 13:56:05 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Nov 2022 13:56:06 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Nov 2022 13:57:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:57:58 GMT
ENV GOPATH=C:\go
# Wed, 09 Nov 2022 13:59:24 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Nov 2022 13:59:25 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 09 Nov 2022 14:03:31 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 14:03:33 GMT
WORKDIR C:\go
# Wed, 09 Nov 2022 18:13:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:13:29 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 09 Nov 2022 18:13:30 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:13:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Nov 2022 18:14:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Nov 2022 18:14:56 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a2b0ba4717890a5f71c35ff277f846f8f9b6668e0e7bb61c09c7be2ae6fa2b`  
		Last Modified: Wed, 09 Nov 2022 14:33:12 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ea601fe915f260a37aa95fd46906a58c4828c48a181f7fec434c255461bc3c`  
		Last Modified: Wed, 09 Nov 2022 14:33:07 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0a12f7377f09e1e60b8f98ba68c21900eb3bd8da74b27356717b7b531b1f19`  
		Last Modified: Wed, 09 Nov 2022 14:33:06 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96720d70c884dea5fd72c530b456770bdc779483b7f1d752e386360daffe6e4e`  
		Last Modified: Wed, 09 Nov 2022 14:33:06 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10a1ec572d19d510940ad8ddec14084b9e4d8300ef36b3ef50f23b477df789d`  
		Last Modified: Wed, 09 Nov 2022 14:33:16 GMT  
		Size: 25.5 MB (25457961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378cf1d27c9b1599652ca2d1c09cf3196ecbd22b40ee08813574a0fc119440d7`  
		Last Modified: Wed, 09 Nov 2022 14:33:04 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561cd622fdb3c0fabfcb202894dc24ba2a9491bf349e487be308fb6315c43c1d`  
		Last Modified: Wed, 09 Nov 2022 14:33:04 GMT  
		Size: 326.0 KB (326032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe2ec77bf4f0673d2620baa4e0302b768acebce02398e710036bf3f656c0ecc`  
		Last Modified: Wed, 09 Nov 2022 14:33:03 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eaf4d425600774d03d9f467838fe1b18d6a9460b749c91c1024aa8904b0e334`  
		Last Modified: Wed, 09 Nov 2022 14:33:58 GMT  
		Size: 157.6 MB (157648264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6413639a75ce7d233f32964ef57abd38fc992a742736bc7e7a163fa8aa5b4b0`  
		Last Modified: Wed, 09 Nov 2022 14:33:03 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614f1b9006d1823d89a42263057e769283383c54144a3dc50d4ea64dec74b5c7`  
		Last Modified: Wed, 09 Nov 2022 19:43:36 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184c91cb508dbf30520922b855e98043d4c3ea2479805b179085847628631e9b`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5127f06a739ff0fd5c240314901aa7fc16f2c5c55c07d10ab007bc1a4b1364dc`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b199d92416df53de1551d66e029f372db1c76a2afe75ea4afa7288ca8a3ab775`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbce37404bc1695c1f7d35e9732764388cfbd8391f96cf201053cb30562029fe`  
		Last Modified: Wed, 09 Nov 2022 19:43:34 GMT  
		Size: 1.6 MB (1624203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ed8f4a92cb5e13a8092652093226fe12e30e288d191f6b727f7fd79c9ad414`  
		Last Modified: Wed, 09 Nov 2022 19:43:34 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:8f08b39d3c846f5fe51158683dd4062da0fed911c1d6a09f372c510316df9486
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1249; amd64

### `caddy:2.6.2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1249; amd64

```console
$ docker pull caddy@sha256:9ed32ae59f8639230dc09e89512d25258e2550fcf519495c20c1e2622b311772
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2667713878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aa94e32ea39d538bc848f49a88694ed5bff88005fcd74e8700db5a7e7befaee`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 13:51:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Nov 2022 13:51:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Nov 2022 13:51:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Nov 2022 13:51:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Nov 2022 13:52:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:52:12 GMT
ENV GOPATH=C:\go
# Wed, 09 Nov 2022 13:52:36 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Nov 2022 13:52:37 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 09 Nov 2022 13:55:50 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:55:52 GMT
WORKDIR C:\go
# Wed, 09 Nov 2022 18:15:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:15:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 09 Nov 2022 18:15:15 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:15:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Nov 2022 18:15:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Nov 2022 18:15:45 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea79272e8d2a572a4d212450946bce415296eae87b6ce74df5b622cdfee02c67`  
		Last Modified: Wed, 09 Nov 2022 14:31:56 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a776f73cd30b265202025b98515575e21f757c88c6361190224cf46c2b7d1d`  
		Last Modified: Wed, 09 Nov 2022 14:31:53 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5268ccf7578edb6ae20eccf50b8be8c8da75b9054711b531062a365dc4fdca4`  
		Last Modified: Wed, 09 Nov 2022 14:31:52 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c9e4ebbf21dbe0a28faabe67fd74fca79784fefc03a56fae2e25366742aa37`  
		Last Modified: Wed, 09 Nov 2022 14:31:51 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671be4304252589ad8fea639a28234c14a6aeab6a0913d98704928824b355f28`  
		Last Modified: Wed, 09 Nov 2022 14:32:01 GMT  
		Size: 25.7 MB (25693161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131c64f4139ebfed8185c51abad4bbb44ad9830a76a221307d83acc03b579f2e`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceec23424e6d501387ce0ab8f96b2349ac91551e8ff768a658f97eb07430e76`  
		Last Modified: Wed, 09 Nov 2022 14:31:49 GMT  
		Size: 548.2 KB (548156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9475cb31b9e6aa94b3c8bac11dad0e1d052709c8d931bf0ae9373371ad4d7bf`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f00ac483de739170f945938526dd868499e135b2661edf64b64a35e533d0ae`  
		Last Modified: Wed, 09 Nov 2022 14:32:45 GMT  
		Size: 157.8 MB (157844340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973945315f37c2cee022dc1f6b25fe2d420fa96edd876cad28a507515f40c18d`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.6 KB (1589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b243f67c60aae1519ab6b4211d6746d958ebdaded4297ea7378794c35d8683`  
		Last Modified: Wed, 09 Nov 2022 19:43:58 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd79a73ed810cffb30c91e80d20bf903af3dea7476f04d503d7051f1bdbe2be4`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd66ad327482a3d8d053309d10877a72859caaef7ed99c3841bf985c63d8164e`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c37cb6737d74657ec2c98ddb8bfaf994aa881104b47b2a3230edc36f93fe9f`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aef28670eb8e61758e89572ed759fc8b57fe8f1e3d40c8021cf21e0c80f3103`  
		Last Modified: Wed, 09 Nov 2022 19:43:57 GMT  
		Size: 1.8 MB (1841412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f961cc28a480ceb15a0e0c07284ecb8e251842282e48ee1695adb121939e3c`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.2-windowsservercore`

```console
$ docker pull caddy@sha256:0a8af8e78d210109370f648e45b709e478abcdb65b491151144dc00c66fa5d39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3650; amd64
	-	windows version 10.0.20348.1249; amd64

### `caddy:2.6.2-windowsservercore` - windows version 10.0.17763.3650; amd64

```console
$ docker pull caddy@sha256:1bb072f445e9d5154311ff5502f598bc04f8f3a39962ba84935c924372254023
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2794246589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09e5adcd59d9a3cef6ebbe389ca4ba29c5fd69972ae3e411b8be53d7267ce1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:09:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:09:11 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:10:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:10:28 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:10:29 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:10:30 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:10:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:10:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:10:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:10:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:10:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:10:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:10:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:10:38 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:10:39 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:10:40 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:10:41 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:11:42 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:11:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c991125a18c41d60a99d6ec86c4c38917cda31bdc78ae2b19547118e64c3130`  
		Last Modified: Wed, 09 Nov 2022 19:42:43 GMT  
		Size: 376.0 KB (375983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c44dcec78b9053b83e9d2b0b85793a2d6dd9f7882eda9b68af412bfc561ae59`  
		Last Modified: Wed, 09 Nov 2022 19:42:42 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679594f71e58468aa9805558e75d701d34727227835b6f244c3227d0e8b3fc51`  
		Last Modified: Wed, 09 Nov 2022 19:42:45 GMT  
		Size: 15.0 MB (14954096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ec8fe5018705645312e2f15ddeff4193348e2d162b522e3d89004171e32611`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de52b8df46e754f4b7a96b07b9fcec10bba34c5203824f45ad667524e900442`  
		Last Modified: Wed, 09 Nov 2022 19:42:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de92b977c1ec3484f7ec22f1caf0af85a365785ef5a626cd1306e02ba2d78514`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14440e034f493a00a52bd65e46382b25e372630456a4bab3984ef60887bd4b2`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7fa7a9304ad99e65a0da0a731b88f220461e17a0a0aefd95e4388273c22107`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4688f22612a7a65254ccf95adb7b14eb333413e66689770a1b2ee648df6ae7a`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04f66e90a6de69b5c69c165ab290a0f792549149c911eef51f26380bdac82f2`  
		Last Modified: Wed, 09 Nov 2022 19:42:38 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a779763f5c2179feba42c73a1b4ac83edb90462493ee5b369908d6e839520f8`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d1d0c12a2c947c8a5a1942711ea238b6899cbbde6dc2d4c32401e2f336ebc5`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9267ecd850272decf95a74353e3505335d6ca458bd2d604cf6fd08f36b42b36d`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0daba2c50a467fa60cd066c4a707a46479815f75be8ccee29e3ffd74089e29c`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3399f861f6994eed02f962f0dfe8919ff2c59d392b5ee7cf1a2374a3e42892`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b97c99b6c4d5675b3327c5f3a35c918b75ab8fb154b22797764b4620b444c0`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634fc965a18e1d74efa1e1e64a43388feca61231913a4e4b3784b0955c81d4ec`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a7f978fb624cd5a777948f956d64e0e5688bd12864fc178bad1fa89cdf12f5`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 305.8 KB (305758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8494101343a0a636a7e1246e9ac5417edfd30766fa9cc3accad02c260ae99e3`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.2-windowsservercore` - windows version 10.0.20348.1249; amd64

```console
$ docker pull caddy@sha256:df26460add1714658ae82eb674ccba73fd3781a29eb1c742153d7f848ba77b03
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2497915476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf8cd6c30b11c2e211f77bf1bd355ab239d0405d001159b36bf501643b70145`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:12:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:12:22 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:12:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:12:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:12:51 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:12:52 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:12:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:12:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:12:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:12:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:12:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:12:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:12:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:13:00 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:13:01 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:13:18 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:13:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1dc6b6b8064ce6aa320f7658f5ddc1b7eafa5e7b7ed6eaa07e0d8a1c990256`  
		Last Modified: Wed, 09 Nov 2022 19:43:12 GMT  
		Size: 617.3 KB (617258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad0e2bc53452df09c89858e4b2f54e4b23c0c8bb58733f05d9b0b3a5f39b1e8`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa3455b7b8e4ed55199abb0ad62eea75ab0ab47616504b3758f35aed63ccbc8`  
		Last Modified: Wed, 09 Nov 2022 19:43:15 GMT  
		Size: 15.2 MB (15168482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d64bc11b8e88956f2cdb7f937525a2fb1c986000887f4dc88dc1eea98446d81`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8502309666e15b454660c5bfd9d1ebd352e18c945b8b2ede9afe9269a5937b`  
		Last Modified: Wed, 09 Nov 2022 19:43:10 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906c51626faa981aaf141adb1be3e8e65cbe12d592fa3c640dc829d28abd4d00`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ee5c1d8d0fd98304b819d90c4adb33feb485f3f47dcf390bee532f8d6b57f4`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63fc79d12f01d2fad54fd51f43571f0aaef608b2d7be31823c881667cb5e41e`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad24427c4c7dcb96616f4886c985d9252699bbaf01bb7f1551a776f57ac3080`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce3623edb8a858ba8a0f7f2184802487aa72c8332935270dbb0308fbbd70c0`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8180ccb35cb5b71974dc1c9130892b1c8ab0f20309906215682be61e553596c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b759234e6db3ee8b177b51b148eeb2a3ef89bc496e3098d56322d6e17a269f3c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc80653154d31f3fad6c8977be60b10618022311edaf9a0cba8a6eee3428aa1`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19a3de5a545f51fc5ee391f49dc670b30e5d6814b0bd8195075243d1d5d2d52`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d26ee259e1db29592ba9e5d679d72c081eab360aed0add981ddf4a44d7c7b2`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732e7368e5a0068535b80c136d98d840daeba6d9dd5d7fe90bb39b10c9fab27f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da48319bd36cb22c79804c6e3e5efa4abb652e22c993fe7a5c98efc0d651240f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8bd93b51837b04ade762d05a59d24ed1f68d2a4cd612020a5915736d43aa6f`  
		Last Modified: Wed, 09 Nov 2022 19:43:05 GMT  
		Size: 337.0 KB (336999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51903721c05174a5370399be9cfbcdfafdc616c28d0599d67308b9a44b07d5d9`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:7d8fa3f8a84211c6129b53d25df161f198e739bb5f6e676467db0eafca8cda29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `caddy:2.6.2-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull caddy@sha256:1bb072f445e9d5154311ff5502f598bc04f8f3a39962ba84935c924372254023
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2794246589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09e5adcd59d9a3cef6ebbe389ca4ba29c5fd69972ae3e411b8be53d7267ce1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:09:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:09:11 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:10:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:10:28 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:10:29 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:10:30 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:10:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:10:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:10:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:10:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:10:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:10:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:10:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:10:38 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:10:39 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:10:40 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:10:41 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:11:42 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:11:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c991125a18c41d60a99d6ec86c4c38917cda31bdc78ae2b19547118e64c3130`  
		Last Modified: Wed, 09 Nov 2022 19:42:43 GMT  
		Size: 376.0 KB (375983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c44dcec78b9053b83e9d2b0b85793a2d6dd9f7882eda9b68af412bfc561ae59`  
		Last Modified: Wed, 09 Nov 2022 19:42:42 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679594f71e58468aa9805558e75d701d34727227835b6f244c3227d0e8b3fc51`  
		Last Modified: Wed, 09 Nov 2022 19:42:45 GMT  
		Size: 15.0 MB (14954096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ec8fe5018705645312e2f15ddeff4193348e2d162b522e3d89004171e32611`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de52b8df46e754f4b7a96b07b9fcec10bba34c5203824f45ad667524e900442`  
		Last Modified: Wed, 09 Nov 2022 19:42:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de92b977c1ec3484f7ec22f1caf0af85a365785ef5a626cd1306e02ba2d78514`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14440e034f493a00a52bd65e46382b25e372630456a4bab3984ef60887bd4b2`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7fa7a9304ad99e65a0da0a731b88f220461e17a0a0aefd95e4388273c22107`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4688f22612a7a65254ccf95adb7b14eb333413e66689770a1b2ee648df6ae7a`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04f66e90a6de69b5c69c165ab290a0f792549149c911eef51f26380bdac82f2`  
		Last Modified: Wed, 09 Nov 2022 19:42:38 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a779763f5c2179feba42c73a1b4ac83edb90462493ee5b369908d6e839520f8`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d1d0c12a2c947c8a5a1942711ea238b6899cbbde6dc2d4c32401e2f336ebc5`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9267ecd850272decf95a74353e3505335d6ca458bd2d604cf6fd08f36b42b36d`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0daba2c50a467fa60cd066c4a707a46479815f75be8ccee29e3ffd74089e29c`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3399f861f6994eed02f962f0dfe8919ff2c59d392b5ee7cf1a2374a3e42892`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b97c99b6c4d5675b3327c5f3a35c918b75ab8fb154b22797764b4620b444c0`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634fc965a18e1d74efa1e1e64a43388feca61231913a4e4b3784b0955c81d4ec`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a7f978fb624cd5a777948f956d64e0e5688bd12864fc178bad1fa89cdf12f5`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 305.8 KB (305758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8494101343a0a636a7e1246e9ac5417edfd30766fa9cc3accad02c260ae99e3`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:618d9f501fb56f3d12f4566a58de1afafc1a3920ba686c84cc2e1134d1bf41e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1249; amd64

### `caddy:2.6.2-windowsservercore-ltsc2022` - windows version 10.0.20348.1249; amd64

```console
$ docker pull caddy@sha256:df26460add1714658ae82eb674ccba73fd3781a29eb1c742153d7f848ba77b03
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2497915476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf8cd6c30b11c2e211f77bf1bd355ab239d0405d001159b36bf501643b70145`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:12:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:12:22 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:12:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:12:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:12:51 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:12:52 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:12:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:12:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:12:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:12:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:12:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:12:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:12:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:13:00 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:13:01 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:13:18 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:13:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1dc6b6b8064ce6aa320f7658f5ddc1b7eafa5e7b7ed6eaa07e0d8a1c990256`  
		Last Modified: Wed, 09 Nov 2022 19:43:12 GMT  
		Size: 617.3 KB (617258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad0e2bc53452df09c89858e4b2f54e4b23c0c8bb58733f05d9b0b3a5f39b1e8`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa3455b7b8e4ed55199abb0ad62eea75ab0ab47616504b3758f35aed63ccbc8`  
		Last Modified: Wed, 09 Nov 2022 19:43:15 GMT  
		Size: 15.2 MB (15168482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d64bc11b8e88956f2cdb7f937525a2fb1c986000887f4dc88dc1eea98446d81`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8502309666e15b454660c5bfd9d1ebd352e18c945b8b2ede9afe9269a5937b`  
		Last Modified: Wed, 09 Nov 2022 19:43:10 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906c51626faa981aaf141adb1be3e8e65cbe12d592fa3c640dc829d28abd4d00`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ee5c1d8d0fd98304b819d90c4adb33feb485f3f47dcf390bee532f8d6b57f4`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63fc79d12f01d2fad54fd51f43571f0aaef608b2d7be31823c881667cb5e41e`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad24427c4c7dcb96616f4886c985d9252699bbaf01bb7f1551a776f57ac3080`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce3623edb8a858ba8a0f7f2184802487aa72c8332935270dbb0308fbbd70c0`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8180ccb35cb5b71974dc1c9130892b1c8ab0f20309906215682be61e553596c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b759234e6db3ee8b177b51b148eeb2a3ef89bc496e3098d56322d6e17a269f3c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc80653154d31f3fad6c8977be60b10618022311edaf9a0cba8a6eee3428aa1`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19a3de5a545f51fc5ee391f49dc670b30e5d6814b0bd8195075243d1d5d2d52`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d26ee259e1db29592ba9e5d679d72c081eab360aed0add981ddf4a44d7c7b2`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732e7368e5a0068535b80c136d98d840daeba6d9dd5d7fe90bb39b10c9fab27f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da48319bd36cb22c79804c6e3e5efa4abb652e22c993fe7a5c98efc0d651240f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8bd93b51837b04ade762d05a59d24ed1f68d2a4cd612020a5915736d43aa6f`  
		Last Modified: Wed, 09 Nov 2022 19:43:05 GMT  
		Size: 337.0 KB (336999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51903721c05174a5370399be9cfbcdfafdc616c28d0599d67308b9a44b07d5d9`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:25a0097607868fb05a89a5ab9fea2f2ea4cecdc89d887d7dcee8c778a21b9e1f
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
$ docker pull caddy@sha256:b12b313a563011ab587b862567334b5f1e510002b8e013bc40af1ae4377e032d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16834898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48e1e3f680dff812573b72d098360058ddd668873bde28a22261f68c876822fa`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:27 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Thu, 10 Nov 2022 20:49:27 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:32:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 10 Nov 2022 21:32:43 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 10 Nov 2022 21:32:43 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 10 Nov 2022 21:32:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 10 Nov 2022 21:32:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:32:49 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 10 Nov 2022 21:32:49 GMT
ENV XDG_DATA_HOME=/data
# Thu, 10 Nov 2022 21:32:50 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 10 Nov 2022 21:32:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Nov 2022 21:32:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Nov 2022 21:32:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Nov 2022 21:32:52 GMT
EXPOSE 80
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 443
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 443/udp
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 2019
# Thu, 10 Nov 2022 21:32:54 GMT
WORKDIR /srv
# Thu, 10 Nov 2022 21:32:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6f07846270a9d34a7f4e9dda7d81a5b081ba30588b9e3486c62b5cdcbc1405`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 304.4 KB (304400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5465143f5f5b00ed906a73fc1ac3b86f9deaee0c21b275408cf309fef94a4041`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 5.8 KB (5754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47d9833dc35b7555f175e85c7c0fba471ad40d97a949f6b0f80bfc19605f383`  
		Last Modified: Thu, 10 Nov 2022 21:34:01 GMT  
		Size: 13.9 MB (13910625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662ebf5c4140b8798aa93a33fe7539f17a6eafc57111e615a4634561648b9e23`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a49a9fa13cf6792de98f5351389c9fdad662db85ca244483c7b515f2f1ed87d0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16617549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32dee3a3e8e899357be2b1b4428f62f334dec2af23a51967830b837e25ae896d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 06:34:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Nov 2022 06:34:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 11 Nov 2022 06:34:17 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 11 Nov 2022 06:34:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Nov 2022 06:34:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Nov 2022 06:34:20 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Nov 2022 06:34:20 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Nov 2022 06:34:21 GMT
EXPOSE 80
# Fri, 11 Nov 2022 06:34:21 GMT
EXPOSE 443
# Fri, 11 Nov 2022 06:34:22 GMT
EXPOSE 443/udp
# Fri, 11 Nov 2022 06:34:22 GMT
EXPOSE 2019
# Fri, 11 Nov 2022 06:34:22 GMT
WORKDIR /srv
# Fri, 11 Nov 2022 06:34:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ccfb174b467ecb8cc057263afb9939d1b3e15b9bc1c515179694d952fbf851`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 303.5 KB (303527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c1861352af6dba0e4cb99dd7060c884cd671d012e014dba05a612be38386a9`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 5.8 KB (5752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d37c36eede286e9554ac6d4beb0c577e4b2d285a0127336fefda6484662c65e`  
		Last Modified: Fri, 11 Nov 2022 06:35:23 GMT  
		Size: 13.9 MB (13891052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66529f6b32306fba04edbc38d87e496b1a1141951b2861b2be6fbd339dc40264`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:313fb401ecc2c6a4428f9abdcb87f7a3bd48769cbeca02e6e096d00b67329554
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16278672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c799e3816961c596d5c1fb50aae78395f4fd343fc77bf3122e0d396d510fe83`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Thu, 10 Nov 2022 20:39:41 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:30:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 10 Nov 2022 21:30:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 10 Nov 2022 21:30:10 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 10 Nov 2022 21:30:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 10 Nov 2022 21:30:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:30:12 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 10 Nov 2022 21:30:12 GMT
ENV XDG_DATA_HOME=/data
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 80
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 443
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 443/udp
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 2019
# Thu, 10 Nov 2022 21:30:14 GMT
WORKDIR /srv
# Thu, 10 Nov 2022 21:30:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480d8737fa00cd91dd0632e620ecb371ff8e7fbb7792619315f962bd74ac78b0`  
		Last Modified: Thu, 10 Nov 2022 21:30:38 GMT  
		Size: 304.5 KB (304513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8b251ca0b51f9a0e2defca59988fe0d152662e2a155d0861aa02e2a7257dd1`  
		Last Modified: Thu, 10 Nov 2022 21:30:38 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9543d07ca7897910ddae9b3fb026b4004353b71f3342f8889a2ecf194358ef65`  
		Last Modified: Thu, 10 Nov 2022 21:30:39 GMT  
		Size: 13.3 MB (13260509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e0320d2afc0181e222e9018c3ce159603f04d94ac7754b2c57e2a2f198a477`  
		Last Modified: Thu, 10 Nov 2022 21:30:37 GMT  
		Size: 154.0 B  
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
$ docker pull caddy@sha256:1bfbc30b9fa0fe174661a0c039680b75fee83c3fdbeb8504faa1a4de574addce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3650; amd64
	-	windows version 10.0.20348.1249; amd64

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

### `caddy:builder` - windows version 10.0.17763.3650; amd64

```console
$ docker pull caddy@sha256:6cf653a2a7b8de4f339602e03c9c86540b02072e8b96e35878e007f769d7da16
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2963661660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cb2be08bd918187f9f5ad1fe999f73a7b423260e1205806377b8dc44e688751`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 13:56:03 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Nov 2022 13:56:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Nov 2022 13:56:05 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Nov 2022 13:56:06 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Nov 2022 13:57:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:57:58 GMT
ENV GOPATH=C:\go
# Wed, 09 Nov 2022 13:59:24 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Nov 2022 13:59:25 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 09 Nov 2022 14:03:31 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 14:03:33 GMT
WORKDIR C:\go
# Wed, 09 Nov 2022 18:13:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:13:29 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 09 Nov 2022 18:13:30 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:13:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Nov 2022 18:14:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Nov 2022 18:14:56 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a2b0ba4717890a5f71c35ff277f846f8f9b6668e0e7bb61c09c7be2ae6fa2b`  
		Last Modified: Wed, 09 Nov 2022 14:33:12 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ea601fe915f260a37aa95fd46906a58c4828c48a181f7fec434c255461bc3c`  
		Last Modified: Wed, 09 Nov 2022 14:33:07 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0a12f7377f09e1e60b8f98ba68c21900eb3bd8da74b27356717b7b531b1f19`  
		Last Modified: Wed, 09 Nov 2022 14:33:06 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96720d70c884dea5fd72c530b456770bdc779483b7f1d752e386360daffe6e4e`  
		Last Modified: Wed, 09 Nov 2022 14:33:06 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10a1ec572d19d510940ad8ddec14084b9e4d8300ef36b3ef50f23b477df789d`  
		Last Modified: Wed, 09 Nov 2022 14:33:16 GMT  
		Size: 25.5 MB (25457961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378cf1d27c9b1599652ca2d1c09cf3196ecbd22b40ee08813574a0fc119440d7`  
		Last Modified: Wed, 09 Nov 2022 14:33:04 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561cd622fdb3c0fabfcb202894dc24ba2a9491bf349e487be308fb6315c43c1d`  
		Last Modified: Wed, 09 Nov 2022 14:33:04 GMT  
		Size: 326.0 KB (326032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe2ec77bf4f0673d2620baa4e0302b768acebce02398e710036bf3f656c0ecc`  
		Last Modified: Wed, 09 Nov 2022 14:33:03 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eaf4d425600774d03d9f467838fe1b18d6a9460b749c91c1024aa8904b0e334`  
		Last Modified: Wed, 09 Nov 2022 14:33:58 GMT  
		Size: 157.6 MB (157648264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6413639a75ce7d233f32964ef57abd38fc992a742736bc7e7a163fa8aa5b4b0`  
		Last Modified: Wed, 09 Nov 2022 14:33:03 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614f1b9006d1823d89a42263057e769283383c54144a3dc50d4ea64dec74b5c7`  
		Last Modified: Wed, 09 Nov 2022 19:43:36 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184c91cb508dbf30520922b855e98043d4c3ea2479805b179085847628631e9b`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5127f06a739ff0fd5c240314901aa7fc16f2c5c55c07d10ab007bc1a4b1364dc`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b199d92416df53de1551d66e029f372db1c76a2afe75ea4afa7288ca8a3ab775`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbce37404bc1695c1f7d35e9732764388cfbd8391f96cf201053cb30562029fe`  
		Last Modified: Wed, 09 Nov 2022 19:43:34 GMT  
		Size: 1.6 MB (1624203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ed8f4a92cb5e13a8092652093226fe12e30e288d191f6b727f7fd79c9ad414`  
		Last Modified: Wed, 09 Nov 2022 19:43:34 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.20348.1249; amd64

```console
$ docker pull caddy@sha256:9ed32ae59f8639230dc09e89512d25258e2550fcf519495c20c1e2622b311772
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2667713878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aa94e32ea39d538bc848f49a88694ed5bff88005fcd74e8700db5a7e7befaee`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 13:51:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Nov 2022 13:51:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Nov 2022 13:51:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Nov 2022 13:51:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Nov 2022 13:52:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:52:12 GMT
ENV GOPATH=C:\go
# Wed, 09 Nov 2022 13:52:36 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Nov 2022 13:52:37 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 09 Nov 2022 13:55:50 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:55:52 GMT
WORKDIR C:\go
# Wed, 09 Nov 2022 18:15:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:15:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 09 Nov 2022 18:15:15 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:15:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Nov 2022 18:15:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Nov 2022 18:15:45 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea79272e8d2a572a4d212450946bce415296eae87b6ce74df5b622cdfee02c67`  
		Last Modified: Wed, 09 Nov 2022 14:31:56 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a776f73cd30b265202025b98515575e21f757c88c6361190224cf46c2b7d1d`  
		Last Modified: Wed, 09 Nov 2022 14:31:53 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5268ccf7578edb6ae20eccf50b8be8c8da75b9054711b531062a365dc4fdca4`  
		Last Modified: Wed, 09 Nov 2022 14:31:52 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c9e4ebbf21dbe0a28faabe67fd74fca79784fefc03a56fae2e25366742aa37`  
		Last Modified: Wed, 09 Nov 2022 14:31:51 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671be4304252589ad8fea639a28234c14a6aeab6a0913d98704928824b355f28`  
		Last Modified: Wed, 09 Nov 2022 14:32:01 GMT  
		Size: 25.7 MB (25693161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131c64f4139ebfed8185c51abad4bbb44ad9830a76a221307d83acc03b579f2e`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceec23424e6d501387ce0ab8f96b2349ac91551e8ff768a658f97eb07430e76`  
		Last Modified: Wed, 09 Nov 2022 14:31:49 GMT  
		Size: 548.2 KB (548156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9475cb31b9e6aa94b3c8bac11dad0e1d052709c8d931bf0ae9373371ad4d7bf`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f00ac483de739170f945938526dd868499e135b2661edf64b64a35e533d0ae`  
		Last Modified: Wed, 09 Nov 2022 14:32:45 GMT  
		Size: 157.8 MB (157844340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973945315f37c2cee022dc1f6b25fe2d420fa96edd876cad28a507515f40c18d`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.6 KB (1589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b243f67c60aae1519ab6b4211d6746d958ebdaded4297ea7378794c35d8683`  
		Last Modified: Wed, 09 Nov 2022 19:43:58 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd79a73ed810cffb30c91e80d20bf903af3dea7476f04d503d7051f1bdbe2be4`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd66ad327482a3d8d053309d10877a72859caaef7ed99c3841bf985c63d8164e`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c37cb6737d74657ec2c98ddb8bfaf994aa881104b47b2a3230edc36f93fe9f`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aef28670eb8e61758e89572ed759fc8b57fe8f1e3d40c8021cf21e0c80f3103`  
		Last Modified: Wed, 09 Nov 2022 19:43:57 GMT  
		Size: 1.8 MB (1841412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f961cc28a480ceb15a0e0c07284ecb8e251842282e48ee1695adb121939e3c`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1422 bytes)  
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
$ docker pull caddy@sha256:ed2c53e8bf858c413d1112ec78dad49683b6963cb6a6d43a02d3877afee50eb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull caddy@sha256:6cf653a2a7b8de4f339602e03c9c86540b02072e8b96e35878e007f769d7da16
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2963661660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cb2be08bd918187f9f5ad1fe999f73a7b423260e1205806377b8dc44e688751`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 13:56:03 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Nov 2022 13:56:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Nov 2022 13:56:05 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Nov 2022 13:56:06 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Nov 2022 13:57:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:57:58 GMT
ENV GOPATH=C:\go
# Wed, 09 Nov 2022 13:59:24 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Nov 2022 13:59:25 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 09 Nov 2022 14:03:31 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 14:03:33 GMT
WORKDIR C:\go
# Wed, 09 Nov 2022 18:13:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:13:29 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 09 Nov 2022 18:13:30 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:13:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Nov 2022 18:14:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Nov 2022 18:14:56 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a2b0ba4717890a5f71c35ff277f846f8f9b6668e0e7bb61c09c7be2ae6fa2b`  
		Last Modified: Wed, 09 Nov 2022 14:33:12 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ea601fe915f260a37aa95fd46906a58c4828c48a181f7fec434c255461bc3c`  
		Last Modified: Wed, 09 Nov 2022 14:33:07 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0a12f7377f09e1e60b8f98ba68c21900eb3bd8da74b27356717b7b531b1f19`  
		Last Modified: Wed, 09 Nov 2022 14:33:06 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96720d70c884dea5fd72c530b456770bdc779483b7f1d752e386360daffe6e4e`  
		Last Modified: Wed, 09 Nov 2022 14:33:06 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10a1ec572d19d510940ad8ddec14084b9e4d8300ef36b3ef50f23b477df789d`  
		Last Modified: Wed, 09 Nov 2022 14:33:16 GMT  
		Size: 25.5 MB (25457961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378cf1d27c9b1599652ca2d1c09cf3196ecbd22b40ee08813574a0fc119440d7`  
		Last Modified: Wed, 09 Nov 2022 14:33:04 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561cd622fdb3c0fabfcb202894dc24ba2a9491bf349e487be308fb6315c43c1d`  
		Last Modified: Wed, 09 Nov 2022 14:33:04 GMT  
		Size: 326.0 KB (326032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe2ec77bf4f0673d2620baa4e0302b768acebce02398e710036bf3f656c0ecc`  
		Last Modified: Wed, 09 Nov 2022 14:33:03 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eaf4d425600774d03d9f467838fe1b18d6a9460b749c91c1024aa8904b0e334`  
		Last Modified: Wed, 09 Nov 2022 14:33:58 GMT  
		Size: 157.6 MB (157648264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6413639a75ce7d233f32964ef57abd38fc992a742736bc7e7a163fa8aa5b4b0`  
		Last Modified: Wed, 09 Nov 2022 14:33:03 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614f1b9006d1823d89a42263057e769283383c54144a3dc50d4ea64dec74b5c7`  
		Last Modified: Wed, 09 Nov 2022 19:43:36 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184c91cb508dbf30520922b855e98043d4c3ea2479805b179085847628631e9b`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5127f06a739ff0fd5c240314901aa7fc16f2c5c55c07d10ab007bc1a4b1364dc`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b199d92416df53de1551d66e029f372db1c76a2afe75ea4afa7288ca8a3ab775`  
		Last Modified: Wed, 09 Nov 2022 19:43:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbce37404bc1695c1f7d35e9732764388cfbd8391f96cf201053cb30562029fe`  
		Last Modified: Wed, 09 Nov 2022 19:43:34 GMT  
		Size: 1.6 MB (1624203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ed8f4a92cb5e13a8092652093226fe12e30e288d191f6b727f7fd79c9ad414`  
		Last Modified: Wed, 09 Nov 2022 19:43:34 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:8f08b39d3c846f5fe51158683dd4062da0fed911c1d6a09f372c510316df9486
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1249; amd64

### `caddy:builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1249; amd64

```console
$ docker pull caddy@sha256:9ed32ae59f8639230dc09e89512d25258e2550fcf519495c20c1e2622b311772
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2667713878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aa94e32ea39d538bc848f49a88694ed5bff88005fcd74e8700db5a7e7befaee`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 13:51:30 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Nov 2022 13:51:31 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Nov 2022 13:51:32 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Nov 2022 13:51:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Nov 2022 13:52:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:52:12 GMT
ENV GOPATH=C:\go
# Wed, 09 Nov 2022 13:52:36 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Nov 2022 13:52:37 GMT
ENV GOLANG_VERSION=1.19.3
# Wed, 09 Nov 2022 13:55:50 GMT
RUN $url = 'https://dl.google.com/go/go1.19.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'b51549a9f21ee053f8a3d8e38e45b1b8b282d976f3b60f1f89b37ac54e272d31'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Nov 2022 13:55:52 GMT
WORKDIR C:\go
# Wed, 09 Nov 2022 18:15:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:15:14 GMT
ENV XCADDY_VERSION=v0.3.1
# Wed, 09 Nov 2022 18:15:15 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:15:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Nov 2022 18:15:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.1/xcaddy_0.3.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('f20e6ae1f20b65098ed7d1638a7ba96bd8da8dc8e7b6f771d32f33216abfd20606b821c6780d49ed866629764613deaff9adf3c7a26c35ec9413979b5e1087a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 09 Nov 2022 18:15:45 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea79272e8d2a572a4d212450946bce415296eae87b6ce74df5b622cdfee02c67`  
		Last Modified: Wed, 09 Nov 2022 14:31:56 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a776f73cd30b265202025b98515575e21f757c88c6361190224cf46c2b7d1d`  
		Last Modified: Wed, 09 Nov 2022 14:31:53 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5268ccf7578edb6ae20eccf50b8be8c8da75b9054711b531062a365dc4fdca4`  
		Last Modified: Wed, 09 Nov 2022 14:31:52 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c9e4ebbf21dbe0a28faabe67fd74fca79784fefc03a56fae2e25366742aa37`  
		Last Modified: Wed, 09 Nov 2022 14:31:51 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671be4304252589ad8fea639a28234c14a6aeab6a0913d98704928824b355f28`  
		Last Modified: Wed, 09 Nov 2022 14:32:01 GMT  
		Size: 25.7 MB (25693161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131c64f4139ebfed8185c51abad4bbb44ad9830a76a221307d83acc03b579f2e`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceec23424e6d501387ce0ab8f96b2349ac91551e8ff768a658f97eb07430e76`  
		Last Modified: Wed, 09 Nov 2022 14:31:49 GMT  
		Size: 548.2 KB (548156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9475cb31b9e6aa94b3c8bac11dad0e1d052709c8d931bf0ae9373371ad4d7bf`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f00ac483de739170f945938526dd868499e135b2661edf64b64a35e533d0ae`  
		Last Modified: Wed, 09 Nov 2022 14:32:45 GMT  
		Size: 157.8 MB (157844340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973945315f37c2cee022dc1f6b25fe2d420fa96edd876cad28a507515f40c18d`  
		Last Modified: Wed, 09 Nov 2022 14:31:48 GMT  
		Size: 1.6 KB (1589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b243f67c60aae1519ab6b4211d6746d958ebdaded4297ea7378794c35d8683`  
		Last Modified: Wed, 09 Nov 2022 19:43:58 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd79a73ed810cffb30c91e80d20bf903af3dea7476f04d503d7051f1bdbe2be4`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd66ad327482a3d8d053309d10877a72859caaef7ed99c3841bf985c63d8164e`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c37cb6737d74657ec2c98ddb8bfaf994aa881104b47b2a3230edc36f93fe9f`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aef28670eb8e61758e89572ed759fc8b57fe8f1e3d40c8021cf21e0c80f3103`  
		Last Modified: Wed, 09 Nov 2022 19:43:57 GMT  
		Size: 1.8 MB (1841412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f961cc28a480ceb15a0e0c07284ecb8e251842282e48ee1695adb121939e3c`  
		Last Modified: Wed, 09 Nov 2022 19:43:56 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:50743fc6130295e9e8feccd8b2f437d8c472f626bf277dc873734ed98219f44f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3650; amd64
	-	windows version 10.0.20348.1249; amd64

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
$ docker pull caddy@sha256:b12b313a563011ab587b862567334b5f1e510002b8e013bc40af1ae4377e032d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16834898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48e1e3f680dff812573b72d098360058ddd668873bde28a22261f68c876822fa`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:27 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Thu, 10 Nov 2022 20:49:27 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:32:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 10 Nov 2022 21:32:43 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 10 Nov 2022 21:32:43 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 10 Nov 2022 21:32:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 10 Nov 2022 21:32:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:32:49 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 10 Nov 2022 21:32:49 GMT
ENV XDG_DATA_HOME=/data
# Thu, 10 Nov 2022 21:32:50 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 10 Nov 2022 21:32:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Nov 2022 21:32:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Nov 2022 21:32:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Nov 2022 21:32:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Nov 2022 21:32:52 GMT
EXPOSE 80
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 443
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 443/udp
# Thu, 10 Nov 2022 21:32:53 GMT
EXPOSE 2019
# Thu, 10 Nov 2022 21:32:54 GMT
WORKDIR /srv
# Thu, 10 Nov 2022 21:32:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6f07846270a9d34a7f4e9dda7d81a5b081ba30588b9e3486c62b5cdcbc1405`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 304.4 KB (304400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5465143f5f5b00ed906a73fc1ac3b86f9deaee0c21b275408cf309fef94a4041`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 5.8 KB (5754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47d9833dc35b7555f175e85c7c0fba471ad40d97a949f6b0f80bfc19605f383`  
		Last Modified: Thu, 10 Nov 2022 21:34:01 GMT  
		Size: 13.9 MB (13910625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662ebf5c4140b8798aa93a33fe7539f17a6eafc57111e615a4634561648b9e23`  
		Last Modified: Thu, 10 Nov 2022 21:33:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a49a9fa13cf6792de98f5351389c9fdad662db85ca244483c7b515f2f1ed87d0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16617549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32dee3a3e8e899357be2b1b4428f62f334dec2af23a51967830b837e25ae896d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 06:34:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 11 Nov 2022 06:34:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Fri, 11 Nov 2022 06:34:17 GMT
ENV CADDY_VERSION=v2.6.2
# Fri, 11 Nov 2022 06:34:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 11 Nov 2022 06:34:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Nov 2022 06:34:20 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 11 Nov 2022 06:34:20 GMT
ENV XDG_DATA_HOME=/data
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 11 Nov 2022 06:34:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 11 Nov 2022 06:34:21 GMT
EXPOSE 80
# Fri, 11 Nov 2022 06:34:21 GMT
EXPOSE 443
# Fri, 11 Nov 2022 06:34:22 GMT
EXPOSE 443/udp
# Fri, 11 Nov 2022 06:34:22 GMT
EXPOSE 2019
# Fri, 11 Nov 2022 06:34:22 GMT
WORKDIR /srv
# Fri, 11 Nov 2022 06:34:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ccfb174b467ecb8cc057263afb9939d1b3e15b9bc1c515179694d952fbf851`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 303.5 KB (303527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c1861352af6dba0e4cb99dd7060c884cd671d012e014dba05a612be38386a9`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 5.8 KB (5752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d37c36eede286e9554ac6d4beb0c577e4b2d285a0127336fefda6484662c65e`  
		Last Modified: Fri, 11 Nov 2022 06:35:23 GMT  
		Size: 13.9 MB (13891052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66529f6b32306fba04edbc38d87e496b1a1141951b2861b2be6fbd339dc40264`  
		Last Modified: Fri, 11 Nov 2022 06:35:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:313fb401ecc2c6a4428f9abdcb87f7a3bd48769cbeca02e6e096d00b67329554
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16278672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c799e3816961c596d5c1fb50aae78395f4fd343fc77bf3122e0d396d510fe83`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Thu, 10 Nov 2022 20:39:41 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:30:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 10 Nov 2022 21:30:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"
# Thu, 10 Nov 2022 21:30:10 GMT
ENV CADDY_VERSION=v2.6.2
# Thu, 10 Nov 2022 21:30:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae18c0facae7c8ee872492a1ba63a4c7608915d6d9fe267aef4f869cf65ebd4b7f9ff57f609aff2bd52db98c761d877b574aea2c0c9ddc2ec53d0d5e174cb542' ;; 		armhf)   binArch='armv6'; checksum='6de688e6514df67594635c79be51a3fe3b7b29254b36349955979571d0624dd9bb228abcb798e76fc64ec0e1c4884443c3fd5074a5b5124ee895d29d239bcf1c' ;; 		armv7)   binArch='armv7'; checksum='ba2186fd97c2e3f8930ee04bf01774938fc3682365fe4be70d9326f2b2a430f337c617f2c385aaa3d4e6dccb7ba980990d26cdc395574e6a5172c4f74cd9391d' ;; 		aarch64) binArch='arm64'; checksum='91b5d50cd5c0dd84bf7dfcc437880df0d39dc62af57574cea2b560000c5bf12ba415b8723c5cb091276a93b979249ff939d567fef3a2a6ed417f93af266effcc' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='f8aa3a478a989217a5f4e6b58936d2a69ffb99f2b7625760451ecab6fdc6d2534f815b8414a2121d63cdbea4f92022cebaa8550f9e3a61681ec25893ebf11ee6' ;; 		s390x)   binArch='s390x'; checksum='2c8f9b6b28194dcc14db98c0657f6a47f35dbfa6c0a45fc485b488ada7c5b77abb4f880d3763dac1699d1007ba8e0f622a075fc7f394a0f3898fb90883c00407' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 10 Nov 2022 21:30:12 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:30:12 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 10 Nov 2022 21:30:12 GMT
ENV XDG_DATA_HOME=/data
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Nov 2022 21:30:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 80
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 443
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 443/udp
# Thu, 10 Nov 2022 21:30:13 GMT
EXPOSE 2019
# Thu, 10 Nov 2022 21:30:14 GMT
WORKDIR /srv
# Thu, 10 Nov 2022 21:30:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480d8737fa00cd91dd0632e620ecb371ff8e7fbb7792619315f962bd74ac78b0`  
		Last Modified: Thu, 10 Nov 2022 21:30:38 GMT  
		Size: 304.5 KB (304513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8b251ca0b51f9a0e2defca59988fe0d152662e2a155d0861aa02e2a7257dd1`  
		Last Modified: Thu, 10 Nov 2022 21:30:38 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9543d07ca7897910ddae9b3fb026b4004353b71f3342f8889a2ecf194358ef65`  
		Last Modified: Thu, 10 Nov 2022 21:30:39 GMT  
		Size: 13.3 MB (13260509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e0320d2afc0181e222e9018c3ce159603f04d94ac7754b2c57e2a2f198a477`  
		Last Modified: Thu, 10 Nov 2022 21:30:37 GMT  
		Size: 154.0 B  
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

### `caddy:latest` - windows version 10.0.17763.3650; amd64

```console
$ docker pull caddy@sha256:1bb072f445e9d5154311ff5502f598bc04f8f3a39962ba84935c924372254023
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2794246589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09e5adcd59d9a3cef6ebbe389ca4ba29c5fd69972ae3e411b8be53d7267ce1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:09:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:09:11 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:10:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:10:28 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:10:29 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:10:30 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:10:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:10:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:10:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:10:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:10:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:10:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:10:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:10:38 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:10:39 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:10:40 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:10:41 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:11:42 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:11:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c991125a18c41d60a99d6ec86c4c38917cda31bdc78ae2b19547118e64c3130`  
		Last Modified: Wed, 09 Nov 2022 19:42:43 GMT  
		Size: 376.0 KB (375983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c44dcec78b9053b83e9d2b0b85793a2d6dd9f7882eda9b68af412bfc561ae59`  
		Last Modified: Wed, 09 Nov 2022 19:42:42 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679594f71e58468aa9805558e75d701d34727227835b6f244c3227d0e8b3fc51`  
		Last Modified: Wed, 09 Nov 2022 19:42:45 GMT  
		Size: 15.0 MB (14954096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ec8fe5018705645312e2f15ddeff4193348e2d162b522e3d89004171e32611`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de52b8df46e754f4b7a96b07b9fcec10bba34c5203824f45ad667524e900442`  
		Last Modified: Wed, 09 Nov 2022 19:42:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de92b977c1ec3484f7ec22f1caf0af85a365785ef5a626cd1306e02ba2d78514`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14440e034f493a00a52bd65e46382b25e372630456a4bab3984ef60887bd4b2`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7fa7a9304ad99e65a0da0a731b88f220461e17a0a0aefd95e4388273c22107`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4688f22612a7a65254ccf95adb7b14eb333413e66689770a1b2ee648df6ae7a`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04f66e90a6de69b5c69c165ab290a0f792549149c911eef51f26380bdac82f2`  
		Last Modified: Wed, 09 Nov 2022 19:42:38 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a779763f5c2179feba42c73a1b4ac83edb90462493ee5b369908d6e839520f8`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d1d0c12a2c947c8a5a1942711ea238b6899cbbde6dc2d4c32401e2f336ebc5`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9267ecd850272decf95a74353e3505335d6ca458bd2d604cf6fd08f36b42b36d`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0daba2c50a467fa60cd066c4a707a46479815f75be8ccee29e3ffd74089e29c`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3399f861f6994eed02f962f0dfe8919ff2c59d392b5ee7cf1a2374a3e42892`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b97c99b6c4d5675b3327c5f3a35c918b75ab8fb154b22797764b4620b444c0`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634fc965a18e1d74efa1e1e64a43388feca61231913a4e4b3784b0955c81d4ec`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a7f978fb624cd5a777948f956d64e0e5688bd12864fc178bad1fa89cdf12f5`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 305.8 KB (305758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8494101343a0a636a7e1246e9ac5417edfd30766fa9cc3accad02c260ae99e3`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.20348.1249; amd64

```console
$ docker pull caddy@sha256:df26460add1714658ae82eb674ccba73fd3781a29eb1c742153d7f848ba77b03
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2497915476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf8cd6c30b11c2e211f77bf1bd355ab239d0405d001159b36bf501643b70145`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:12:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:12:22 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:12:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:12:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:12:51 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:12:52 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:12:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:12:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:12:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:12:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:12:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:12:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:12:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:13:00 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:13:01 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:13:18 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:13:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1dc6b6b8064ce6aa320f7658f5ddc1b7eafa5e7b7ed6eaa07e0d8a1c990256`  
		Last Modified: Wed, 09 Nov 2022 19:43:12 GMT  
		Size: 617.3 KB (617258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad0e2bc53452df09c89858e4b2f54e4b23c0c8bb58733f05d9b0b3a5f39b1e8`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa3455b7b8e4ed55199abb0ad62eea75ab0ab47616504b3758f35aed63ccbc8`  
		Last Modified: Wed, 09 Nov 2022 19:43:15 GMT  
		Size: 15.2 MB (15168482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d64bc11b8e88956f2cdb7f937525a2fb1c986000887f4dc88dc1eea98446d81`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8502309666e15b454660c5bfd9d1ebd352e18c945b8b2ede9afe9269a5937b`  
		Last Modified: Wed, 09 Nov 2022 19:43:10 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906c51626faa981aaf141adb1be3e8e65cbe12d592fa3c640dc829d28abd4d00`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ee5c1d8d0fd98304b819d90c4adb33feb485f3f47dcf390bee532f8d6b57f4`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63fc79d12f01d2fad54fd51f43571f0aaef608b2d7be31823c881667cb5e41e`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad24427c4c7dcb96616f4886c985d9252699bbaf01bb7f1551a776f57ac3080`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce3623edb8a858ba8a0f7f2184802487aa72c8332935270dbb0308fbbd70c0`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8180ccb35cb5b71974dc1c9130892b1c8ab0f20309906215682be61e553596c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b759234e6db3ee8b177b51b148eeb2a3ef89bc496e3098d56322d6e17a269f3c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc80653154d31f3fad6c8977be60b10618022311edaf9a0cba8a6eee3428aa1`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19a3de5a545f51fc5ee391f49dc670b30e5d6814b0bd8195075243d1d5d2d52`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d26ee259e1db29592ba9e5d679d72c081eab360aed0add981ddf4a44d7c7b2`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732e7368e5a0068535b80c136d98d840daeba6d9dd5d7fe90bb39b10c9fab27f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da48319bd36cb22c79804c6e3e5efa4abb652e22c993fe7a5c98efc0d651240f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8bd93b51837b04ade762d05a59d24ed1f68d2a4cd612020a5915736d43aa6f`  
		Last Modified: Wed, 09 Nov 2022 19:43:05 GMT  
		Size: 337.0 KB (336999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51903721c05174a5370399be9cfbcdfafdc616c28d0599d67308b9a44b07d5d9`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:0a8af8e78d210109370f648e45b709e478abcdb65b491151144dc00c66fa5d39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3650; amd64
	-	windows version 10.0.20348.1249; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.3650; amd64

```console
$ docker pull caddy@sha256:1bb072f445e9d5154311ff5502f598bc04f8f3a39962ba84935c924372254023
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2794246589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09e5adcd59d9a3cef6ebbe389ca4ba29c5fd69972ae3e411b8be53d7267ce1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:09:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:09:11 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:10:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:10:28 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:10:29 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:10:30 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:10:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:10:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:10:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:10:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:10:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:10:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:10:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:10:38 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:10:39 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:10:40 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:10:41 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:11:42 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:11:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c991125a18c41d60a99d6ec86c4c38917cda31bdc78ae2b19547118e64c3130`  
		Last Modified: Wed, 09 Nov 2022 19:42:43 GMT  
		Size: 376.0 KB (375983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c44dcec78b9053b83e9d2b0b85793a2d6dd9f7882eda9b68af412bfc561ae59`  
		Last Modified: Wed, 09 Nov 2022 19:42:42 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679594f71e58468aa9805558e75d701d34727227835b6f244c3227d0e8b3fc51`  
		Last Modified: Wed, 09 Nov 2022 19:42:45 GMT  
		Size: 15.0 MB (14954096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ec8fe5018705645312e2f15ddeff4193348e2d162b522e3d89004171e32611`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de52b8df46e754f4b7a96b07b9fcec10bba34c5203824f45ad667524e900442`  
		Last Modified: Wed, 09 Nov 2022 19:42:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de92b977c1ec3484f7ec22f1caf0af85a365785ef5a626cd1306e02ba2d78514`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14440e034f493a00a52bd65e46382b25e372630456a4bab3984ef60887bd4b2`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7fa7a9304ad99e65a0da0a731b88f220461e17a0a0aefd95e4388273c22107`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4688f22612a7a65254ccf95adb7b14eb333413e66689770a1b2ee648df6ae7a`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04f66e90a6de69b5c69c165ab290a0f792549149c911eef51f26380bdac82f2`  
		Last Modified: Wed, 09 Nov 2022 19:42:38 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a779763f5c2179feba42c73a1b4ac83edb90462493ee5b369908d6e839520f8`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d1d0c12a2c947c8a5a1942711ea238b6899cbbde6dc2d4c32401e2f336ebc5`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9267ecd850272decf95a74353e3505335d6ca458bd2d604cf6fd08f36b42b36d`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0daba2c50a467fa60cd066c4a707a46479815f75be8ccee29e3ffd74089e29c`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3399f861f6994eed02f962f0dfe8919ff2c59d392b5ee7cf1a2374a3e42892`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b97c99b6c4d5675b3327c5f3a35c918b75ab8fb154b22797764b4620b444c0`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634fc965a18e1d74efa1e1e64a43388feca61231913a4e4b3784b0955c81d4ec`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a7f978fb624cd5a777948f956d64e0e5688bd12864fc178bad1fa89cdf12f5`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 305.8 KB (305758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8494101343a0a636a7e1246e9ac5417edfd30766fa9cc3accad02c260ae99e3`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.20348.1249; amd64

```console
$ docker pull caddy@sha256:df26460add1714658ae82eb674ccba73fd3781a29eb1c742153d7f848ba77b03
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2497915476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf8cd6c30b11c2e211f77bf1bd355ab239d0405d001159b36bf501643b70145`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:12:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:12:22 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:12:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:12:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:12:51 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:12:52 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:12:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:12:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:12:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:12:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:12:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:12:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:12:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:13:00 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:13:01 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:13:18 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:13:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1dc6b6b8064ce6aa320f7658f5ddc1b7eafa5e7b7ed6eaa07e0d8a1c990256`  
		Last Modified: Wed, 09 Nov 2022 19:43:12 GMT  
		Size: 617.3 KB (617258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad0e2bc53452df09c89858e4b2f54e4b23c0c8bb58733f05d9b0b3a5f39b1e8`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa3455b7b8e4ed55199abb0ad62eea75ab0ab47616504b3758f35aed63ccbc8`  
		Last Modified: Wed, 09 Nov 2022 19:43:15 GMT  
		Size: 15.2 MB (15168482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d64bc11b8e88956f2cdb7f937525a2fb1c986000887f4dc88dc1eea98446d81`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8502309666e15b454660c5bfd9d1ebd352e18c945b8b2ede9afe9269a5937b`  
		Last Modified: Wed, 09 Nov 2022 19:43:10 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906c51626faa981aaf141adb1be3e8e65cbe12d592fa3c640dc829d28abd4d00`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ee5c1d8d0fd98304b819d90c4adb33feb485f3f47dcf390bee532f8d6b57f4`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63fc79d12f01d2fad54fd51f43571f0aaef608b2d7be31823c881667cb5e41e`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad24427c4c7dcb96616f4886c985d9252699bbaf01bb7f1551a776f57ac3080`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce3623edb8a858ba8a0f7f2184802487aa72c8332935270dbb0308fbbd70c0`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8180ccb35cb5b71974dc1c9130892b1c8ab0f20309906215682be61e553596c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b759234e6db3ee8b177b51b148eeb2a3ef89bc496e3098d56322d6e17a269f3c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc80653154d31f3fad6c8977be60b10618022311edaf9a0cba8a6eee3428aa1`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19a3de5a545f51fc5ee391f49dc670b30e5d6814b0bd8195075243d1d5d2d52`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d26ee259e1db29592ba9e5d679d72c081eab360aed0add981ddf4a44d7c7b2`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732e7368e5a0068535b80c136d98d840daeba6d9dd5d7fe90bb39b10c9fab27f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da48319bd36cb22c79804c6e3e5efa4abb652e22c993fe7a5c98efc0d651240f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8bd93b51837b04ade762d05a59d24ed1f68d2a4cd612020a5915736d43aa6f`  
		Last Modified: Wed, 09 Nov 2022 19:43:05 GMT  
		Size: 337.0 KB (336999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51903721c05174a5370399be9cfbcdfafdc616c28d0599d67308b9a44b07d5d9`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:7d8fa3f8a84211c6129b53d25df161f198e739bb5f6e676467db0eafca8cda29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull caddy@sha256:1bb072f445e9d5154311ff5502f598bc04f8f3a39962ba84935c924372254023
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2794246589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09e5adcd59d9a3cef6ebbe389ca4ba29c5fd69972ae3e411b8be53d7267ce1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:09:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:09:11 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:10:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:10:28 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:10:29 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:10:30 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:10:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:10:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:10:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:10:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:10:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:10:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:10:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:10:38 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:10:39 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:10:40 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:10:41 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:11:42 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:11:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c991125a18c41d60a99d6ec86c4c38917cda31bdc78ae2b19547118e64c3130`  
		Last Modified: Wed, 09 Nov 2022 19:42:43 GMT  
		Size: 376.0 KB (375983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c44dcec78b9053b83e9d2b0b85793a2d6dd9f7882eda9b68af412bfc561ae59`  
		Last Modified: Wed, 09 Nov 2022 19:42:42 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679594f71e58468aa9805558e75d701d34727227835b6f244c3227d0e8b3fc51`  
		Last Modified: Wed, 09 Nov 2022 19:42:45 GMT  
		Size: 15.0 MB (14954096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ec8fe5018705645312e2f15ddeff4193348e2d162b522e3d89004171e32611`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de52b8df46e754f4b7a96b07b9fcec10bba34c5203824f45ad667524e900442`  
		Last Modified: Wed, 09 Nov 2022 19:42:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de92b977c1ec3484f7ec22f1caf0af85a365785ef5a626cd1306e02ba2d78514`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14440e034f493a00a52bd65e46382b25e372630456a4bab3984ef60887bd4b2`  
		Last Modified: Wed, 09 Nov 2022 19:42:41 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7fa7a9304ad99e65a0da0a731b88f220461e17a0a0aefd95e4388273c22107`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4688f22612a7a65254ccf95adb7b14eb333413e66689770a1b2ee648df6ae7a`  
		Last Modified: Wed, 09 Nov 2022 19:42:39 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04f66e90a6de69b5c69c165ab290a0f792549149c911eef51f26380bdac82f2`  
		Last Modified: Wed, 09 Nov 2022 19:42:38 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a779763f5c2179feba42c73a1b4ac83edb90462493ee5b369908d6e839520f8`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d1d0c12a2c947c8a5a1942711ea238b6899cbbde6dc2d4c32401e2f336ebc5`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9267ecd850272decf95a74353e3505335d6ca458bd2d604cf6fd08f36b42b36d`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0daba2c50a467fa60cd066c4a707a46479815f75be8ccee29e3ffd74089e29c`  
		Last Modified: Wed, 09 Nov 2022 19:42:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3399f861f6994eed02f962f0dfe8919ff2c59d392b5ee7cf1a2374a3e42892`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b97c99b6c4d5675b3327c5f3a35c918b75ab8fb154b22797764b4620b444c0`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634fc965a18e1d74efa1e1e64a43388feca61231913a4e4b3784b0955c81d4ec`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a7f978fb624cd5a777948f956d64e0e5688bd12864fc178bad1fa89cdf12f5`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 305.8 KB (305758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8494101343a0a636a7e1246e9ac5417edfd30766fa9cc3accad02c260ae99e3`  
		Last Modified: Wed, 09 Nov 2022 19:42:35 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:618d9f501fb56f3d12f4566a58de1afafc1a3920ba686c84cc2e1134d1bf41e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1249; amd64

### `caddy:windowsservercore-ltsc2022` - windows version 10.0.20348.1249; amd64

```console
$ docker pull caddy@sha256:df26460add1714658ae82eb674ccba73fd3781a29eb1c742153d7f848ba77b03
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2497915476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cf8cd6c30b11c2e211f77bf1bd355ab239d0405d001159b36bf501643b70145`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 18:12:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/8c5fc6fc265c5d8557f17a18b778c398a2c6f27b/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Nov 2022 18:12:22 GMT
ENV CADDY_VERSION=v2.6.2
# Wed, 09 Nov 2022 18:12:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.2/caddy_2.6.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('1454eb2de857fa091a00e62199bb5ea7840210a90a9b04f626f0cf3688cdf69ea736b497e3b8ac0f1b40bb9aba416bfa9e4eb9c33be166665ee0ce02a26cfd98')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Nov 2022 18:12:50 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Nov 2022 18:12:51 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Nov 2022 18:12:52 GMT
LABEL org.opencontainers.image.version=v2.6.2
# Wed, 09 Nov 2022 18:12:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Nov 2022 18:12:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Nov 2022 18:12:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Nov 2022 18:12:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Nov 2022 18:12:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Nov 2022 18:12:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Nov 2022 18:12:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Nov 2022 18:13:00 GMT
EXPOSE 80
# Wed, 09 Nov 2022 18:13:01 GMT
EXPOSE 443
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 443/udp
# Wed, 09 Nov 2022 18:13:02 GMT
EXPOSE 2019
# Wed, 09 Nov 2022 18:13:18 GMT
RUN caddy version
# Wed, 09 Nov 2022 18:13:19 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1dc6b6b8064ce6aa320f7658f5ddc1b7eafa5e7b7ed6eaa07e0d8a1c990256`  
		Last Modified: Wed, 09 Nov 2022 19:43:12 GMT  
		Size: 617.3 KB (617258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad0e2bc53452df09c89858e4b2f54e4b23c0c8bb58733f05d9b0b3a5f39b1e8`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa3455b7b8e4ed55199abb0ad62eea75ab0ab47616504b3758f35aed63ccbc8`  
		Last Modified: Wed, 09 Nov 2022 19:43:15 GMT  
		Size: 15.2 MB (15168482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d64bc11b8e88956f2cdb7f937525a2fb1c986000887f4dc88dc1eea98446d81`  
		Last Modified: Wed, 09 Nov 2022 19:43:11 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8502309666e15b454660c5bfd9d1ebd352e18c945b8b2ede9afe9269a5937b`  
		Last Modified: Wed, 09 Nov 2022 19:43:10 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906c51626faa981aaf141adb1be3e8e65cbe12d592fa3c640dc829d28abd4d00`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ee5c1d8d0fd98304b819d90c4adb33feb485f3f47dcf390bee532f8d6b57f4`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63fc79d12f01d2fad54fd51f43571f0aaef608b2d7be31823c881667cb5e41e`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad24427c4c7dcb96616f4886c985d9252699bbaf01bb7f1551a776f57ac3080`  
		Last Modified: Wed, 09 Nov 2022 19:43:09 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce3623edb8a858ba8a0f7f2184802487aa72c8332935270dbb0308fbbd70c0`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8180ccb35cb5b71974dc1c9130892b1c8ab0f20309906215682be61e553596c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b759234e6db3ee8b177b51b148eeb2a3ef89bc496e3098d56322d6e17a269f3c`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc80653154d31f3fad6c8977be60b10618022311edaf9a0cba8a6eee3428aa1`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19a3de5a545f51fc5ee391f49dc670b30e5d6814b0bd8195075243d1d5d2d52`  
		Last Modified: Wed, 09 Nov 2022 19:43:07 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d26ee259e1db29592ba9e5d679d72c081eab360aed0add981ddf4a44d7c7b2`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732e7368e5a0068535b80c136d98d840daeba6d9dd5d7fe90bb39b10c9fab27f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da48319bd36cb22c79804c6e3e5efa4abb652e22c993fe7a5c98efc0d651240f`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8bd93b51837b04ade762d05a59d24ed1f68d2a4cd612020a5915736d43aa6f`  
		Last Modified: Wed, 09 Nov 2022 19:43:05 GMT  
		Size: 337.0 KB (336999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51903721c05174a5370399be9cfbcdfafdc616c28d0599d67308b9a44b07d5d9`  
		Last Modified: Wed, 09 Nov 2022 19:43:04 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
