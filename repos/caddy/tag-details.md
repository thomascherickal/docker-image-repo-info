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
-	[`caddy:2.4.2`](#caddy242)
-	[`caddy:2.4.2-alpine`](#caddy242-alpine)
-	[`caddy:2.4.2-builder`](#caddy242-builder)
-	[`caddy:2.4.2-builder-alpine`](#caddy242-builder-alpine)
-	[`caddy:2.4.2-builder-windowsservercore-1809`](#caddy242-builder-windowsservercore-1809)
-	[`caddy:2.4.2-builder-windowsservercore-ltsc2016`](#caddy242-builder-windowsservercore-ltsc2016)
-	[`caddy:2.4.2-windowsservercore`](#caddy242-windowsservercore)
-	[`caddy:2.4.2-windowsservercore-1809`](#caddy242-windowsservercore-1809)
-	[`caddy:2.4.2-windowsservercore-ltsc2016`](#caddy242-windowsservercore-ltsc2016)
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
$ docker pull caddy@sha256:31493fd55da69e11db44f6acbd0c92070187cfd61dd0a5bfe17a0f6aa7b894d2
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
$ docker pull caddy@sha256:c3176ebaceec5d64a4892205d7cf3d32da87e2fcbbb8a47d787ef4200ef0e6d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14649179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57e953391a547aacb19ba079ee6713b24b8400352d6d95a8a43e79fb035ec0f7`
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
# Mon, 14 Jun 2021 17:19:37 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:19:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:19:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:19:41 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:19:41 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:19:41 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:19:41 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:19:41 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:19:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:19:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:19:43 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:19:43 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:19:43 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:19:44 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:19:44 GMT
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
	-	`sha256:037bdadcf837298422d86bb75d10aa9ea21eaaf0969e1d8e99b730b07208eb03`  
		Last Modified: Mon, 14 Jun 2021 17:20:16 GMT  
		Size: 11.5 MB (11530800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9785de7e5400398efa43aedd6416426c14e3101f52a5930b52b6e8ea3a0cd96`  
		Last Modified: Mon, 14 Jun 2021 17:20:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:53bc8c15c11306be1cd426dffb91df56e5dc186ae54c22eb08996f14c647378f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13817125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dd81d0e3a6035d5df068c9af8811281698921854e5190944b1f7a079651bb7d`
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
# Mon, 14 Jun 2021 17:49:40 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:49:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:49:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:49:44 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:49:44 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:49:44 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:49:44 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:49:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:49:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:49:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:49:46 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:49:46 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:49:47 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:49:47 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:49:47 GMT
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
	-	`sha256:028e0db410d042e12d6b3f64499cc00ae7298c02382ba1105cdc5ee03aaed549`  
		Last Modified: Mon, 14 Jun 2021 17:50:59 GMT  
		Size: 10.9 MB (10888459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64dbe91d32616efff4ec27f049638b231cfd0091a68480d45a21791d44b469c`  
		Last Modified: Mon, 14 Jun 2021 17:50:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:6fc967765fceab93d7838f17d2eeceddc56e21a65654e3ba92c799437ff09280
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13593827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d1b6dc4a59a634275f3c206036245997415a7d1894697b43d1dadc232712e8e`
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
# Mon, 14 Jun 2021 17:57:41 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:57:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:57:44 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:57:45 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:57:45 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:57:45 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:57:45 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:57:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:57:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:57:47 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:57:47 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:57:48 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:57:48 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:57:48 GMT
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
	-	`sha256:e97e805578bb88faf1e3b052fe899c9818d27e0e114574198d5e3d45a8faf1b9`  
		Last Modified: Mon, 14 Jun 2021 17:59:01 GMT  
		Size: 10.9 MB (10864008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee92873b0980eae80c33cd1bd74d1b35754b48c89cbe68088f4e98b4dd04e2f`  
		Last Modified: Mon, 14 Jun 2021 17:58:59 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:1f49cc95c1e8ebd7fe139595b64b8d3b2cbdafff4c46ff46bc4516054a50e3ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13466108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:749cdbfee8dde296c03efb611b07c067ca297771a1314bbcbbba992429e899e7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:32:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 15 Jun 2021 22:32:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 15 Jun 2021 22:32:20 GMT
ENV CADDY_VERSION=v2.4.2
# Tue, 15 Jun 2021 22:32:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 15 Jun 2021 22:32:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:32:23 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 15 Jun 2021 22:32:24 GMT
ENV XDG_DATA_HOME=/data
# Tue, 15 Jun 2021 22:32:24 GMT
VOLUME [/config]
# Tue, 15 Jun 2021 22:32:24 GMT
VOLUME [/data]
# Tue, 15 Jun 2021 22:32:24 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Tue, 15 Jun 2021 22:32:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 15 Jun 2021 22:32:26 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 15 Jun 2021 22:32:26 GMT
EXPOSE 80
# Tue, 15 Jun 2021 22:32:26 GMT
EXPOSE 443
# Tue, 15 Jun 2021 22:32:26 GMT
EXPOSE 2019
# Tue, 15 Jun 2021 22:32:26 GMT
WORKDIR /srv
# Tue, 15 Jun 2021 22:32:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d0b72044755ebd2b829600b94a69aa9096bbb4bf9a01c1795b5b245261b99a`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 300.6 KB (300631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abde659ccf1d73128ef1e71a9701b014e0f27d4abf15b3d410d0474cdd0adb95`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0b93549f9104a9bb517f1ae15bd6ef4d44f83d21964728c50aa960b97098dc`  
		Last Modified: Tue, 15 Jun 2021 22:33:26 GMT  
		Size: 10.4 MB (10447450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69a851000e14247059ab07104ab76f86231aaa1a4fb5abb6b321e66a45003d3`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:7764cdcd665f8e23165bf385240e8951ab046dd6f54808b247b57e284882ecc5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13175121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c3b2d52d66b7076e6c98e715324384114a94b978294b836f566919d77faa909`
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
# Mon, 14 Jun 2021 18:16:57 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:17:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 18:17:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 18:17:56 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 18:18:00 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 18:18:08 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 18:18:15 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 18:18:26 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:18:36 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:18:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:18:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:18:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:19:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:19:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:19:27 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:19:32 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:19:38 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:19:43 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:19:49 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 18:19:56 GMT
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
	-	`sha256:d23e936288e88eac2d5280068486ab71f9023047b51d2c012a09fd305cc70e19`  
		Last Modified: Mon, 14 Jun 2021 18:21:33 GMT  
		Size: 10.1 MB (10053418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59596542df0c41e54f99fa862419a9f75ef8cfce5b1788110d747951a295518e`  
		Last Modified: Mon, 14 Jun 2021 18:21:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:c8d5cda3a4ef8a3fae917a732cd349372b1cc625071f9b3acc77a9033eb55e63
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14004446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5539a479891dabbacf899df4a9c0af209caf5e8b82799b452efd5c9093bd99`
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
# Mon, 14 Jun 2021 17:41:42 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:41:46 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:41:46 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:41:46 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:41:47 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:41:49 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:41:49 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:41:49 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:41:49 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:41:50 GMT
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
	-	`sha256:9b59880ffc79bf424b9fb38c497ec3d3edea77c4cbabb6b295bad830e4732008`  
		Last Modified: Mon, 14 Jun 2021 17:42:22 GMT  
		Size: 11.1 MB (11094948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4a0a3f3a72f3127538116c7943809378ae5921f09f19249fb98a578d261a49`  
		Last Modified: Mon, 14 Jun 2021 17:42:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:84c41546a31938e07bc74b9535459f62221b5fa62f50aadb3f7138ceb0a638b7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2654297157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7933e1b45a92be68914695f31f1c84c86b602c5233536557c1ccee877d1216b0`
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
# Mon, 14 Jun 2021 18:15:56 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:16:40 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8d5cf4479e471d47fd067ce2fbe34c2015a96caedab95ca042aeb633956cbc2bb89c1bc4fe6593c1f96ca58bc66b21f32caa6b099122b9d500a3902245fa5105')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 14 Jun 2021 18:16:43 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 14 Jun 2021 18:16:45 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 14 Jun 2021 18:16:48 GMT
VOLUME [c:/config]
# Mon, 14 Jun 2021 18:16:50 GMT
VOLUME [c:/data]
# Mon, 14 Jun 2021 18:16:53 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:16:55 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:16:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:17:01 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:17:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:17:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:17:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:17:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:17:15 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:17:17 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:17:20 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:17:39 GMT
RUN caddy version
# Mon, 14 Jun 2021 18:17:41 GMT
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
	-	`sha256:07802e3c606e3b9298421527979a2b9797c286d601553a4f8c11271d67919b58`  
		Last Modified: Mon, 14 Jun 2021 18:25:04 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4847967ab228abb45531c45132179ebac7d55ea85bf85ea3f3f420aff0be2863`  
		Last Modified: Mon, 14 Jun 2021 18:25:17 GMT  
		Size: 12.0 MB (12025127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e590a115b7ca0fdadc5a634f9a3b1a58db5ac8a89765f1d00351421045e7dd62`  
		Last Modified: Mon, 14 Jun 2021 18:25:03 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a698c5067c38c742726c5f427f5f07d028e7768a91c4f2fd9a973f662a750b0`  
		Last Modified: Mon, 14 Jun 2021 18:25:03 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4d9bb89edb4e6f90cfacbb81068b117b3b8affe4430a23ddc2f8aa8b1803fa`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369f1dad8944bfe55423327ebaedf96f73e356ca6fd92d4e9a8d2fdbc6b6293c`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f126fec1b223ee19a7f02455cd95a68d8275a8589273ff50b9f7ffbad72a882`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3949035d30e3b80897ac6fc2b4776dccd30680886816cfe8c27ed8bc8c0c595`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c1d9637c1841b64adc5cccf8a5ce5275754886c8c7eb26005eef69727bc101`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa902629ee85278422f20ba99ecc504972ce7c6263bdfa5f1d0a51103ed3e272`  
		Last Modified: Mon, 14 Jun 2021 18:24:59 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7795b0b452df39f057bb8fb233e6862dba05177f3c225da1443588e4e7ec3326`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b936a424e3378bda5aaa142367741f0486702c00117d08a527d36f3876cc7a0`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74ede6be2a18e8c915b5e55628de5a029cf0bb5b69edc917dd8f1c6e1426ee6`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cdf00e847ddd24f1ba768e20fd224aa86a161461a82d3a210f1d5ce1f28cb2`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51405f73ce954be2e339c2cfa1a28109cd371d9fb8986047079a8ba8cc4a9d7a`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38f74dca7b51152c809bf35c007d8affbfc36cae366903110509bdba8f3bde6`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca41d82a7c33c949c331f1ff7958f3ec1551f1bda90faaf07d7b112111a251bc`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582046a83a61d6a9e5701d72c1102b19e9e9ba65665c38d03618e34acdaa5c36`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 300.2 KB (300242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a16f8caea000f3748f024fd14e1419c77091e71e4c220b06a94dc02ffc746c`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:4d5c4f12af6b434f907c262accbfeef1c9eb948d91bb5113bde117904152d9bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278396558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b0d047c64024dd8b9ee7374a59e2e19a219277308f3db92d25f22e903b4f6fb`
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
# Mon, 14 Jun 2021 18:17:52 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:19:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8d5cf4479e471d47fd067ce2fbe34c2015a96caedab95ca042aeb633956cbc2bb89c1bc4fe6593c1f96ca58bc66b21f32caa6b099122b9d500a3902245fa5105')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 14 Jun 2021 18:19:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 14 Jun 2021 18:19:41 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 14 Jun 2021 18:19:43 GMT
VOLUME [c:/config]
# Mon, 14 Jun 2021 18:19:46 GMT
VOLUME [c:/data]
# Mon, 14 Jun 2021 18:19:48 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:19:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:19:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:19:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:19:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:20:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:20:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:20:04 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:20:07 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:20:09 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:20:11 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:21:14 GMT
RUN caddy version
# Mon, 14 Jun 2021 18:21:17 GMT
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
	-	`sha256:5bd5fde0219b866984e02c69748a7c533734e7d3ce1c605e00b2794ba719ca78`  
		Last Modified: Mon, 14 Jun 2021 18:25:40 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ff67696fba822eac7dc90ce8b74a3463e180c1277ce1b5235dd553efd54d37`  
		Last Modified: Mon, 14 Jun 2021 18:25:53 GMT  
		Size: 12.0 MB (12011979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb05b150667473f58bd9ff97143e7addb941c15c23d7c0190462052e171a5d3`  
		Last Modified: Mon, 14 Jun 2021 18:25:40 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417ec686bccf8c11c7e167450f76c56e965e0d895b8a67d2959fa0cd8e0f46c6`  
		Last Modified: Mon, 14 Jun 2021 18:25:39 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e7f7e817f7b000e684b2477e658283e3bc5e32f705e2a1af3eb2171451ab1a`  
		Last Modified: Mon, 14 Jun 2021 18:25:38 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9adbfef5bd1c4ce567e8643e7eb3ac228fc89e60afffa0d4ad65188836ee10e`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46951e23f2c6f042a74af530655917c470e7e58bd428811bea889f06ece060f3`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b702d713b07cb19c098b0a4c2ad22de8111ab140c99b88deb21ffa5f10870f`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1554c780202a1e2bfb6cafbf73148847f97c535c407f63f750903997105d516f`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a72ab2ef98ce84364537328634d5a56cb6c9080cdec9988778c0e15d451dc51`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0cb0fb150ef4d4bb3e78339539c6453dcdf1d1b11d50728bb72e262b603fa9`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d8666b345f227a53b8d4cc8698ebe05b454caf116f8329e30d4328ba56896e`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bce3d7ad9504e8b1a2a5f46b50605a7e895686efeae62529b2fb0c8210a2e7`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d806bd36723a790387c5f61446d9b73da291b1e1592e6943b28686f3dc50fb39`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddf127d6e3c5443190a309b2f703cfd1d079beea71723b1507958dbbf2b5cab`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace91f2d94fe0fd5d53fce078d832db72cc38e2ef7692a44f57f9377dcbf3f8f`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f8adfaab4745797ca3869f6e54a87e5c399e56609635f7b74b039fb8f9fc00`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca3d4ed717fc9e7154ad94da8a5ea30b61ba4dfe9ec25bdcfcb55e6291cbec7`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 274.6 KB (274630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deafc6c05519d23d4709cd8504c83ff6c43943477ddcaf57ae7a871acdbdf489`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:2a518987da6ad50fba4fa2ce40b159460bc68d42e4d37c7784c118470e738821
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
$ docker pull caddy@sha256:c3176ebaceec5d64a4892205d7cf3d32da87e2fcbbb8a47d787ef4200ef0e6d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14649179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57e953391a547aacb19ba079ee6713b24b8400352d6d95a8a43e79fb035ec0f7`
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
# Mon, 14 Jun 2021 17:19:37 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:19:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:19:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:19:41 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:19:41 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:19:41 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:19:41 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:19:41 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:19:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:19:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:19:43 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:19:43 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:19:43 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:19:44 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:19:44 GMT
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
	-	`sha256:037bdadcf837298422d86bb75d10aa9ea21eaaf0969e1d8e99b730b07208eb03`  
		Last Modified: Mon, 14 Jun 2021 17:20:16 GMT  
		Size: 11.5 MB (11530800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9785de7e5400398efa43aedd6416426c14e3101f52a5930b52b6e8ea3a0cd96`  
		Last Modified: Mon, 14 Jun 2021 17:20:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:53bc8c15c11306be1cd426dffb91df56e5dc186ae54c22eb08996f14c647378f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13817125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dd81d0e3a6035d5df068c9af8811281698921854e5190944b1f7a079651bb7d`
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
# Mon, 14 Jun 2021 17:49:40 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:49:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:49:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:49:44 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:49:44 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:49:44 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:49:44 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:49:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:49:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:49:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:49:46 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:49:46 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:49:47 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:49:47 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:49:47 GMT
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
	-	`sha256:028e0db410d042e12d6b3f64499cc00ae7298c02382ba1105cdc5ee03aaed549`  
		Last Modified: Mon, 14 Jun 2021 17:50:59 GMT  
		Size: 10.9 MB (10888459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64dbe91d32616efff4ec27f049638b231cfd0091a68480d45a21791d44b469c`  
		Last Modified: Mon, 14 Jun 2021 17:50:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:6fc967765fceab93d7838f17d2eeceddc56e21a65654e3ba92c799437ff09280
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13593827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d1b6dc4a59a634275f3c206036245997415a7d1894697b43d1dadc232712e8e`
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
# Mon, 14 Jun 2021 17:57:41 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:57:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:57:44 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:57:45 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:57:45 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:57:45 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:57:45 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:57:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:57:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:57:47 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:57:47 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:57:48 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:57:48 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:57:48 GMT
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
	-	`sha256:e97e805578bb88faf1e3b052fe899c9818d27e0e114574198d5e3d45a8faf1b9`  
		Last Modified: Mon, 14 Jun 2021 17:59:01 GMT  
		Size: 10.9 MB (10864008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee92873b0980eae80c33cd1bd74d1b35754b48c89cbe68088f4e98b4dd04e2f`  
		Last Modified: Mon, 14 Jun 2021 17:58:59 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:1f49cc95c1e8ebd7fe139595b64b8d3b2cbdafff4c46ff46bc4516054a50e3ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13466108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:749cdbfee8dde296c03efb611b07c067ca297771a1314bbcbbba992429e899e7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:32:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 15 Jun 2021 22:32:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 15 Jun 2021 22:32:20 GMT
ENV CADDY_VERSION=v2.4.2
# Tue, 15 Jun 2021 22:32:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 15 Jun 2021 22:32:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:32:23 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 15 Jun 2021 22:32:24 GMT
ENV XDG_DATA_HOME=/data
# Tue, 15 Jun 2021 22:32:24 GMT
VOLUME [/config]
# Tue, 15 Jun 2021 22:32:24 GMT
VOLUME [/data]
# Tue, 15 Jun 2021 22:32:24 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Tue, 15 Jun 2021 22:32:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 15 Jun 2021 22:32:26 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 15 Jun 2021 22:32:26 GMT
EXPOSE 80
# Tue, 15 Jun 2021 22:32:26 GMT
EXPOSE 443
# Tue, 15 Jun 2021 22:32:26 GMT
EXPOSE 2019
# Tue, 15 Jun 2021 22:32:26 GMT
WORKDIR /srv
# Tue, 15 Jun 2021 22:32:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d0b72044755ebd2b829600b94a69aa9096bbb4bf9a01c1795b5b245261b99a`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 300.6 KB (300631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abde659ccf1d73128ef1e71a9701b014e0f27d4abf15b3d410d0474cdd0adb95`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0b93549f9104a9bb517f1ae15bd6ef4d44f83d21964728c50aa960b97098dc`  
		Last Modified: Tue, 15 Jun 2021 22:33:26 GMT  
		Size: 10.4 MB (10447450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69a851000e14247059ab07104ab76f86231aaa1a4fb5abb6b321e66a45003d3`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:7764cdcd665f8e23165bf385240e8951ab046dd6f54808b247b57e284882ecc5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13175121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c3b2d52d66b7076e6c98e715324384114a94b978294b836f566919d77faa909`
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
# Mon, 14 Jun 2021 18:16:57 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:17:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 18:17:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 18:17:56 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 18:18:00 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 18:18:08 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 18:18:15 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 18:18:26 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:18:36 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:18:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:18:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:18:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:19:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:19:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:19:27 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:19:32 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:19:38 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:19:43 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:19:49 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 18:19:56 GMT
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
	-	`sha256:d23e936288e88eac2d5280068486ab71f9023047b51d2c012a09fd305cc70e19`  
		Last Modified: Mon, 14 Jun 2021 18:21:33 GMT  
		Size: 10.1 MB (10053418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59596542df0c41e54f99fa862419a9f75ef8cfce5b1788110d747951a295518e`  
		Last Modified: Mon, 14 Jun 2021 18:21:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:c8d5cda3a4ef8a3fae917a732cd349372b1cc625071f9b3acc77a9033eb55e63
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14004446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5539a479891dabbacf899df4a9c0af209caf5e8b82799b452efd5c9093bd99`
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
# Mon, 14 Jun 2021 17:41:42 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:41:46 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:41:46 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:41:46 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:41:47 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:41:49 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:41:49 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:41:49 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:41:49 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:41:50 GMT
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
	-	`sha256:9b59880ffc79bf424b9fb38c497ec3d3edea77c4cbabb6b295bad830e4732008`  
		Last Modified: Mon, 14 Jun 2021 17:42:22 GMT  
		Size: 11.1 MB (11094948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4a0a3f3a72f3127538116c7943809378ae5921f09f19249fb98a578d261a49`  
		Last Modified: Mon, 14 Jun 2021 17:42:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:3bef1d372a9949d4c020af490ed84a192382df2217da31603fc31b5acb200ba8
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
$ docker pull caddy@sha256:03ffe16fc60ddb7be4684d7c3c8e257038b2c00864c027415e8b05fc120c28d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.9 MB (116937549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d58d2ab3ddba126c2fd014ebdac7030a6d1c5eac1d0c5ea0ac1509d9c8c882d`
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
# Thu, 10 Jun 2021 21:26:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:26:40 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:26:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:26:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:26:42 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:19:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:19:01 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:19:48 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:19:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:19:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:19:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:19:50 GMT
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
	-	`sha256:e25adedf14febf43281fc3b4750e8b0c50f2bb061ef8f5e16a829d3392fa447b`  
		Last Modified: Thu, 10 Jun 2021 21:35:42 GMT  
		Size: 106.1 MB (106136761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52c85161d43b0fdd8bb3ae8fdf77b9e4fc783bceb11f591ed3bbdf1e4722abd`  
		Last Modified: Thu, 10 Jun 2021 21:35:26 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20d66408196d46dd8f1b9f81fb5afa2219f5ca4c68a313ca1c49d3b908f755d`  
		Last Modified: Thu, 10 Jun 2021 23:19:40 GMT  
		Size: 6.4 MB (6395665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84f14058db07dc0560a9f209a7d8768b4ebd80f1426006dec9fe3b4d7c7bd25`  
		Last Modified: Mon, 14 Jun 2021 17:20:29 GMT  
		Size: 1.3 MB (1311168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86b5f727a9d842c09b761d61887e9298328559147dd8e911eb7c5f6fcf5bfc2`  
		Last Modified: Mon, 14 Jun 2021 17:20:29 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:af84e4e4719a6f04129f95de4a1dadacacae55e4b82f98cc9f883020f40860da
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.7 MB (112708776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbae3456b30daef0a0988bb5200978e3a8b2981efecdd2f7a811c692ed7bcc6d`
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
# Thu, 10 Jun 2021 22:01:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 22:01:50 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 22:01:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 22:01:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 22:01:52 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:15:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:15:37 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:49:58 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:49:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:49:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:49:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:50:00 GMT
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
	-	`sha256:f6a122050eb4da5951b1c88f56bfe65cb0c1a50d4e9869ad63787a8d0fc9ff1e`  
		Last Modified: Thu, 10 Jun 2021 22:15:45 GMT  
		Size: 102.4 MB (102351924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc08c6e1815e1794433258a6a0a93785a234db42641d49902c4f194c1d6abc82`  
		Last Modified: Thu, 10 Jun 2021 22:15:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2e5491ca84af37b9bdc0dfcb0a65b798aea4ab080785e1bba16e36672accd4`  
		Last Modified: Thu, 10 Jun 2021 23:16:52 GMT  
		Size: 6.2 MB (6230941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cecdb7ddd0ec1710ae049c902367f06a18606501ca9d1dbe17ec00349029fb8`  
		Last Modified: Mon, 14 Jun 2021 17:51:16 GMT  
		Size: 1.2 MB (1221680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1729fe2ea9a0baa2a26bc61d595958dcecfcb3f577dcebaca53051ec502bf397`  
		Last Modified: Mon, 14 Jun 2021 17:51:16 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2a428d87d883958655e8d72e6461ed205031fac28d71b943746dda7178f2e555
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.6 MB (111602497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da4e596b14ba8264520d8c3f799a567c9b7f3847ae587434759e51d9c667bf76`
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
# Thu, 10 Jun 2021 22:35:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 22:35:30 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 22:35:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 22:35:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 22:35:32 GMT
WORKDIR /go
# Fri, 11 Jun 2021 00:34:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Jun 2021 00:34:12 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:57:59 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:57:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:58:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:58:01 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:58:01 GMT
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
	-	`sha256:3e05d01ffccbffea159372f8065e42d62b484e73624dae1b567d908c12bb6fa3`  
		Last Modified: Thu, 10 Jun 2021 22:53:44 GMT  
		Size: 102.1 MB (102116599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9c0e093faea54528f8e070b0ad60f87674bf3a4654d312ccf7d110de2a6f6a`  
		Last Modified: Thu, 10 Jun 2021 22:53:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59aa8029ac012f4886ea6bced5e66e03743aff8bd41e8c7413cab0369c79c91b`  
		Last Modified: Fri, 11 Jun 2021 00:35:26 GMT  
		Size: 5.6 MB (5560992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a1e9ca701d6638943ef23a3969d9ba902fada02c041a3a797515d585882566`  
		Last Modified: Mon, 14 Jun 2021 17:59:18 GMT  
		Size: 1.2 MB (1219508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017f9bacdf7cdb13305fcaf052511ab74f9d9d2b9cbae1253957277cdb6cdd48`  
		Last Modified: Mon, 14 Jun 2021 17:59:17 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b0e22365417fa304ab483e3f2da3c7b79886ee3bced561c8113dd66b4e664fec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112151491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14b18c1aa44d74288d99db407cad68df0fb403a47cdad522a7524f856bb773f4`
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
# Thu, 10 Jun 2021 21:45:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:45:54 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:45:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:45:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:45:55 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:04:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:04:40 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:39:47 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:39:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:39:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:39:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:39:49 GMT
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
	-	`sha256:a9da95e357649360250671b270e39318d13b2ddff5d5aaac20081d588c9b6f74`  
		Last Modified: Thu, 10 Jun 2021 21:55:04 GMT  
		Size: 101.5 MB (101471730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a246c0d2a229c1d281fc3c1c9aa7fe651a820da43e66cd7ab7660e606d8d9824`  
		Last Modified: Thu, 10 Jun 2021 21:54:43 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2518188a669fe97c7d7feaf8a0ef8974bd167bc206832dc95bae562e6d972fe6`  
		Last Modified: Thu, 10 Jun 2021 23:05:37 GMT  
		Size: 6.5 MB (6483980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cb2ec8e0329ac1e5a6a5f1146f63479477cd73be5c2a0a676a12b3fda9485f`  
		Last Modified: Mon, 14 Jun 2021 17:40:46 GMT  
		Size: 1.2 MB (1201544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3538e34014117eaf3a7b09c03f2fcc11383c7bcebc701bcdfbf5a2a2a61906bb`  
		Last Modified: Mon, 14 Jun 2021 17:40:45 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:f8fc6696fb7cd73549cdc80e5889efd4c9ba480b9622ffe9f316c6e32b6068dc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (111016742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cbbf856cae07e092449ff2a67b42618d6082d532dec5969a4bfa5089b96b11c`
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
# Thu, 10 Jun 2021 21:27:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:27:48 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:27:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:28:04 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:28:11 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:16:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:16:36 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 18:20:23 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:20:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 18:20:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 18:20:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 18:20:58 GMT
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
	-	`sha256:c81f5fe451abbc39d3bdfca4378da5aa2c8b041d846b68db7b6004029734d919`  
		Last Modified: Thu, 10 Jun 2021 21:41:32 GMT  
		Size: 99.9 MB (99918197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9387c57f22b360d0c37409febd5288b34f77782689d3995e0092564a035eae10`  
		Last Modified: Thu, 10 Jun 2021 21:41:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af95f6a2bbd2f3bf752226a7020c5dcb4ba9e36df520e5b7dac8913f4f852d6e`  
		Last Modified: Thu, 10 Jun 2021 23:18:16 GMT  
		Size: 6.8 MB (6830748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994f06d8c6a86a071bc59b2d0644e6c4118c2a51d61edbf571623d36f9b1b987`  
		Last Modified: Mon, 14 Jun 2021 18:21:51 GMT  
		Size: 1.2 MB (1170526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54fa15ba38d0d74a3579bc4af43b527cc19bc368e7351ccaf85c90264bfc31c`  
		Last Modified: Mon, 14 Jun 2021 18:21:50 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:2d70ee7ce742b7eba9d3c4097f0ee5448f02a40e7cc10514c12bbd3272fa7448
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115888076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f08a6df8ec993ccbd835eee259d75804dc13b90f39ad9dccd7971136aecb356`
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
# Thu, 10 Jun 2021 21:52:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:52:35 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:52:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:52:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:52:38 GMT
WORKDIR /go
# Thu, 10 Jun 2021 22:58:58 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 22:58:59 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:41:55 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:41:55 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:41:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:41:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:41:57 GMT
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
	-	`sha256:4b203e6fc30bb6c460e0aea06ed2a200569017655c2678db9ce6fed7a17762cc`  
		Last Modified: Thu, 10 Jun 2021 22:03:02 GMT  
		Size: 105.3 MB (105259453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9fa95d716a4e0cf3f1602cd1def2172371118109ba036c7d525ac506357a1b`  
		Last Modified: Thu, 10 Jun 2021 22:02:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1ceddc3358bec9a3e7284afbcb0a578916db67c3a60fbc269cf78c11f26623`  
		Last Modified: Thu, 10 Jun 2021 22:59:42 GMT  
		Size: 6.5 MB (6479018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab4e3358d5deaa72e1a9a5207c52a6f1133bd89e6c424bb9cf4f0b9fbf2e5b6`  
		Last Modified: Mon, 14 Jun 2021 17:42:29 GMT  
		Size: 1.3 MB (1264529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29212836bbaacf27e155ad8002b1c2a6b5cd2dbe13986b27a57dc427357f2ce`  
		Last Modified: Mon, 14 Jun 2021 17:42:29 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:32914545de594aa79ff4231b61d5594f830641d124fb3cfa56e0575e940ec569
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2808449608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f1d0a4465ebc0bcefa7e5556bfb70eddabb69cf27ef61b558f45bef720fe883`
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
# Mon, 14 Jun 2021 18:21:36 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:21:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 18:22:12 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 14 Jun 2021 18:22:15 GMT
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
	-	`sha256:92f879ad577a7254271b2a27970912d5990740c6c23b65c14d3585b0b331b6b1`  
		Last Modified: Mon, 14 Jun 2021 18:26:07 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14bceb7d820e8f377e4a2d219ae96ee84dafd1055c85c1ce3deb22ea38cb8bf`  
		Last Modified: Mon, 14 Jun 2021 18:26:07 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ddb113a61bc728c0f730228bd4b782a04bcd9bec04ca60a8f46ca5b82e827a8`  
		Last Modified: Mon, 14 Jun 2021 18:26:08 GMT  
		Size: 1.7 MB (1730897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f05c3ba05a4dc7082b32ebd8dae3976fd8adb32927054b6fc0e3f137970df1`  
		Last Modified: Mon, 14 Jun 2021 18:26:07 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:3dc1e8d5170dfd5b5e6fbb34d885db2414827f33c49ca301aaaa82644bb7a6fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6437016101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:913b54138653e16a37ea51c2051dd30d0bc4ff76fece599b23b92c1aa7a11ff3`
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
# Mon, 14 Jun 2021 18:22:30 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:22:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 18:24:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 14 Jun 2021 18:24:02 GMT
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
	-	`sha256:3d01a14f10d204dac3535ad62c6b042cc9edc8c2c7c0996ecc45efbb896d5eed`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612bbd13a883cfddbf2977f7de24716a7978eea9f601ba5854f82d36f10068c4`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40a20ce35485bdd147339935426465c403bd3c52351030d040de662cec3253b`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.7 MB (1700121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a492d6062ee0783839f1bb22b289b12c884913a9018f1943add9b74a638df8f5`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:746c493872f8b672a3d07e35ca12032e8378587480dd245d512aacd2d23a9aa9
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
$ docker pull caddy@sha256:03ffe16fc60ddb7be4684d7c3c8e257038b2c00864c027415e8b05fc120c28d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.9 MB (116937549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d58d2ab3ddba126c2fd014ebdac7030a6d1c5eac1d0c5ea0ac1509d9c8c882d`
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
# Thu, 10 Jun 2021 21:26:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:26:40 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:26:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:26:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:26:42 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:19:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:19:01 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:19:48 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:19:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:19:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:19:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:19:50 GMT
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
	-	`sha256:e25adedf14febf43281fc3b4750e8b0c50f2bb061ef8f5e16a829d3392fa447b`  
		Last Modified: Thu, 10 Jun 2021 21:35:42 GMT  
		Size: 106.1 MB (106136761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52c85161d43b0fdd8bb3ae8fdf77b9e4fc783bceb11f591ed3bbdf1e4722abd`  
		Last Modified: Thu, 10 Jun 2021 21:35:26 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20d66408196d46dd8f1b9f81fb5afa2219f5ca4c68a313ca1c49d3b908f755d`  
		Last Modified: Thu, 10 Jun 2021 23:19:40 GMT  
		Size: 6.4 MB (6395665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84f14058db07dc0560a9f209a7d8768b4ebd80f1426006dec9fe3b4d7c7bd25`  
		Last Modified: Mon, 14 Jun 2021 17:20:29 GMT  
		Size: 1.3 MB (1311168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86b5f727a9d842c09b761d61887e9298328559147dd8e911eb7c5f6fcf5bfc2`  
		Last Modified: Mon, 14 Jun 2021 17:20:29 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:af84e4e4719a6f04129f95de4a1dadacacae55e4b82f98cc9f883020f40860da
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.7 MB (112708776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbae3456b30daef0a0988bb5200978e3a8b2981efecdd2f7a811c692ed7bcc6d`
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
# Thu, 10 Jun 2021 22:01:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 22:01:50 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 22:01:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 22:01:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 22:01:52 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:15:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:15:37 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:49:58 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:49:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:49:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:49:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:50:00 GMT
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
	-	`sha256:f6a122050eb4da5951b1c88f56bfe65cb0c1a50d4e9869ad63787a8d0fc9ff1e`  
		Last Modified: Thu, 10 Jun 2021 22:15:45 GMT  
		Size: 102.4 MB (102351924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc08c6e1815e1794433258a6a0a93785a234db42641d49902c4f194c1d6abc82`  
		Last Modified: Thu, 10 Jun 2021 22:15:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2e5491ca84af37b9bdc0dfcb0a65b798aea4ab080785e1bba16e36672accd4`  
		Last Modified: Thu, 10 Jun 2021 23:16:52 GMT  
		Size: 6.2 MB (6230941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cecdb7ddd0ec1710ae049c902367f06a18606501ca9d1dbe17ec00349029fb8`  
		Last Modified: Mon, 14 Jun 2021 17:51:16 GMT  
		Size: 1.2 MB (1221680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1729fe2ea9a0baa2a26bc61d595958dcecfcb3f577dcebaca53051ec502bf397`  
		Last Modified: Mon, 14 Jun 2021 17:51:16 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2a428d87d883958655e8d72e6461ed205031fac28d71b943746dda7178f2e555
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.6 MB (111602497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da4e596b14ba8264520d8c3f799a567c9b7f3847ae587434759e51d9c667bf76`
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
# Thu, 10 Jun 2021 22:35:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 22:35:30 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 22:35:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 22:35:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 22:35:32 GMT
WORKDIR /go
# Fri, 11 Jun 2021 00:34:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Jun 2021 00:34:12 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:57:59 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:57:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:58:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:58:01 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:58:01 GMT
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
	-	`sha256:3e05d01ffccbffea159372f8065e42d62b484e73624dae1b567d908c12bb6fa3`  
		Last Modified: Thu, 10 Jun 2021 22:53:44 GMT  
		Size: 102.1 MB (102116599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9c0e093faea54528f8e070b0ad60f87674bf3a4654d312ccf7d110de2a6f6a`  
		Last Modified: Thu, 10 Jun 2021 22:53:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59aa8029ac012f4886ea6bced5e66e03743aff8bd41e8c7413cab0369c79c91b`  
		Last Modified: Fri, 11 Jun 2021 00:35:26 GMT  
		Size: 5.6 MB (5560992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a1e9ca701d6638943ef23a3969d9ba902fada02c041a3a797515d585882566`  
		Last Modified: Mon, 14 Jun 2021 17:59:18 GMT  
		Size: 1.2 MB (1219508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017f9bacdf7cdb13305fcaf052511ab74f9d9d2b9cbae1253957277cdb6cdd48`  
		Last Modified: Mon, 14 Jun 2021 17:59:17 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b0e22365417fa304ab483e3f2da3c7b79886ee3bced561c8113dd66b4e664fec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112151491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14b18c1aa44d74288d99db407cad68df0fb403a47cdad522a7524f856bb773f4`
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
# Thu, 10 Jun 2021 21:45:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:45:54 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:45:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:45:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:45:55 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:04:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:04:40 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:39:47 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:39:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:39:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:39:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:39:49 GMT
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
	-	`sha256:a9da95e357649360250671b270e39318d13b2ddff5d5aaac20081d588c9b6f74`  
		Last Modified: Thu, 10 Jun 2021 21:55:04 GMT  
		Size: 101.5 MB (101471730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a246c0d2a229c1d281fc3c1c9aa7fe651a820da43e66cd7ab7660e606d8d9824`  
		Last Modified: Thu, 10 Jun 2021 21:54:43 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2518188a669fe97c7d7feaf8a0ef8974bd167bc206832dc95bae562e6d972fe6`  
		Last Modified: Thu, 10 Jun 2021 23:05:37 GMT  
		Size: 6.5 MB (6483980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cb2ec8e0329ac1e5a6a5f1146f63479477cd73be5c2a0a676a12b3fda9485f`  
		Last Modified: Mon, 14 Jun 2021 17:40:46 GMT  
		Size: 1.2 MB (1201544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3538e34014117eaf3a7b09c03f2fcc11383c7bcebc701bcdfbf5a2a2a61906bb`  
		Last Modified: Mon, 14 Jun 2021 17:40:45 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:f8fc6696fb7cd73549cdc80e5889efd4c9ba480b9622ffe9f316c6e32b6068dc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (111016742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cbbf856cae07e092449ff2a67b42618d6082d532dec5969a4bfa5089b96b11c`
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
# Thu, 10 Jun 2021 21:27:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:27:48 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:27:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:28:04 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:28:11 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:16:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:16:36 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 18:20:23 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:20:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 18:20:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 18:20:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 18:20:58 GMT
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
	-	`sha256:c81f5fe451abbc39d3bdfca4378da5aa2c8b041d846b68db7b6004029734d919`  
		Last Modified: Thu, 10 Jun 2021 21:41:32 GMT  
		Size: 99.9 MB (99918197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9387c57f22b360d0c37409febd5288b34f77782689d3995e0092564a035eae10`  
		Last Modified: Thu, 10 Jun 2021 21:41:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af95f6a2bbd2f3bf752226a7020c5dcb4ba9e36df520e5b7dac8913f4f852d6e`  
		Last Modified: Thu, 10 Jun 2021 23:18:16 GMT  
		Size: 6.8 MB (6830748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994f06d8c6a86a071bc59b2d0644e6c4118c2a51d61edbf571623d36f9b1b987`  
		Last Modified: Mon, 14 Jun 2021 18:21:51 GMT  
		Size: 1.2 MB (1170526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54fa15ba38d0d74a3579bc4af43b527cc19bc368e7351ccaf85c90264bfc31c`  
		Last Modified: Mon, 14 Jun 2021 18:21:50 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:2d70ee7ce742b7eba9d3c4097f0ee5448f02a40e7cc10514c12bbd3272fa7448
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115888076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f08a6df8ec993ccbd835eee259d75804dc13b90f39ad9dccd7971136aecb356`
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
# Thu, 10 Jun 2021 21:52:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:52:35 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:52:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:52:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:52:38 GMT
WORKDIR /go
# Thu, 10 Jun 2021 22:58:58 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 22:58:59 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:41:55 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:41:55 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:41:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:41:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:41:57 GMT
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
	-	`sha256:4b203e6fc30bb6c460e0aea06ed2a200569017655c2678db9ce6fed7a17762cc`  
		Last Modified: Thu, 10 Jun 2021 22:03:02 GMT  
		Size: 105.3 MB (105259453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9fa95d716a4e0cf3f1602cd1def2172371118109ba036c7d525ac506357a1b`  
		Last Modified: Thu, 10 Jun 2021 22:02:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1ceddc3358bec9a3e7284afbcb0a578916db67c3a60fbc269cf78c11f26623`  
		Last Modified: Thu, 10 Jun 2021 22:59:42 GMT  
		Size: 6.5 MB (6479018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab4e3358d5deaa72e1a9a5207c52a6f1133bd89e6c424bb9cf4f0b9fbf2e5b6`  
		Last Modified: Mon, 14 Jun 2021 17:42:29 GMT  
		Size: 1.3 MB (1264529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29212836bbaacf27e155ad8002b1c2a6b5cd2dbe13986b27a57dc427357f2ce`  
		Last Modified: Mon, 14 Jun 2021 17:42:29 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:6732f41f4155f39383864cbc74d3ac805ffda32377941904bfe0ee8d3516f679
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:32914545de594aa79ff4231b61d5594f830641d124fb3cfa56e0575e940ec569
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2808449608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f1d0a4465ebc0bcefa7e5556bfb70eddabb69cf27ef61b558f45bef720fe883`
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
# Mon, 14 Jun 2021 18:21:36 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:21:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 18:22:12 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 14 Jun 2021 18:22:15 GMT
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
	-	`sha256:92f879ad577a7254271b2a27970912d5990740c6c23b65c14d3585b0b331b6b1`  
		Last Modified: Mon, 14 Jun 2021 18:26:07 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14bceb7d820e8f377e4a2d219ae96ee84dafd1055c85c1ce3deb22ea38cb8bf`  
		Last Modified: Mon, 14 Jun 2021 18:26:07 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ddb113a61bc728c0f730228bd4b782a04bcd9bec04ca60a8f46ca5b82e827a8`  
		Last Modified: Mon, 14 Jun 2021 18:26:08 GMT  
		Size: 1.7 MB (1730897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f05c3ba05a4dc7082b32ebd8dae3976fd8adb32927054b6fc0e3f137970df1`  
		Last Modified: Mon, 14 Jun 2021 18:26:07 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:80f678464d89f88f808d926ddf79d5173f7367cc7c1e2381ecc3a7fb7307bb2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `caddy:2-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:3dc1e8d5170dfd5b5e6fbb34d885db2414827f33c49ca301aaaa82644bb7a6fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6437016101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:913b54138653e16a37ea51c2051dd30d0bc4ff76fece599b23b92c1aa7a11ff3`
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
# Mon, 14 Jun 2021 18:22:30 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:22:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 18:24:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 14 Jun 2021 18:24:02 GMT
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
	-	`sha256:3d01a14f10d204dac3535ad62c6b042cc9edc8c2c7c0996ecc45efbb896d5eed`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612bbd13a883cfddbf2977f7de24716a7978eea9f601ba5854f82d36f10068c4`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40a20ce35485bdd147339935426465c403bd3c52351030d040de662cec3253b`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.7 MB (1700121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a492d6062ee0783839f1bb22b289b12c884913a9018f1943add9b74a638df8f5`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:6b1a7e2d64eea0fda092326bf2660a9f57caa3d9e0679b9b2916458ae71a2880
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:84c41546a31938e07bc74b9535459f62221b5fa62f50aadb3f7138ceb0a638b7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2654297157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7933e1b45a92be68914695f31f1c84c86b602c5233536557c1ccee877d1216b0`
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
# Mon, 14 Jun 2021 18:15:56 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:16:40 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8d5cf4479e471d47fd067ce2fbe34c2015a96caedab95ca042aeb633956cbc2bb89c1bc4fe6593c1f96ca58bc66b21f32caa6b099122b9d500a3902245fa5105')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 14 Jun 2021 18:16:43 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 14 Jun 2021 18:16:45 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 14 Jun 2021 18:16:48 GMT
VOLUME [c:/config]
# Mon, 14 Jun 2021 18:16:50 GMT
VOLUME [c:/data]
# Mon, 14 Jun 2021 18:16:53 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:16:55 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:16:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:17:01 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:17:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:17:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:17:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:17:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:17:15 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:17:17 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:17:20 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:17:39 GMT
RUN caddy version
# Mon, 14 Jun 2021 18:17:41 GMT
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
	-	`sha256:07802e3c606e3b9298421527979a2b9797c286d601553a4f8c11271d67919b58`  
		Last Modified: Mon, 14 Jun 2021 18:25:04 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4847967ab228abb45531c45132179ebac7d55ea85bf85ea3f3f420aff0be2863`  
		Last Modified: Mon, 14 Jun 2021 18:25:17 GMT  
		Size: 12.0 MB (12025127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e590a115b7ca0fdadc5a634f9a3b1a58db5ac8a89765f1d00351421045e7dd62`  
		Last Modified: Mon, 14 Jun 2021 18:25:03 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a698c5067c38c742726c5f427f5f07d028e7768a91c4f2fd9a973f662a750b0`  
		Last Modified: Mon, 14 Jun 2021 18:25:03 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4d9bb89edb4e6f90cfacbb81068b117b3b8affe4430a23ddc2f8aa8b1803fa`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369f1dad8944bfe55423327ebaedf96f73e356ca6fd92d4e9a8d2fdbc6b6293c`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f126fec1b223ee19a7f02455cd95a68d8275a8589273ff50b9f7ffbad72a882`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3949035d30e3b80897ac6fc2b4776dccd30680886816cfe8c27ed8bc8c0c595`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c1d9637c1841b64adc5cccf8a5ce5275754886c8c7eb26005eef69727bc101`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa902629ee85278422f20ba99ecc504972ce7c6263bdfa5f1d0a51103ed3e272`  
		Last Modified: Mon, 14 Jun 2021 18:24:59 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7795b0b452df39f057bb8fb233e6862dba05177f3c225da1443588e4e7ec3326`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b936a424e3378bda5aaa142367741f0486702c00117d08a527d36f3876cc7a0`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74ede6be2a18e8c915b5e55628de5a029cf0bb5b69edc917dd8f1c6e1426ee6`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cdf00e847ddd24f1ba768e20fd224aa86a161461a82d3a210f1d5ce1f28cb2`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51405f73ce954be2e339c2cfa1a28109cd371d9fb8986047079a8ba8cc4a9d7a`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38f74dca7b51152c809bf35c007d8affbfc36cae366903110509bdba8f3bde6`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca41d82a7c33c949c331f1ff7958f3ec1551f1bda90faaf07d7b112111a251bc`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582046a83a61d6a9e5701d72c1102b19e9e9ba65665c38d03618e34acdaa5c36`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 300.2 KB (300242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a16f8caea000f3748f024fd14e1419c77091e71e4c220b06a94dc02ffc746c`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:4d5c4f12af6b434f907c262accbfeef1c9eb948d91bb5113bde117904152d9bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278396558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b0d047c64024dd8b9ee7374a59e2e19a219277308f3db92d25f22e903b4f6fb`
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
# Mon, 14 Jun 2021 18:17:52 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:19:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8d5cf4479e471d47fd067ce2fbe34c2015a96caedab95ca042aeb633956cbc2bb89c1bc4fe6593c1f96ca58bc66b21f32caa6b099122b9d500a3902245fa5105')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 14 Jun 2021 18:19:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 14 Jun 2021 18:19:41 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 14 Jun 2021 18:19:43 GMT
VOLUME [c:/config]
# Mon, 14 Jun 2021 18:19:46 GMT
VOLUME [c:/data]
# Mon, 14 Jun 2021 18:19:48 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:19:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:19:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:19:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:19:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:20:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:20:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:20:04 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:20:07 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:20:09 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:20:11 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:21:14 GMT
RUN caddy version
# Mon, 14 Jun 2021 18:21:17 GMT
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
	-	`sha256:5bd5fde0219b866984e02c69748a7c533734e7d3ce1c605e00b2794ba719ca78`  
		Last Modified: Mon, 14 Jun 2021 18:25:40 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ff67696fba822eac7dc90ce8b74a3463e180c1277ce1b5235dd553efd54d37`  
		Last Modified: Mon, 14 Jun 2021 18:25:53 GMT  
		Size: 12.0 MB (12011979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb05b150667473f58bd9ff97143e7addb941c15c23d7c0190462052e171a5d3`  
		Last Modified: Mon, 14 Jun 2021 18:25:40 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417ec686bccf8c11c7e167450f76c56e965e0d895b8a67d2959fa0cd8e0f46c6`  
		Last Modified: Mon, 14 Jun 2021 18:25:39 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e7f7e817f7b000e684b2477e658283e3bc5e32f705e2a1af3eb2171451ab1a`  
		Last Modified: Mon, 14 Jun 2021 18:25:38 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9adbfef5bd1c4ce567e8643e7eb3ac228fc89e60afffa0d4ad65188836ee10e`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46951e23f2c6f042a74af530655917c470e7e58bd428811bea889f06ece060f3`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b702d713b07cb19c098b0a4c2ad22de8111ab140c99b88deb21ffa5f10870f`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1554c780202a1e2bfb6cafbf73148847f97c535c407f63f750903997105d516f`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a72ab2ef98ce84364537328634d5a56cb6c9080cdec9988778c0e15d451dc51`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0cb0fb150ef4d4bb3e78339539c6453dcdf1d1b11d50728bb72e262b603fa9`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d8666b345f227a53b8d4cc8698ebe05b454caf116f8329e30d4328ba56896e`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bce3d7ad9504e8b1a2a5f46b50605a7e895686efeae62529b2fb0c8210a2e7`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d806bd36723a790387c5f61446d9b73da291b1e1592e6943b28686f3dc50fb39`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddf127d6e3c5443190a309b2f703cfd1d079beea71723b1507958dbbf2b5cab`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace91f2d94fe0fd5d53fce078d832db72cc38e2ef7692a44f57f9377dcbf3f8f`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f8adfaab4745797ca3869f6e54a87e5c399e56609635f7b74b039fb8f9fc00`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca3d4ed717fc9e7154ad94da8a5ea30b61ba4dfe9ec25bdcfcb55e6291cbec7`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 274.6 KB (274630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deafc6c05519d23d4709cd8504c83ff6c43943477ddcaf57ae7a871acdbdf489`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:1791c7844819a24a2bae3a297d7e61abe6b39e642e60743a94def9537939148a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:84c41546a31938e07bc74b9535459f62221b5fa62f50aadb3f7138ceb0a638b7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2654297157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7933e1b45a92be68914695f31f1c84c86b602c5233536557c1ccee877d1216b0`
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
# Mon, 14 Jun 2021 18:15:56 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:16:40 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8d5cf4479e471d47fd067ce2fbe34c2015a96caedab95ca042aeb633956cbc2bb89c1bc4fe6593c1f96ca58bc66b21f32caa6b099122b9d500a3902245fa5105')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 14 Jun 2021 18:16:43 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 14 Jun 2021 18:16:45 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 14 Jun 2021 18:16:48 GMT
VOLUME [c:/config]
# Mon, 14 Jun 2021 18:16:50 GMT
VOLUME [c:/data]
# Mon, 14 Jun 2021 18:16:53 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:16:55 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:16:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:17:01 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:17:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:17:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:17:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:17:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:17:15 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:17:17 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:17:20 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:17:39 GMT
RUN caddy version
# Mon, 14 Jun 2021 18:17:41 GMT
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
	-	`sha256:07802e3c606e3b9298421527979a2b9797c286d601553a4f8c11271d67919b58`  
		Last Modified: Mon, 14 Jun 2021 18:25:04 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4847967ab228abb45531c45132179ebac7d55ea85bf85ea3f3f420aff0be2863`  
		Last Modified: Mon, 14 Jun 2021 18:25:17 GMT  
		Size: 12.0 MB (12025127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e590a115b7ca0fdadc5a634f9a3b1a58db5ac8a89765f1d00351421045e7dd62`  
		Last Modified: Mon, 14 Jun 2021 18:25:03 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a698c5067c38c742726c5f427f5f07d028e7768a91c4f2fd9a973f662a750b0`  
		Last Modified: Mon, 14 Jun 2021 18:25:03 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4d9bb89edb4e6f90cfacbb81068b117b3b8affe4430a23ddc2f8aa8b1803fa`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369f1dad8944bfe55423327ebaedf96f73e356ca6fd92d4e9a8d2fdbc6b6293c`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f126fec1b223ee19a7f02455cd95a68d8275a8589273ff50b9f7ffbad72a882`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3949035d30e3b80897ac6fc2b4776dccd30680886816cfe8c27ed8bc8c0c595`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c1d9637c1841b64adc5cccf8a5ce5275754886c8c7eb26005eef69727bc101`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa902629ee85278422f20ba99ecc504972ce7c6263bdfa5f1d0a51103ed3e272`  
		Last Modified: Mon, 14 Jun 2021 18:24:59 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7795b0b452df39f057bb8fb233e6862dba05177f3c225da1443588e4e7ec3326`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b936a424e3378bda5aaa142367741f0486702c00117d08a527d36f3876cc7a0`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74ede6be2a18e8c915b5e55628de5a029cf0bb5b69edc917dd8f1c6e1426ee6`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cdf00e847ddd24f1ba768e20fd224aa86a161461a82d3a210f1d5ce1f28cb2`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51405f73ce954be2e339c2cfa1a28109cd371d9fb8986047079a8ba8cc4a9d7a`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38f74dca7b51152c809bf35c007d8affbfc36cae366903110509bdba8f3bde6`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca41d82a7c33c949c331f1ff7958f3ec1551f1bda90faaf07d7b112111a251bc`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582046a83a61d6a9e5701d72c1102b19e9e9ba65665c38d03618e34acdaa5c36`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 300.2 KB (300242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a16f8caea000f3748f024fd14e1419c77091e71e4c220b06a94dc02ffc746c`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:076e0573f1533c025ab55f299e32833e09ed22b4c52605a2351aba5baa2f585d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:4d5c4f12af6b434f907c262accbfeef1c9eb948d91bb5113bde117904152d9bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278396558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b0d047c64024dd8b9ee7374a59e2e19a219277308f3db92d25f22e903b4f6fb`
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
# Mon, 14 Jun 2021 18:17:52 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:19:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8d5cf4479e471d47fd067ce2fbe34c2015a96caedab95ca042aeb633956cbc2bb89c1bc4fe6593c1f96ca58bc66b21f32caa6b099122b9d500a3902245fa5105')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 14 Jun 2021 18:19:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 14 Jun 2021 18:19:41 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 14 Jun 2021 18:19:43 GMT
VOLUME [c:/config]
# Mon, 14 Jun 2021 18:19:46 GMT
VOLUME [c:/data]
# Mon, 14 Jun 2021 18:19:48 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:19:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:19:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:19:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:19:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:20:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:20:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:20:04 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:20:07 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:20:09 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:20:11 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:21:14 GMT
RUN caddy version
# Mon, 14 Jun 2021 18:21:17 GMT
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
	-	`sha256:5bd5fde0219b866984e02c69748a7c533734e7d3ce1c605e00b2794ba719ca78`  
		Last Modified: Mon, 14 Jun 2021 18:25:40 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ff67696fba822eac7dc90ce8b74a3463e180c1277ce1b5235dd553efd54d37`  
		Last Modified: Mon, 14 Jun 2021 18:25:53 GMT  
		Size: 12.0 MB (12011979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb05b150667473f58bd9ff97143e7addb941c15c23d7c0190462052e171a5d3`  
		Last Modified: Mon, 14 Jun 2021 18:25:40 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417ec686bccf8c11c7e167450f76c56e965e0d895b8a67d2959fa0cd8e0f46c6`  
		Last Modified: Mon, 14 Jun 2021 18:25:39 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e7f7e817f7b000e684b2477e658283e3bc5e32f705e2a1af3eb2171451ab1a`  
		Last Modified: Mon, 14 Jun 2021 18:25:38 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9adbfef5bd1c4ce567e8643e7eb3ac228fc89e60afffa0d4ad65188836ee10e`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46951e23f2c6f042a74af530655917c470e7e58bd428811bea889f06ece060f3`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b702d713b07cb19c098b0a4c2ad22de8111ab140c99b88deb21ffa5f10870f`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1554c780202a1e2bfb6cafbf73148847f97c535c407f63f750903997105d516f`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a72ab2ef98ce84364537328634d5a56cb6c9080cdec9988778c0e15d451dc51`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0cb0fb150ef4d4bb3e78339539c6453dcdf1d1b11d50728bb72e262b603fa9`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d8666b345f227a53b8d4cc8698ebe05b454caf116f8329e30d4328ba56896e`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bce3d7ad9504e8b1a2a5f46b50605a7e895686efeae62529b2fb0c8210a2e7`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d806bd36723a790387c5f61446d9b73da291b1e1592e6943b28686f3dc50fb39`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddf127d6e3c5443190a309b2f703cfd1d079beea71723b1507958dbbf2b5cab`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace91f2d94fe0fd5d53fce078d832db72cc38e2ef7692a44f57f9377dcbf3f8f`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f8adfaab4745797ca3869f6e54a87e5c399e56609635f7b74b039fb8f9fc00`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca3d4ed717fc9e7154ad94da8a5ea30b61ba4dfe9ec25bdcfcb55e6291cbec7`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 274.6 KB (274630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deafc6c05519d23d4709cd8504c83ff6c43943477ddcaf57ae7a871acdbdf489`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0`

```console
$ docker pull caddy@sha256:882a396e2459e610d2115e7c9990e23c73bcfe620dd0e338efb1af710ac0a2c8
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
$ docker pull caddy@sha256:ad7fcb5e4f8d580907534fec48254bcb2b52e3c664ef7d04bd9b07675bc703f2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13616002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f2fa07b13962aea8a31de154b8943ab89fb70831d9b6344421fd135267512d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:09 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Tue, 15 Jun 2021 21:45:09 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:31:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 15 Jun 2021 22:32:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Tue, 15 Jun 2021 22:32:01 GMT
ENV CADDY_VERSION=v2.3.0
# Tue, 15 Jun 2021 22:32:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 15 Jun 2021 22:32:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:32:04 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 15 Jun 2021 22:32:04 GMT
ENV XDG_DATA_HOME=/data
# Tue, 15 Jun 2021 22:32:05 GMT
VOLUME [/config]
# Tue, 15 Jun 2021 22:32:05 GMT
VOLUME [/data]
# Tue, 15 Jun 2021 22:32:05 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Tue, 15 Jun 2021 22:32:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 15 Jun 2021 22:32:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 15 Jun 2021 22:32:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 15 Jun 2021 22:32:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 15 Jun 2021 22:32:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 15 Jun 2021 22:32:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 15 Jun 2021 22:32:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 15 Jun 2021 22:32:07 GMT
EXPOSE 80
# Tue, 15 Jun 2021 22:32:07 GMT
EXPOSE 443
# Tue, 15 Jun 2021 22:32:07 GMT
EXPOSE 2019
# Tue, 15 Jun 2021 22:32:07 GMT
WORKDIR /srv
# Tue, 15 Jun 2021 22:32:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7676a035324952b8345177f1dab18d42cb1a255f5c7c185aaefa04b9d03a791d`  
		Last Modified: Tue, 15 Jun 2021 22:33:12 GMT  
		Size: 300.3 KB (300337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b04585800cb03a18b0fc6fb828594086bdf31f22a8130c561d531f0a0d8b32`  
		Last Modified: Tue, 15 Jun 2021 22:33:12 GMT  
		Size: 5.8 KB (5836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9794e31ac10a1f9a6febe02282ab1d8546e8626d1b147c6c91462d39672a63a`  
		Last Modified: Tue, 15 Jun 2021 22:33:14 GMT  
		Size: 10.6 MB (10598982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284e8a930ea4edb8c0951795abfea6c3b45b0a47df12f40a825f12cb281001a8`  
		Last Modified: Tue, 15 Jun 2021 22:33:12 GMT  
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
$ docker pull caddy@sha256:3c990f355e9151ee07ed68cbe0177caad70239dfd1ff536e3f25e151a967abbc
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
$ docker pull caddy@sha256:ad7fcb5e4f8d580907534fec48254bcb2b52e3c664ef7d04bd9b07675bc703f2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13616002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f2fa07b13962aea8a31de154b8943ab89fb70831d9b6344421fd135267512d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:09 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Tue, 15 Jun 2021 21:45:09 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:31:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 15 Jun 2021 22:32:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Tue, 15 Jun 2021 22:32:01 GMT
ENV CADDY_VERSION=v2.3.0
# Tue, 15 Jun 2021 22:32:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 15 Jun 2021 22:32:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:32:04 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 15 Jun 2021 22:32:04 GMT
ENV XDG_DATA_HOME=/data
# Tue, 15 Jun 2021 22:32:05 GMT
VOLUME [/config]
# Tue, 15 Jun 2021 22:32:05 GMT
VOLUME [/data]
# Tue, 15 Jun 2021 22:32:05 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Tue, 15 Jun 2021 22:32:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 15 Jun 2021 22:32:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 15 Jun 2021 22:32:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 15 Jun 2021 22:32:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 15 Jun 2021 22:32:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 15 Jun 2021 22:32:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 15 Jun 2021 22:32:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 15 Jun 2021 22:32:07 GMT
EXPOSE 80
# Tue, 15 Jun 2021 22:32:07 GMT
EXPOSE 443
# Tue, 15 Jun 2021 22:32:07 GMT
EXPOSE 2019
# Tue, 15 Jun 2021 22:32:07 GMT
WORKDIR /srv
# Tue, 15 Jun 2021 22:32:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7676a035324952b8345177f1dab18d42cb1a255f5c7c185aaefa04b9d03a791d`  
		Last Modified: Tue, 15 Jun 2021 22:33:12 GMT  
		Size: 300.3 KB (300337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b04585800cb03a18b0fc6fb828594086bdf31f22a8130c561d531f0a0d8b32`  
		Last Modified: Tue, 15 Jun 2021 22:33:12 GMT  
		Size: 5.8 KB (5836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9794e31ac10a1f9a6febe02282ab1d8546e8626d1b147c6c91462d39672a63a`  
		Last Modified: Tue, 15 Jun 2021 22:33:14 GMT  
		Size: 10.6 MB (10598982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284e8a930ea4edb8c0951795abfea6c3b45b0a47df12f40a825f12cb281001a8`  
		Last Modified: Tue, 15 Jun 2021 22:33:12 GMT  
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
$ docker pull caddy@sha256:c85f231d43559a2b0056d7348d1a9a00d09befbfef5d91dfcfc650597a184600
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
$ docker pull caddy@sha256:66abdba0beb713ba30e451fc2f6a2685562880913a54afb3e9c15d241c635849
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.6 MB (119571407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a0815f636bedfbe14b5318cf8f3c67a30de0615ba7d5dfbcd55b046290e6176`
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
# Thu, 10 Jun 2021 21:32:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:32:13 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:32:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:32:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:32:14 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:18:49 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:18:49 GMT
ENV XCADDY_VERSION=v0.1.9
# Thu, 10 Jun 2021 23:18:49 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 10 Jun 2021 23:18:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Jun 2021 23:18:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 10 Jun 2021 23:18:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 10 Jun 2021 23:18:52 GMT
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
	-	`sha256:45645685a6b6163aec9fca5cbba282bcdd9f5d05618f0d05cd2ae3cea7d189fe`  
		Last Modified: Thu, 10 Jun 2021 21:37:25 GMT  
		Size: 106.8 MB (106846128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26c0b7800df7ff25dda336ae8a8e011f7af248e7b88c1d3e77c58ac29ae2755`  
		Last Modified: Thu, 10 Jun 2021 21:37:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85f4d0dd62afa81ec30dd72889df6ec6ea242407a40f575e4bb9c79a2e33eff`  
		Last Modified: Thu, 10 Jun 2021 23:19:29 GMT  
		Size: 8.3 MB (8331959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7033ff0a1e20c02c49ff77b151caf3956a95519d65b39ab74889d5dd5531ed2a`  
		Last Modified: Thu, 10 Jun 2021 23:19:28 GMT  
		Size: 1.3 MB (1311160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ab79ec2ca7e7be9aece0a71f900457db015da276ad9f6be4f2a91b941108eb`  
		Last Modified: Thu, 10 Jun 2021 23:19:27 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:54b4749347941a5da83c37d7d6354ae4a44964180c396017caafd4d7511a332b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114759050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9203997bd72876c6f3ceafd942eee8682ea331f754f5b500263783857ecbcd8a`
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
# Thu, 10 Jun 2021 22:11:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 22:11:51 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 22:11:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 22:11:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 22:11:52 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:15:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:15:16 GMT
ENV XCADDY_VERSION=v0.1.9
# Thu, 10 Jun 2021 23:15:16 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 10 Jun 2021 23:15:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Jun 2021 23:15:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 10 Jun 2021 23:15:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 10 Jun 2021 23:15:18 GMT
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
	-	`sha256:486819c75a22e5ed4347ed53c9fe89e3ebfee04af5ee6d8e83087c2b61d1cdbd`  
		Last Modified: Thu, 10 Jun 2021 22:18:20 GMT  
		Size: 102.7 MB (102700905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61718e725ae0c40bce035c770dc76f5124e85cf567fccc4b908dacf8364c342f`  
		Last Modified: Thu, 10 Jun 2021 22:17:55 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3624613faf4a7b50068a7fe079cd46d9d722a3fef714e1e9f1a3addb8d19956b`  
		Last Modified: Thu, 10 Jun 2021 23:16:37 GMT  
		Size: 7.9 MB (7949522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62edd010960fce04b286616f894d24fd961afc96370ee382f4689e663af9067d`  
		Last Modified: Thu, 10 Jun 2021 23:16:36 GMT  
		Size: 1.2 MB (1221674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1199882516f2847f9b077c5665a08a26b9e0e085f609b9577f6e18f40df65cd1`  
		Last Modified: Thu, 10 Jun 2021 23:16:35 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:28ddedf354a31c1aabc002718b4f05dc8ae99b1559b347d90f3132e19ea7c0fd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113559953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14fbae9fa3ec5b4f54093a91db20409fcd3f2da433edba20f706729a34d82386`
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
# Thu, 10 Jun 2021 22:47:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 22:47:02 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 22:47:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 22:47:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 22:47:03 GMT
WORKDIR /go
# Fri, 11 Jun 2021 00:33:51 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Jun 2021 00:33:52 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 11 Jun 2021 00:33:52 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 11 Jun 2021 00:33:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 11 Jun 2021 00:33:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 11 Jun 2021 00:33:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 11 Jun 2021 00:33:54 GMT
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
	-	`sha256:df9036c2884e4a8ef6c0ded81f798ae0dfcd0ef61ce7de996a69fa0018fe402b`  
		Last Modified: Thu, 10 Jun 2021 22:56:26 GMT  
		Size: 102.5 MB (102489502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9bec4ac91c0246b9f558aa13a6f1a90257a611a8a7b202178c6cc3c61bf639`  
		Last Modified: Thu, 10 Jun 2021 22:56:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c88ee845e531926665391366753b0b3e6e51781813589fe768bd9070ffcee0e`  
		Last Modified: Fri, 11 Jun 2021 00:35:13 GMT  
		Size: 7.2 MB (7160975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1e177e62e8df10c90d21017a141dc540e7641148057598c7183f701cfb7e59`  
		Last Modified: Fri, 11 Jun 2021 00:35:13 GMT  
		Size: 1.2 MB (1219504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b61601565a372b7df2b42cbf674d6cf72114ab6b1f1d08f8738888dbf6fd27`  
		Last Modified: Fri, 11 Jun 2021 00:35:12 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e0cbe8682e3163c63778217041a654d16060c1e0aabb42808e5a468b1c5c4621
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.9 MB (114882209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36e54850e322e3ffe7d9defa2642c21d8070a8a7664bc9e4171e285f79b3646e`
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
# Thu, 10 Jun 2021 21:50:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:50:29 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:50:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:50:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:50:30 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:04:25 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:04:25 GMT
ENV XCADDY_VERSION=v0.1.9
# Thu, 10 Jun 2021 23:04:25 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 10 Jun 2021 23:04:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Jun 2021 23:04:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 10 Jun 2021 23:04:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 10 Jun 2021 23:04:27 GMT
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
	-	`sha256:b0d2c8dc2485ffbee5080242e6fb6797aed1cbfbaa26b36c66c10c47913ea0fe`  
		Last Modified: Thu, 10 Jun 2021 21:57:07 GMT  
		Size: 102.2 MB (102162815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f45cfdd585c4a6b36fe9dcc17b2d082b79cdf26ed58b590c31fb9bc342de34`  
		Last Modified: Thu, 10 Jun 2021 21:56:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0a2e38042160dff8ab981a10e039aaea0323c3dc29bd2564fa68a7e4fc2bb5`  
		Last Modified: Thu, 10 Jun 2021 23:05:25 GMT  
		Size: 8.5 MB (8525221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f421d3cdfc4df72d2e07893544d5b70ecd8f4d0b3a995f228e0a290c59b630ad`  
		Last Modified: Thu, 10 Jun 2021 23:05:24 GMT  
		Size: 1.2 MB (1201541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26bbcbe0c2146e989a9cbacd21a09130c0c0a9627c57f50d3ad2fc806bfb2762`  
		Last Modified: Thu, 10 Jun 2021 23:05:24 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:b991e9d1b4c878f545678a358aaeb819aff15f3b8547151fa5d7e256e559042e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (114043843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdf13e7461103f32cc713007a2fe886c02e2b48799a1c78f71de8b12b064e637`
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
# Thu, 10 Jun 2021 21:35:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:35:37 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:35:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:35:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:35:50 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:15:25 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:15:31 GMT
ENV XCADDY_VERSION=v0.1.9
# Thu, 10 Jun 2021 23:15:35 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 10 Jun 2021 23:15:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Jun 2021 23:15:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 10 Jun 2021 23:15:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 10 Jun 2021 23:15:58 GMT
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
	-	`sha256:00a08a27a322b7e79fed3e5996802ec5d9fa558c4ef5bb4289bb6cd36d8eda5d`  
		Last Modified: Thu, 10 Jun 2021 21:43:21 GMT  
		Size: 100.8 MB (100836900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7183a6312e4eb4f3e0b7e261cb7145985ab8732effd3772bfa36eeeae7dd6317`  
		Last Modified: Thu, 10 Jun 2021 21:43:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3659d6f2ae2121b985ce787cbb4d3f2f2ff706f65bcb3e146690af24407280c7`  
		Last Modified: Thu, 10 Jun 2021 23:18:06 GMT  
		Size: 8.9 MB (8945763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f6c509ed2601af85d204fbd5a1ec3ffc7da03bbe6ef91ab385906c8999a73f`  
		Last Modified: Thu, 10 Jun 2021 23:18:05 GMT  
		Size: 1.2 MB (1170515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8e6aa7451182d3385f32a20b8675f2086c594c07d7eea6d37dcb66b9c08dfd`  
		Last Modified: Thu, 10 Jun 2021 23:18:05 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; s390x

```console
$ docker pull caddy@sha256:b11c4b2254a133a58366147988d55011b258d941c8b018b68f306fd3958a1018
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118461549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:738e410094b561f3ebe0fffcdc185f681ca4ce8f0aa202f85a71bf5f2546b292`
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
# Thu, 10 Jun 2021 22:00:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 22:00:23 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 22:00:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 22:00:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 22:00:26 GMT
WORKDIR /go
# Thu, 10 Jun 2021 22:58:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 22:58:39 GMT
ENV XCADDY_VERSION=v0.1.9
# Thu, 10 Jun 2021 22:58:40 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 10 Jun 2021 22:58:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Jun 2021 22:58:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 10 Jun 2021 22:58:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 10 Jun 2021 22:58:44 GMT
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
	-	`sha256:48deb59b0c4b5d9c08219ae3fea9624069f4b9ab39cdd6643bf24374afebddb0`  
		Last Modified: Thu, 10 Jun 2021 22:04:19 GMT  
		Size: 106.0 MB (105972819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9698d73307c65bd3c8b8ed1af4789c47142250bce0215e1b6a21151755aeeb`  
		Last Modified: Thu, 10 Jun 2021 22:04:06 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2989c1a50f7c884c27276b7c21c3b415bd09786a163412c28edddf2a709d96bd`  
		Last Modified: Thu, 10 Jun 2021 22:59:35 GMT  
		Size: 8.4 MB (8373730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ff13d479da10090d7f6b21305d0544b94adb67ed1ef5030de39f0b4dbcbd4a`  
		Last Modified: Thu, 10 Jun 2021 22:59:34 GMT  
		Size: 1.3 MB (1264516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c832aad9674649efd5e457c3212c46ded4d3fe50593380cab4dd39e0a3e97c9a`  
		Last Modified: Thu, 10 Jun 2021 22:59:34 GMT  
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
$ docker pull caddy@sha256:1a9038c6c8ff30d015590b0321b2f58d8a403b1b708db7421af383470e630217
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
$ docker pull caddy@sha256:66abdba0beb713ba30e451fc2f6a2685562880913a54afb3e9c15d241c635849
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.6 MB (119571407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a0815f636bedfbe14b5318cf8f3c67a30de0615ba7d5dfbcd55b046290e6176`
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
# Thu, 10 Jun 2021 21:32:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:32:13 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:32:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:32:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:32:14 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:18:49 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:18:49 GMT
ENV XCADDY_VERSION=v0.1.9
# Thu, 10 Jun 2021 23:18:49 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 10 Jun 2021 23:18:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Jun 2021 23:18:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 10 Jun 2021 23:18:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 10 Jun 2021 23:18:52 GMT
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
	-	`sha256:45645685a6b6163aec9fca5cbba282bcdd9f5d05618f0d05cd2ae3cea7d189fe`  
		Last Modified: Thu, 10 Jun 2021 21:37:25 GMT  
		Size: 106.8 MB (106846128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26c0b7800df7ff25dda336ae8a8e011f7af248e7b88c1d3e77c58ac29ae2755`  
		Last Modified: Thu, 10 Jun 2021 21:37:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85f4d0dd62afa81ec30dd72889df6ec6ea242407a40f575e4bb9c79a2e33eff`  
		Last Modified: Thu, 10 Jun 2021 23:19:29 GMT  
		Size: 8.3 MB (8331959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7033ff0a1e20c02c49ff77b151caf3956a95519d65b39ab74889d5dd5531ed2a`  
		Last Modified: Thu, 10 Jun 2021 23:19:28 GMT  
		Size: 1.3 MB (1311160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ab79ec2ca7e7be9aece0a71f900457db015da276ad9f6be4f2a91b941108eb`  
		Last Modified: Thu, 10 Jun 2021 23:19:27 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:54b4749347941a5da83c37d7d6354ae4a44964180c396017caafd4d7511a332b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114759050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9203997bd72876c6f3ceafd942eee8682ea331f754f5b500263783857ecbcd8a`
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
# Thu, 10 Jun 2021 22:11:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 22:11:51 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 22:11:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 22:11:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 22:11:52 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:15:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:15:16 GMT
ENV XCADDY_VERSION=v0.1.9
# Thu, 10 Jun 2021 23:15:16 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 10 Jun 2021 23:15:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Jun 2021 23:15:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 10 Jun 2021 23:15:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 10 Jun 2021 23:15:18 GMT
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
	-	`sha256:486819c75a22e5ed4347ed53c9fe89e3ebfee04af5ee6d8e83087c2b61d1cdbd`  
		Last Modified: Thu, 10 Jun 2021 22:18:20 GMT  
		Size: 102.7 MB (102700905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61718e725ae0c40bce035c770dc76f5124e85cf567fccc4b908dacf8364c342f`  
		Last Modified: Thu, 10 Jun 2021 22:17:55 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3624613faf4a7b50068a7fe079cd46d9d722a3fef714e1e9f1a3addb8d19956b`  
		Last Modified: Thu, 10 Jun 2021 23:16:37 GMT  
		Size: 7.9 MB (7949522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62edd010960fce04b286616f894d24fd961afc96370ee382f4689e663af9067d`  
		Last Modified: Thu, 10 Jun 2021 23:16:36 GMT  
		Size: 1.2 MB (1221674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1199882516f2847f9b077c5665a08a26b9e0e085f609b9577f6e18f40df65cd1`  
		Last Modified: Thu, 10 Jun 2021 23:16:35 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:28ddedf354a31c1aabc002718b4f05dc8ae99b1559b347d90f3132e19ea7c0fd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113559953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14fbae9fa3ec5b4f54093a91db20409fcd3f2da433edba20f706729a34d82386`
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
# Thu, 10 Jun 2021 22:47:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 22:47:02 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 22:47:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 22:47:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 22:47:03 GMT
WORKDIR /go
# Fri, 11 Jun 2021 00:33:51 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Jun 2021 00:33:52 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 11 Jun 2021 00:33:52 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 11 Jun 2021 00:33:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 11 Jun 2021 00:33:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 11 Jun 2021 00:33:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 11 Jun 2021 00:33:54 GMT
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
	-	`sha256:df9036c2884e4a8ef6c0ded81f798ae0dfcd0ef61ce7de996a69fa0018fe402b`  
		Last Modified: Thu, 10 Jun 2021 22:56:26 GMT  
		Size: 102.5 MB (102489502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9bec4ac91c0246b9f558aa13a6f1a90257a611a8a7b202178c6cc3c61bf639`  
		Last Modified: Thu, 10 Jun 2021 22:56:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c88ee845e531926665391366753b0b3e6e51781813589fe768bd9070ffcee0e`  
		Last Modified: Fri, 11 Jun 2021 00:35:13 GMT  
		Size: 7.2 MB (7160975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1e177e62e8df10c90d21017a141dc540e7641148057598c7183f701cfb7e59`  
		Last Modified: Fri, 11 Jun 2021 00:35:13 GMT  
		Size: 1.2 MB (1219504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b61601565a372b7df2b42cbf674d6cf72114ab6b1f1d08f8738888dbf6fd27`  
		Last Modified: Fri, 11 Jun 2021 00:35:12 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e0cbe8682e3163c63778217041a654d16060c1e0aabb42808e5a468b1c5c4621
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.9 MB (114882209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36e54850e322e3ffe7d9defa2642c21d8070a8a7664bc9e4171e285f79b3646e`
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
# Thu, 10 Jun 2021 21:50:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:50:29 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:50:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:50:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:50:30 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:04:25 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:04:25 GMT
ENV XCADDY_VERSION=v0.1.9
# Thu, 10 Jun 2021 23:04:25 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 10 Jun 2021 23:04:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Jun 2021 23:04:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 10 Jun 2021 23:04:27 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 10 Jun 2021 23:04:27 GMT
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
	-	`sha256:b0d2c8dc2485ffbee5080242e6fb6797aed1cbfbaa26b36c66c10c47913ea0fe`  
		Last Modified: Thu, 10 Jun 2021 21:57:07 GMT  
		Size: 102.2 MB (102162815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f45cfdd585c4a6b36fe9dcc17b2d082b79cdf26ed58b590c31fb9bc342de34`  
		Last Modified: Thu, 10 Jun 2021 21:56:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0a2e38042160dff8ab981a10e039aaea0323c3dc29bd2564fa68a7e4fc2bb5`  
		Last Modified: Thu, 10 Jun 2021 23:05:25 GMT  
		Size: 8.5 MB (8525221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f421d3cdfc4df72d2e07893544d5b70ecd8f4d0b3a995f228e0a290c59b630ad`  
		Last Modified: Thu, 10 Jun 2021 23:05:24 GMT  
		Size: 1.2 MB (1201541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26bbcbe0c2146e989a9cbacd21a09130c0c0a9627c57f50d3ad2fc806bfb2762`  
		Last Modified: Thu, 10 Jun 2021 23:05:24 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:b991e9d1b4c878f545678a358aaeb819aff15f3b8547151fa5d7e256e559042e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (114043843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdf13e7461103f32cc713007a2fe886c02e2b48799a1c78f71de8b12b064e637`
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
# Thu, 10 Jun 2021 21:35:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:35:37 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:35:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:35:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:35:50 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:15:25 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:15:31 GMT
ENV XCADDY_VERSION=v0.1.9
# Thu, 10 Jun 2021 23:15:35 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 10 Jun 2021 23:15:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Jun 2021 23:15:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 10 Jun 2021 23:15:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 10 Jun 2021 23:15:58 GMT
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
	-	`sha256:00a08a27a322b7e79fed3e5996802ec5d9fa558c4ef5bb4289bb6cd36d8eda5d`  
		Last Modified: Thu, 10 Jun 2021 21:43:21 GMT  
		Size: 100.8 MB (100836900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7183a6312e4eb4f3e0b7e261cb7145985ab8732effd3772bfa36eeeae7dd6317`  
		Last Modified: Thu, 10 Jun 2021 21:43:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3659d6f2ae2121b985ce787cbb4d3f2f2ff706f65bcb3e146690af24407280c7`  
		Last Modified: Thu, 10 Jun 2021 23:18:06 GMT  
		Size: 8.9 MB (8945763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f6c509ed2601af85d204fbd5a1ec3ffc7da03bbe6ef91ab385906c8999a73f`  
		Last Modified: Thu, 10 Jun 2021 23:18:05 GMT  
		Size: 1.2 MB (1170515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8e6aa7451182d3385f32a20b8675f2086c594c07d7eea6d37dcb66b9c08dfd`  
		Last Modified: Thu, 10 Jun 2021 23:18:05 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:b11c4b2254a133a58366147988d55011b258d941c8b018b68f306fd3958a1018
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118461549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:738e410094b561f3ebe0fffcdc185f681ca4ce8f0aa202f85a71bf5f2546b292`
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
# Thu, 10 Jun 2021 22:00:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.13.src.tar.gz'; 	sha256='99069e7223479cce4553f84f874b9345f6f4045f27cf5089489b546da619a244'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 22:00:23 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 22:00:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 22:00:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 22:00:26 GMT
WORKDIR /go
# Thu, 10 Jun 2021 22:58:38 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 22:58:39 GMT
ENV XCADDY_VERSION=v0.1.9
# Thu, 10 Jun 2021 22:58:40 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 10 Jun 2021 22:58:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Jun 2021 22:58:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 10 Jun 2021 22:58:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 10 Jun 2021 22:58:44 GMT
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
	-	`sha256:48deb59b0c4b5d9c08219ae3fea9624069f4b9ab39cdd6643bf24374afebddb0`  
		Last Modified: Thu, 10 Jun 2021 22:04:19 GMT  
		Size: 106.0 MB (105972819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9698d73307c65bd3c8b8ed1af4789c47142250bce0215e1b6a21151755aeeb`  
		Last Modified: Thu, 10 Jun 2021 22:04:06 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2989c1a50f7c884c27276b7c21c3b415bd09786a163412c28edddf2a709d96bd`  
		Last Modified: Thu, 10 Jun 2021 22:59:35 GMT  
		Size: 8.4 MB (8373730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ff13d479da10090d7f6b21305d0544b94adb67ed1ef5030de39f0b4dbcbd4a`  
		Last Modified: Thu, 10 Jun 2021 22:59:34 GMT  
		Size: 1.3 MB (1264516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c832aad9674649efd5e457c3212c46ded4d3fe50593380cab4dd39e0a3e97c9a`  
		Last Modified: Thu, 10 Jun 2021 22:59:34 GMT  
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

## `caddy:2.4.2`

```console
$ docker pull caddy@sha256:31493fd55da69e11db44f6acbd0c92070187cfd61dd0a5bfe17a0f6aa7b894d2
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

### `caddy:2.4.2` - linux; amd64

```console
$ docker pull caddy@sha256:c3176ebaceec5d64a4892205d7cf3d32da87e2fcbbb8a47d787ef4200ef0e6d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14649179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57e953391a547aacb19ba079ee6713b24b8400352d6d95a8a43e79fb035ec0f7`
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
# Mon, 14 Jun 2021 17:19:37 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:19:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:19:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:19:41 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:19:41 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:19:41 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:19:41 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:19:41 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:19:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:19:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:19:43 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:19:43 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:19:43 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:19:44 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:19:44 GMT
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
	-	`sha256:037bdadcf837298422d86bb75d10aa9ea21eaaf0969e1d8e99b730b07208eb03`  
		Last Modified: Mon, 14 Jun 2021 17:20:16 GMT  
		Size: 11.5 MB (11530800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9785de7e5400398efa43aedd6416426c14e3101f52a5930b52b6e8ea3a0cd96`  
		Last Modified: Mon, 14 Jun 2021 17:20:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:53bc8c15c11306be1cd426dffb91df56e5dc186ae54c22eb08996f14c647378f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13817125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dd81d0e3a6035d5df068c9af8811281698921854e5190944b1f7a079651bb7d`
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
# Mon, 14 Jun 2021 17:49:40 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:49:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:49:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:49:44 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:49:44 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:49:44 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:49:44 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:49:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:49:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:49:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:49:46 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:49:46 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:49:47 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:49:47 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:49:47 GMT
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
	-	`sha256:028e0db410d042e12d6b3f64499cc00ae7298c02382ba1105cdc5ee03aaed549`  
		Last Modified: Mon, 14 Jun 2021 17:50:59 GMT  
		Size: 10.9 MB (10888459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64dbe91d32616efff4ec27f049638b231cfd0091a68480d45a21791d44b469c`  
		Last Modified: Mon, 14 Jun 2021 17:50:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:6fc967765fceab93d7838f17d2eeceddc56e21a65654e3ba92c799437ff09280
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13593827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d1b6dc4a59a634275f3c206036245997415a7d1894697b43d1dadc232712e8e`
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
# Mon, 14 Jun 2021 17:57:41 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:57:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:57:44 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:57:45 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:57:45 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:57:45 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:57:45 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:57:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:57:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:57:47 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:57:47 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:57:48 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:57:48 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:57:48 GMT
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
	-	`sha256:e97e805578bb88faf1e3b052fe899c9818d27e0e114574198d5e3d45a8faf1b9`  
		Last Modified: Mon, 14 Jun 2021 17:59:01 GMT  
		Size: 10.9 MB (10864008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee92873b0980eae80c33cd1bd74d1b35754b48c89cbe68088f4e98b4dd04e2f`  
		Last Modified: Mon, 14 Jun 2021 17:58:59 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:1f49cc95c1e8ebd7fe139595b64b8d3b2cbdafff4c46ff46bc4516054a50e3ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13466108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:749cdbfee8dde296c03efb611b07c067ca297771a1314bbcbbba992429e899e7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:32:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 15 Jun 2021 22:32:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 15 Jun 2021 22:32:20 GMT
ENV CADDY_VERSION=v2.4.2
# Tue, 15 Jun 2021 22:32:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 15 Jun 2021 22:32:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:32:23 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 15 Jun 2021 22:32:24 GMT
ENV XDG_DATA_HOME=/data
# Tue, 15 Jun 2021 22:32:24 GMT
VOLUME [/config]
# Tue, 15 Jun 2021 22:32:24 GMT
VOLUME [/data]
# Tue, 15 Jun 2021 22:32:24 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Tue, 15 Jun 2021 22:32:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 15 Jun 2021 22:32:26 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 15 Jun 2021 22:32:26 GMT
EXPOSE 80
# Tue, 15 Jun 2021 22:32:26 GMT
EXPOSE 443
# Tue, 15 Jun 2021 22:32:26 GMT
EXPOSE 2019
# Tue, 15 Jun 2021 22:32:26 GMT
WORKDIR /srv
# Tue, 15 Jun 2021 22:32:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d0b72044755ebd2b829600b94a69aa9096bbb4bf9a01c1795b5b245261b99a`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 300.6 KB (300631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abde659ccf1d73128ef1e71a9701b014e0f27d4abf15b3d410d0474cdd0adb95`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0b93549f9104a9bb517f1ae15bd6ef4d44f83d21964728c50aa960b97098dc`  
		Last Modified: Tue, 15 Jun 2021 22:33:26 GMT  
		Size: 10.4 MB (10447450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69a851000e14247059ab07104ab76f86231aaa1a4fb5abb6b321e66a45003d3`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2` - linux; ppc64le

```console
$ docker pull caddy@sha256:7764cdcd665f8e23165bf385240e8951ab046dd6f54808b247b57e284882ecc5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13175121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c3b2d52d66b7076e6c98e715324384114a94b978294b836f566919d77faa909`
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
# Mon, 14 Jun 2021 18:16:57 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:17:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 18:17:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 18:17:56 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 18:18:00 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 18:18:08 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 18:18:15 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 18:18:26 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:18:36 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:18:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:18:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:18:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:19:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:19:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:19:27 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:19:32 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:19:38 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:19:43 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:19:49 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 18:19:56 GMT
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
	-	`sha256:d23e936288e88eac2d5280068486ab71f9023047b51d2c012a09fd305cc70e19`  
		Last Modified: Mon, 14 Jun 2021 18:21:33 GMT  
		Size: 10.1 MB (10053418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59596542df0c41e54f99fa862419a9f75ef8cfce5b1788110d747951a295518e`  
		Last Modified: Mon, 14 Jun 2021 18:21:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2` - linux; s390x

```console
$ docker pull caddy@sha256:c8d5cda3a4ef8a3fae917a732cd349372b1cc625071f9b3acc77a9033eb55e63
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14004446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5539a479891dabbacf899df4a9c0af209caf5e8b82799b452efd5c9093bd99`
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
# Mon, 14 Jun 2021 17:41:42 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:41:46 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:41:46 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:41:46 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:41:47 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:41:49 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:41:49 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:41:49 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:41:49 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:41:50 GMT
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
	-	`sha256:9b59880ffc79bf424b9fb38c497ec3d3edea77c4cbabb6b295bad830e4732008`  
		Last Modified: Mon, 14 Jun 2021 17:42:22 GMT  
		Size: 11.1 MB (11094948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4a0a3f3a72f3127538116c7943809378ae5921f09f19249fb98a578d261a49`  
		Last Modified: Mon, 14 Jun 2021 17:42:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:84c41546a31938e07bc74b9535459f62221b5fa62f50aadb3f7138ceb0a638b7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2654297157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7933e1b45a92be68914695f31f1c84c86b602c5233536557c1ccee877d1216b0`
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
# Mon, 14 Jun 2021 18:15:56 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:16:40 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8d5cf4479e471d47fd067ce2fbe34c2015a96caedab95ca042aeb633956cbc2bb89c1bc4fe6593c1f96ca58bc66b21f32caa6b099122b9d500a3902245fa5105')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 14 Jun 2021 18:16:43 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 14 Jun 2021 18:16:45 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 14 Jun 2021 18:16:48 GMT
VOLUME [c:/config]
# Mon, 14 Jun 2021 18:16:50 GMT
VOLUME [c:/data]
# Mon, 14 Jun 2021 18:16:53 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:16:55 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:16:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:17:01 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:17:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:17:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:17:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:17:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:17:15 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:17:17 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:17:20 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:17:39 GMT
RUN caddy version
# Mon, 14 Jun 2021 18:17:41 GMT
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
	-	`sha256:07802e3c606e3b9298421527979a2b9797c286d601553a4f8c11271d67919b58`  
		Last Modified: Mon, 14 Jun 2021 18:25:04 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4847967ab228abb45531c45132179ebac7d55ea85bf85ea3f3f420aff0be2863`  
		Last Modified: Mon, 14 Jun 2021 18:25:17 GMT  
		Size: 12.0 MB (12025127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e590a115b7ca0fdadc5a634f9a3b1a58db5ac8a89765f1d00351421045e7dd62`  
		Last Modified: Mon, 14 Jun 2021 18:25:03 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a698c5067c38c742726c5f427f5f07d028e7768a91c4f2fd9a973f662a750b0`  
		Last Modified: Mon, 14 Jun 2021 18:25:03 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4d9bb89edb4e6f90cfacbb81068b117b3b8affe4430a23ddc2f8aa8b1803fa`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369f1dad8944bfe55423327ebaedf96f73e356ca6fd92d4e9a8d2fdbc6b6293c`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f126fec1b223ee19a7f02455cd95a68d8275a8589273ff50b9f7ffbad72a882`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3949035d30e3b80897ac6fc2b4776dccd30680886816cfe8c27ed8bc8c0c595`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c1d9637c1841b64adc5cccf8a5ce5275754886c8c7eb26005eef69727bc101`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa902629ee85278422f20ba99ecc504972ce7c6263bdfa5f1d0a51103ed3e272`  
		Last Modified: Mon, 14 Jun 2021 18:24:59 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7795b0b452df39f057bb8fb233e6862dba05177f3c225da1443588e4e7ec3326`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b936a424e3378bda5aaa142367741f0486702c00117d08a527d36f3876cc7a0`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74ede6be2a18e8c915b5e55628de5a029cf0bb5b69edc917dd8f1c6e1426ee6`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cdf00e847ddd24f1ba768e20fd224aa86a161461a82d3a210f1d5ce1f28cb2`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51405f73ce954be2e339c2cfa1a28109cd371d9fb8986047079a8ba8cc4a9d7a`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38f74dca7b51152c809bf35c007d8affbfc36cae366903110509bdba8f3bde6`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca41d82a7c33c949c331f1ff7958f3ec1551f1bda90faaf07d7b112111a251bc`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582046a83a61d6a9e5701d72c1102b19e9e9ba65665c38d03618e34acdaa5c36`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 300.2 KB (300242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a16f8caea000f3748f024fd14e1419c77091e71e4c220b06a94dc02ffc746c`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:4d5c4f12af6b434f907c262accbfeef1c9eb948d91bb5113bde117904152d9bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278396558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b0d047c64024dd8b9ee7374a59e2e19a219277308f3db92d25f22e903b4f6fb`
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
# Mon, 14 Jun 2021 18:17:52 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:19:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8d5cf4479e471d47fd067ce2fbe34c2015a96caedab95ca042aeb633956cbc2bb89c1bc4fe6593c1f96ca58bc66b21f32caa6b099122b9d500a3902245fa5105')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 14 Jun 2021 18:19:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 14 Jun 2021 18:19:41 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 14 Jun 2021 18:19:43 GMT
VOLUME [c:/config]
# Mon, 14 Jun 2021 18:19:46 GMT
VOLUME [c:/data]
# Mon, 14 Jun 2021 18:19:48 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:19:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:19:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:19:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:19:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:20:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:20:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:20:04 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:20:07 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:20:09 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:20:11 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:21:14 GMT
RUN caddy version
# Mon, 14 Jun 2021 18:21:17 GMT
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
	-	`sha256:5bd5fde0219b866984e02c69748a7c533734e7d3ce1c605e00b2794ba719ca78`  
		Last Modified: Mon, 14 Jun 2021 18:25:40 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ff67696fba822eac7dc90ce8b74a3463e180c1277ce1b5235dd553efd54d37`  
		Last Modified: Mon, 14 Jun 2021 18:25:53 GMT  
		Size: 12.0 MB (12011979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb05b150667473f58bd9ff97143e7addb941c15c23d7c0190462052e171a5d3`  
		Last Modified: Mon, 14 Jun 2021 18:25:40 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417ec686bccf8c11c7e167450f76c56e965e0d895b8a67d2959fa0cd8e0f46c6`  
		Last Modified: Mon, 14 Jun 2021 18:25:39 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e7f7e817f7b000e684b2477e658283e3bc5e32f705e2a1af3eb2171451ab1a`  
		Last Modified: Mon, 14 Jun 2021 18:25:38 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9adbfef5bd1c4ce567e8643e7eb3ac228fc89e60afffa0d4ad65188836ee10e`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46951e23f2c6f042a74af530655917c470e7e58bd428811bea889f06ece060f3`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b702d713b07cb19c098b0a4c2ad22de8111ab140c99b88deb21ffa5f10870f`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1554c780202a1e2bfb6cafbf73148847f97c535c407f63f750903997105d516f`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a72ab2ef98ce84364537328634d5a56cb6c9080cdec9988778c0e15d451dc51`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0cb0fb150ef4d4bb3e78339539c6453dcdf1d1b11d50728bb72e262b603fa9`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d8666b345f227a53b8d4cc8698ebe05b454caf116f8329e30d4328ba56896e`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bce3d7ad9504e8b1a2a5f46b50605a7e895686efeae62529b2fb0c8210a2e7`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d806bd36723a790387c5f61446d9b73da291b1e1592e6943b28686f3dc50fb39`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddf127d6e3c5443190a309b2f703cfd1d079beea71723b1507958dbbf2b5cab`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace91f2d94fe0fd5d53fce078d832db72cc38e2ef7692a44f57f9377dcbf3f8f`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f8adfaab4745797ca3869f6e54a87e5c399e56609635f7b74b039fb8f9fc00`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca3d4ed717fc9e7154ad94da8a5ea30b61ba4dfe9ec25bdcfcb55e6291cbec7`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 274.6 KB (274630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deafc6c05519d23d4709cd8504c83ff6c43943477ddcaf57ae7a871acdbdf489`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.2-alpine`

```console
$ docker pull caddy@sha256:2a518987da6ad50fba4fa2ce40b159460bc68d42e4d37c7784c118470e738821
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.4.2-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:c3176ebaceec5d64a4892205d7cf3d32da87e2fcbbb8a47d787ef4200ef0e6d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14649179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57e953391a547aacb19ba079ee6713b24b8400352d6d95a8a43e79fb035ec0f7`
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
# Mon, 14 Jun 2021 17:19:37 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:19:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:19:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:19:41 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:19:41 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:19:41 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:19:41 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:19:41 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:19:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:19:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:19:43 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:19:43 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:19:43 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:19:44 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:19:44 GMT
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
	-	`sha256:037bdadcf837298422d86bb75d10aa9ea21eaaf0969e1d8e99b730b07208eb03`  
		Last Modified: Mon, 14 Jun 2021 17:20:16 GMT  
		Size: 11.5 MB (11530800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9785de7e5400398efa43aedd6416426c14e3101f52a5930b52b6e8ea3a0cd96`  
		Last Modified: Mon, 14 Jun 2021 17:20:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:53bc8c15c11306be1cd426dffb91df56e5dc186ae54c22eb08996f14c647378f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13817125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dd81d0e3a6035d5df068c9af8811281698921854e5190944b1f7a079651bb7d`
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
# Mon, 14 Jun 2021 17:49:40 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:49:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:49:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:49:44 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:49:44 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:49:44 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:49:44 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:49:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:49:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:49:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:49:46 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:49:46 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:49:47 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:49:47 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:49:47 GMT
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
	-	`sha256:028e0db410d042e12d6b3f64499cc00ae7298c02382ba1105cdc5ee03aaed549`  
		Last Modified: Mon, 14 Jun 2021 17:50:59 GMT  
		Size: 10.9 MB (10888459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64dbe91d32616efff4ec27f049638b231cfd0091a68480d45a21791d44b469c`  
		Last Modified: Mon, 14 Jun 2021 17:50:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:6fc967765fceab93d7838f17d2eeceddc56e21a65654e3ba92c799437ff09280
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13593827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d1b6dc4a59a634275f3c206036245997415a7d1894697b43d1dadc232712e8e`
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
# Mon, 14 Jun 2021 17:57:41 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:57:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:57:44 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:57:45 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:57:45 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:57:45 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:57:45 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:57:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:57:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:57:47 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:57:47 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:57:48 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:57:48 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:57:48 GMT
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
	-	`sha256:e97e805578bb88faf1e3b052fe899c9818d27e0e114574198d5e3d45a8faf1b9`  
		Last Modified: Mon, 14 Jun 2021 17:59:01 GMT  
		Size: 10.9 MB (10864008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee92873b0980eae80c33cd1bd74d1b35754b48c89cbe68088f4e98b4dd04e2f`  
		Last Modified: Mon, 14 Jun 2021 17:58:59 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:1f49cc95c1e8ebd7fe139595b64b8d3b2cbdafff4c46ff46bc4516054a50e3ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13466108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:749cdbfee8dde296c03efb611b07c067ca297771a1314bbcbbba992429e899e7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:32:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 15 Jun 2021 22:32:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 15 Jun 2021 22:32:20 GMT
ENV CADDY_VERSION=v2.4.2
# Tue, 15 Jun 2021 22:32:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 15 Jun 2021 22:32:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:32:23 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 15 Jun 2021 22:32:24 GMT
ENV XDG_DATA_HOME=/data
# Tue, 15 Jun 2021 22:32:24 GMT
VOLUME [/config]
# Tue, 15 Jun 2021 22:32:24 GMT
VOLUME [/data]
# Tue, 15 Jun 2021 22:32:24 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Tue, 15 Jun 2021 22:32:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 15 Jun 2021 22:32:26 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 15 Jun 2021 22:32:26 GMT
EXPOSE 80
# Tue, 15 Jun 2021 22:32:26 GMT
EXPOSE 443
# Tue, 15 Jun 2021 22:32:26 GMT
EXPOSE 2019
# Tue, 15 Jun 2021 22:32:26 GMT
WORKDIR /srv
# Tue, 15 Jun 2021 22:32:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d0b72044755ebd2b829600b94a69aa9096bbb4bf9a01c1795b5b245261b99a`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 300.6 KB (300631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abde659ccf1d73128ef1e71a9701b014e0f27d4abf15b3d410d0474cdd0adb95`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0b93549f9104a9bb517f1ae15bd6ef4d44f83d21964728c50aa960b97098dc`  
		Last Modified: Tue, 15 Jun 2021 22:33:26 GMT  
		Size: 10.4 MB (10447450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69a851000e14247059ab07104ab76f86231aaa1a4fb5abb6b321e66a45003d3`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:7764cdcd665f8e23165bf385240e8951ab046dd6f54808b247b57e284882ecc5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13175121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c3b2d52d66b7076e6c98e715324384114a94b978294b836f566919d77faa909`
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
# Mon, 14 Jun 2021 18:16:57 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:17:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 18:17:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 18:17:56 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 18:18:00 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 18:18:08 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 18:18:15 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 18:18:26 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:18:36 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:18:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:18:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:18:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:19:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:19:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:19:27 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:19:32 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:19:38 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:19:43 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:19:49 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 18:19:56 GMT
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
	-	`sha256:d23e936288e88eac2d5280068486ab71f9023047b51d2c012a09fd305cc70e19`  
		Last Modified: Mon, 14 Jun 2021 18:21:33 GMT  
		Size: 10.1 MB (10053418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59596542df0c41e54f99fa862419a9f75ef8cfce5b1788110d747951a295518e`  
		Last Modified: Mon, 14 Jun 2021 18:21:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:c8d5cda3a4ef8a3fae917a732cd349372b1cc625071f9b3acc77a9033eb55e63
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14004446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5539a479891dabbacf899df4a9c0af209caf5e8b82799b452efd5c9093bd99`
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
# Mon, 14 Jun 2021 17:41:42 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:41:46 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:41:46 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:41:46 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:41:47 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:41:49 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:41:49 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:41:49 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:41:49 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:41:50 GMT
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
	-	`sha256:9b59880ffc79bf424b9fb38c497ec3d3edea77c4cbabb6b295bad830e4732008`  
		Last Modified: Mon, 14 Jun 2021 17:42:22 GMT  
		Size: 11.1 MB (11094948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4a0a3f3a72f3127538116c7943809378ae5921f09f19249fb98a578d261a49`  
		Last Modified: Mon, 14 Jun 2021 17:42:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.2-builder`

```console
$ docker pull caddy@sha256:3bef1d372a9949d4c020af490ed84a192382df2217da31603fc31b5acb200ba8
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

### `caddy:2.4.2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:03ffe16fc60ddb7be4684d7c3c8e257038b2c00864c027415e8b05fc120c28d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.9 MB (116937549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d58d2ab3ddba126c2fd014ebdac7030a6d1c5eac1d0c5ea0ac1509d9c8c882d`
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
# Thu, 10 Jun 2021 21:26:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:26:40 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:26:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:26:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:26:42 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:19:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:19:01 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:19:48 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:19:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:19:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:19:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:19:50 GMT
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
	-	`sha256:e25adedf14febf43281fc3b4750e8b0c50f2bb061ef8f5e16a829d3392fa447b`  
		Last Modified: Thu, 10 Jun 2021 21:35:42 GMT  
		Size: 106.1 MB (106136761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52c85161d43b0fdd8bb3ae8fdf77b9e4fc783bceb11f591ed3bbdf1e4722abd`  
		Last Modified: Thu, 10 Jun 2021 21:35:26 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20d66408196d46dd8f1b9f81fb5afa2219f5ca4c68a313ca1c49d3b908f755d`  
		Last Modified: Thu, 10 Jun 2021 23:19:40 GMT  
		Size: 6.4 MB (6395665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84f14058db07dc0560a9f209a7d8768b4ebd80f1426006dec9fe3b4d7c7bd25`  
		Last Modified: Mon, 14 Jun 2021 17:20:29 GMT  
		Size: 1.3 MB (1311168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86b5f727a9d842c09b761d61887e9298328559147dd8e911eb7c5f6fcf5bfc2`  
		Last Modified: Mon, 14 Jun 2021 17:20:29 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:af84e4e4719a6f04129f95de4a1dadacacae55e4b82f98cc9f883020f40860da
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.7 MB (112708776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbae3456b30daef0a0988bb5200978e3a8b2981efecdd2f7a811c692ed7bcc6d`
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
# Thu, 10 Jun 2021 22:01:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 22:01:50 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 22:01:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 22:01:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 22:01:52 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:15:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:15:37 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:49:58 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:49:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:49:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:49:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:50:00 GMT
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
	-	`sha256:f6a122050eb4da5951b1c88f56bfe65cb0c1a50d4e9869ad63787a8d0fc9ff1e`  
		Last Modified: Thu, 10 Jun 2021 22:15:45 GMT  
		Size: 102.4 MB (102351924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc08c6e1815e1794433258a6a0a93785a234db42641d49902c4f194c1d6abc82`  
		Last Modified: Thu, 10 Jun 2021 22:15:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2e5491ca84af37b9bdc0dfcb0a65b798aea4ab080785e1bba16e36672accd4`  
		Last Modified: Thu, 10 Jun 2021 23:16:52 GMT  
		Size: 6.2 MB (6230941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cecdb7ddd0ec1710ae049c902367f06a18606501ca9d1dbe17ec00349029fb8`  
		Last Modified: Mon, 14 Jun 2021 17:51:16 GMT  
		Size: 1.2 MB (1221680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1729fe2ea9a0baa2a26bc61d595958dcecfcb3f577dcebaca53051ec502bf397`  
		Last Modified: Mon, 14 Jun 2021 17:51:16 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2a428d87d883958655e8d72e6461ed205031fac28d71b943746dda7178f2e555
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.6 MB (111602497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da4e596b14ba8264520d8c3f799a567c9b7f3847ae587434759e51d9c667bf76`
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
# Thu, 10 Jun 2021 22:35:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 22:35:30 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 22:35:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 22:35:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 22:35:32 GMT
WORKDIR /go
# Fri, 11 Jun 2021 00:34:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Jun 2021 00:34:12 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:57:59 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:57:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:58:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:58:01 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:58:01 GMT
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
	-	`sha256:3e05d01ffccbffea159372f8065e42d62b484e73624dae1b567d908c12bb6fa3`  
		Last Modified: Thu, 10 Jun 2021 22:53:44 GMT  
		Size: 102.1 MB (102116599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9c0e093faea54528f8e070b0ad60f87674bf3a4654d312ccf7d110de2a6f6a`  
		Last Modified: Thu, 10 Jun 2021 22:53:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59aa8029ac012f4886ea6bced5e66e03743aff8bd41e8c7413cab0369c79c91b`  
		Last Modified: Fri, 11 Jun 2021 00:35:26 GMT  
		Size: 5.6 MB (5560992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a1e9ca701d6638943ef23a3969d9ba902fada02c041a3a797515d585882566`  
		Last Modified: Mon, 14 Jun 2021 17:59:18 GMT  
		Size: 1.2 MB (1219508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017f9bacdf7cdb13305fcaf052511ab74f9d9d2b9cbae1253957277cdb6cdd48`  
		Last Modified: Mon, 14 Jun 2021 17:59:17 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b0e22365417fa304ab483e3f2da3c7b79886ee3bced561c8113dd66b4e664fec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112151491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14b18c1aa44d74288d99db407cad68df0fb403a47cdad522a7524f856bb773f4`
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
# Thu, 10 Jun 2021 21:45:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:45:54 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:45:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:45:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:45:55 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:04:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:04:40 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:39:47 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:39:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:39:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:39:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:39:49 GMT
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
	-	`sha256:a9da95e357649360250671b270e39318d13b2ddff5d5aaac20081d588c9b6f74`  
		Last Modified: Thu, 10 Jun 2021 21:55:04 GMT  
		Size: 101.5 MB (101471730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a246c0d2a229c1d281fc3c1c9aa7fe651a820da43e66cd7ab7660e606d8d9824`  
		Last Modified: Thu, 10 Jun 2021 21:54:43 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2518188a669fe97c7d7feaf8a0ef8974bd167bc206832dc95bae562e6d972fe6`  
		Last Modified: Thu, 10 Jun 2021 23:05:37 GMT  
		Size: 6.5 MB (6483980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cb2ec8e0329ac1e5a6a5f1146f63479477cd73be5c2a0a676a12b3fda9485f`  
		Last Modified: Mon, 14 Jun 2021 17:40:46 GMT  
		Size: 1.2 MB (1201544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3538e34014117eaf3a7b09c03f2fcc11383c7bcebc701bcdfbf5a2a2a61906bb`  
		Last Modified: Mon, 14 Jun 2021 17:40:45 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:f8fc6696fb7cd73549cdc80e5889efd4c9ba480b9622ffe9f316c6e32b6068dc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (111016742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cbbf856cae07e092449ff2a67b42618d6082d532dec5969a4bfa5089b96b11c`
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
# Thu, 10 Jun 2021 21:27:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:27:48 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:27:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:28:04 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:28:11 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:16:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:16:36 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 18:20:23 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:20:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 18:20:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 18:20:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 18:20:58 GMT
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
	-	`sha256:c81f5fe451abbc39d3bdfca4378da5aa2c8b041d846b68db7b6004029734d919`  
		Last Modified: Thu, 10 Jun 2021 21:41:32 GMT  
		Size: 99.9 MB (99918197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9387c57f22b360d0c37409febd5288b34f77782689d3995e0092564a035eae10`  
		Last Modified: Thu, 10 Jun 2021 21:41:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af95f6a2bbd2f3bf752226a7020c5dcb4ba9e36df520e5b7dac8913f4f852d6e`  
		Last Modified: Thu, 10 Jun 2021 23:18:16 GMT  
		Size: 6.8 MB (6830748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994f06d8c6a86a071bc59b2d0644e6c4118c2a51d61edbf571623d36f9b1b987`  
		Last Modified: Mon, 14 Jun 2021 18:21:51 GMT  
		Size: 1.2 MB (1170526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54fa15ba38d0d74a3579bc4af43b527cc19bc368e7351ccaf85c90264bfc31c`  
		Last Modified: Mon, 14 Jun 2021 18:21:50 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:2d70ee7ce742b7eba9d3c4097f0ee5448f02a40e7cc10514c12bbd3272fa7448
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115888076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f08a6df8ec993ccbd835eee259d75804dc13b90f39ad9dccd7971136aecb356`
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
# Thu, 10 Jun 2021 21:52:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:52:35 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:52:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:52:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:52:38 GMT
WORKDIR /go
# Thu, 10 Jun 2021 22:58:58 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 22:58:59 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:41:55 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:41:55 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:41:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:41:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:41:57 GMT
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
	-	`sha256:4b203e6fc30bb6c460e0aea06ed2a200569017655c2678db9ce6fed7a17762cc`  
		Last Modified: Thu, 10 Jun 2021 22:03:02 GMT  
		Size: 105.3 MB (105259453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9fa95d716a4e0cf3f1602cd1def2172371118109ba036c7d525ac506357a1b`  
		Last Modified: Thu, 10 Jun 2021 22:02:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1ceddc3358bec9a3e7284afbcb0a578916db67c3a60fbc269cf78c11f26623`  
		Last Modified: Thu, 10 Jun 2021 22:59:42 GMT  
		Size: 6.5 MB (6479018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab4e3358d5deaa72e1a9a5207c52a6f1133bd89e6c424bb9cf4f0b9fbf2e5b6`  
		Last Modified: Mon, 14 Jun 2021 17:42:29 GMT  
		Size: 1.3 MB (1264529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29212836bbaacf27e155ad8002b1c2a6b5cd2dbe13986b27a57dc427357f2ce`  
		Last Modified: Mon, 14 Jun 2021 17:42:29 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2-builder` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:32914545de594aa79ff4231b61d5594f830641d124fb3cfa56e0575e940ec569
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2808449608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f1d0a4465ebc0bcefa7e5556bfb70eddabb69cf27ef61b558f45bef720fe883`
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
# Mon, 14 Jun 2021 18:21:36 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:21:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 18:22:12 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 14 Jun 2021 18:22:15 GMT
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
	-	`sha256:92f879ad577a7254271b2a27970912d5990740c6c23b65c14d3585b0b331b6b1`  
		Last Modified: Mon, 14 Jun 2021 18:26:07 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14bceb7d820e8f377e4a2d219ae96ee84dafd1055c85c1ce3deb22ea38cb8bf`  
		Last Modified: Mon, 14 Jun 2021 18:26:07 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ddb113a61bc728c0f730228bd4b782a04bcd9bec04ca60a8f46ca5b82e827a8`  
		Last Modified: Mon, 14 Jun 2021 18:26:08 GMT  
		Size: 1.7 MB (1730897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f05c3ba05a4dc7082b32ebd8dae3976fd8adb32927054b6fc0e3f137970df1`  
		Last Modified: Mon, 14 Jun 2021 18:26:07 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2-builder` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:3dc1e8d5170dfd5b5e6fbb34d885db2414827f33c49ca301aaaa82644bb7a6fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6437016101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:913b54138653e16a37ea51c2051dd30d0bc4ff76fece599b23b92c1aa7a11ff3`
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
# Mon, 14 Jun 2021 18:22:30 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:22:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 18:24:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 14 Jun 2021 18:24:02 GMT
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
	-	`sha256:3d01a14f10d204dac3535ad62c6b042cc9edc8c2c7c0996ecc45efbb896d5eed`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612bbd13a883cfddbf2977f7de24716a7978eea9f601ba5854f82d36f10068c4`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40a20ce35485bdd147339935426465c403bd3c52351030d040de662cec3253b`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.7 MB (1700121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a492d6062ee0783839f1bb22b289b12c884913a9018f1943add9b74a638df8f5`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.2-builder-alpine`

```console
$ docker pull caddy@sha256:746c493872f8b672a3d07e35ca12032e8378587480dd245d512aacd2d23a9aa9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.4.2-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:03ffe16fc60ddb7be4684d7c3c8e257038b2c00864c027415e8b05fc120c28d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.9 MB (116937549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d58d2ab3ddba126c2fd014ebdac7030a6d1c5eac1d0c5ea0ac1509d9c8c882d`
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
# Thu, 10 Jun 2021 21:26:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:26:40 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:26:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:26:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:26:42 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:19:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:19:01 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:19:48 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:19:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:19:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:19:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:19:50 GMT
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
	-	`sha256:e25adedf14febf43281fc3b4750e8b0c50f2bb061ef8f5e16a829d3392fa447b`  
		Last Modified: Thu, 10 Jun 2021 21:35:42 GMT  
		Size: 106.1 MB (106136761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52c85161d43b0fdd8bb3ae8fdf77b9e4fc783bceb11f591ed3bbdf1e4722abd`  
		Last Modified: Thu, 10 Jun 2021 21:35:26 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20d66408196d46dd8f1b9f81fb5afa2219f5ca4c68a313ca1c49d3b908f755d`  
		Last Modified: Thu, 10 Jun 2021 23:19:40 GMT  
		Size: 6.4 MB (6395665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84f14058db07dc0560a9f209a7d8768b4ebd80f1426006dec9fe3b4d7c7bd25`  
		Last Modified: Mon, 14 Jun 2021 17:20:29 GMT  
		Size: 1.3 MB (1311168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86b5f727a9d842c09b761d61887e9298328559147dd8e911eb7c5f6fcf5bfc2`  
		Last Modified: Mon, 14 Jun 2021 17:20:29 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:af84e4e4719a6f04129f95de4a1dadacacae55e4b82f98cc9f883020f40860da
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.7 MB (112708776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbae3456b30daef0a0988bb5200978e3a8b2981efecdd2f7a811c692ed7bcc6d`
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
# Thu, 10 Jun 2021 22:01:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 22:01:50 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 22:01:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 22:01:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 22:01:52 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:15:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:15:37 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:49:58 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:49:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:49:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:49:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:50:00 GMT
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
	-	`sha256:f6a122050eb4da5951b1c88f56bfe65cb0c1a50d4e9869ad63787a8d0fc9ff1e`  
		Last Modified: Thu, 10 Jun 2021 22:15:45 GMT  
		Size: 102.4 MB (102351924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc08c6e1815e1794433258a6a0a93785a234db42641d49902c4f194c1d6abc82`  
		Last Modified: Thu, 10 Jun 2021 22:15:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2e5491ca84af37b9bdc0dfcb0a65b798aea4ab080785e1bba16e36672accd4`  
		Last Modified: Thu, 10 Jun 2021 23:16:52 GMT  
		Size: 6.2 MB (6230941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cecdb7ddd0ec1710ae049c902367f06a18606501ca9d1dbe17ec00349029fb8`  
		Last Modified: Mon, 14 Jun 2021 17:51:16 GMT  
		Size: 1.2 MB (1221680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1729fe2ea9a0baa2a26bc61d595958dcecfcb3f577dcebaca53051ec502bf397`  
		Last Modified: Mon, 14 Jun 2021 17:51:16 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2a428d87d883958655e8d72e6461ed205031fac28d71b943746dda7178f2e555
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.6 MB (111602497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da4e596b14ba8264520d8c3f799a567c9b7f3847ae587434759e51d9c667bf76`
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
# Thu, 10 Jun 2021 22:35:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 22:35:30 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 22:35:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 22:35:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 22:35:32 GMT
WORKDIR /go
# Fri, 11 Jun 2021 00:34:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Jun 2021 00:34:12 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:57:59 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:57:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:58:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:58:01 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:58:01 GMT
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
	-	`sha256:3e05d01ffccbffea159372f8065e42d62b484e73624dae1b567d908c12bb6fa3`  
		Last Modified: Thu, 10 Jun 2021 22:53:44 GMT  
		Size: 102.1 MB (102116599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9c0e093faea54528f8e070b0ad60f87674bf3a4654d312ccf7d110de2a6f6a`  
		Last Modified: Thu, 10 Jun 2021 22:53:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59aa8029ac012f4886ea6bced5e66e03743aff8bd41e8c7413cab0369c79c91b`  
		Last Modified: Fri, 11 Jun 2021 00:35:26 GMT  
		Size: 5.6 MB (5560992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a1e9ca701d6638943ef23a3969d9ba902fada02c041a3a797515d585882566`  
		Last Modified: Mon, 14 Jun 2021 17:59:18 GMT  
		Size: 1.2 MB (1219508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017f9bacdf7cdb13305fcaf052511ab74f9d9d2b9cbae1253957277cdb6cdd48`  
		Last Modified: Mon, 14 Jun 2021 17:59:17 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b0e22365417fa304ab483e3f2da3c7b79886ee3bced561c8113dd66b4e664fec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112151491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14b18c1aa44d74288d99db407cad68df0fb403a47cdad522a7524f856bb773f4`
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
# Thu, 10 Jun 2021 21:45:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:45:54 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:45:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:45:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:45:55 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:04:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:04:40 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:39:47 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:39:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:39:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:39:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:39:49 GMT
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
	-	`sha256:a9da95e357649360250671b270e39318d13b2ddff5d5aaac20081d588c9b6f74`  
		Last Modified: Thu, 10 Jun 2021 21:55:04 GMT  
		Size: 101.5 MB (101471730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a246c0d2a229c1d281fc3c1c9aa7fe651a820da43e66cd7ab7660e606d8d9824`  
		Last Modified: Thu, 10 Jun 2021 21:54:43 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2518188a669fe97c7d7feaf8a0ef8974bd167bc206832dc95bae562e6d972fe6`  
		Last Modified: Thu, 10 Jun 2021 23:05:37 GMT  
		Size: 6.5 MB (6483980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cb2ec8e0329ac1e5a6a5f1146f63479477cd73be5c2a0a676a12b3fda9485f`  
		Last Modified: Mon, 14 Jun 2021 17:40:46 GMT  
		Size: 1.2 MB (1201544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3538e34014117eaf3a7b09c03f2fcc11383c7bcebc701bcdfbf5a2a2a61906bb`  
		Last Modified: Mon, 14 Jun 2021 17:40:45 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:f8fc6696fb7cd73549cdc80e5889efd4c9ba480b9622ffe9f316c6e32b6068dc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (111016742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cbbf856cae07e092449ff2a67b42618d6082d532dec5969a4bfa5089b96b11c`
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
# Thu, 10 Jun 2021 21:27:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:27:48 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:27:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:28:04 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:28:11 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:16:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:16:36 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 18:20:23 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:20:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 18:20:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 18:20:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 18:20:58 GMT
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
	-	`sha256:c81f5fe451abbc39d3bdfca4378da5aa2c8b041d846b68db7b6004029734d919`  
		Last Modified: Thu, 10 Jun 2021 21:41:32 GMT  
		Size: 99.9 MB (99918197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9387c57f22b360d0c37409febd5288b34f77782689d3995e0092564a035eae10`  
		Last Modified: Thu, 10 Jun 2021 21:41:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af95f6a2bbd2f3bf752226a7020c5dcb4ba9e36df520e5b7dac8913f4f852d6e`  
		Last Modified: Thu, 10 Jun 2021 23:18:16 GMT  
		Size: 6.8 MB (6830748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994f06d8c6a86a071bc59b2d0644e6c4118c2a51d61edbf571623d36f9b1b987`  
		Last Modified: Mon, 14 Jun 2021 18:21:51 GMT  
		Size: 1.2 MB (1170526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54fa15ba38d0d74a3579bc4af43b527cc19bc368e7351ccaf85c90264bfc31c`  
		Last Modified: Mon, 14 Jun 2021 18:21:50 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:2d70ee7ce742b7eba9d3c4097f0ee5448f02a40e7cc10514c12bbd3272fa7448
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115888076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f08a6df8ec993ccbd835eee259d75804dc13b90f39ad9dccd7971136aecb356`
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
# Thu, 10 Jun 2021 21:52:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:52:35 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:52:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:52:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:52:38 GMT
WORKDIR /go
# Thu, 10 Jun 2021 22:58:58 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 22:58:59 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:41:55 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:41:55 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:41:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:41:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:41:57 GMT
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
	-	`sha256:4b203e6fc30bb6c460e0aea06ed2a200569017655c2678db9ce6fed7a17762cc`  
		Last Modified: Thu, 10 Jun 2021 22:03:02 GMT  
		Size: 105.3 MB (105259453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9fa95d716a4e0cf3f1602cd1def2172371118109ba036c7d525ac506357a1b`  
		Last Modified: Thu, 10 Jun 2021 22:02:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1ceddc3358bec9a3e7284afbcb0a578916db67c3a60fbc269cf78c11f26623`  
		Last Modified: Thu, 10 Jun 2021 22:59:42 GMT  
		Size: 6.5 MB (6479018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab4e3358d5deaa72e1a9a5207c52a6f1133bd89e6c424bb9cf4f0b9fbf2e5b6`  
		Last Modified: Mon, 14 Jun 2021 17:42:29 GMT  
		Size: 1.3 MB (1264529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29212836bbaacf27e155ad8002b1c2a6b5cd2dbe13986b27a57dc427357f2ce`  
		Last Modified: Mon, 14 Jun 2021 17:42:29 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:6732f41f4155f39383864cbc74d3ac805ffda32377941904bfe0ee8d3516f679
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `caddy:2.4.2-builder-windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:32914545de594aa79ff4231b61d5594f830641d124fb3cfa56e0575e940ec569
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2808449608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f1d0a4465ebc0bcefa7e5556bfb70eddabb69cf27ef61b558f45bef720fe883`
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
# Mon, 14 Jun 2021 18:21:36 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:21:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 18:22:12 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 14 Jun 2021 18:22:15 GMT
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
	-	`sha256:92f879ad577a7254271b2a27970912d5990740c6c23b65c14d3585b0b331b6b1`  
		Last Modified: Mon, 14 Jun 2021 18:26:07 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14bceb7d820e8f377e4a2d219ae96ee84dafd1055c85c1ce3deb22ea38cb8bf`  
		Last Modified: Mon, 14 Jun 2021 18:26:07 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ddb113a61bc728c0f730228bd4b782a04bcd9bec04ca60a8f46ca5b82e827a8`  
		Last Modified: Mon, 14 Jun 2021 18:26:08 GMT  
		Size: 1.7 MB (1730897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f05c3ba05a4dc7082b32ebd8dae3976fd8adb32927054b6fc0e3f137970df1`  
		Last Modified: Mon, 14 Jun 2021 18:26:07 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.2-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:80f678464d89f88f808d926ddf79d5173f7367cc7c1e2381ecc3a7fb7307bb2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `caddy:2.4.2-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:3dc1e8d5170dfd5b5e6fbb34d885db2414827f33c49ca301aaaa82644bb7a6fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6437016101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:913b54138653e16a37ea51c2051dd30d0bc4ff76fece599b23b92c1aa7a11ff3`
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
# Mon, 14 Jun 2021 18:22:30 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:22:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 18:24:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 14 Jun 2021 18:24:02 GMT
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
	-	`sha256:3d01a14f10d204dac3535ad62c6b042cc9edc8c2c7c0996ecc45efbb896d5eed`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612bbd13a883cfddbf2977f7de24716a7978eea9f601ba5854f82d36f10068c4`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40a20ce35485bdd147339935426465c403bd3c52351030d040de662cec3253b`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.7 MB (1700121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a492d6062ee0783839f1bb22b289b12c884913a9018f1943add9b74a638df8f5`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.2-windowsservercore`

```console
$ docker pull caddy@sha256:6b1a7e2d64eea0fda092326bf2660a9f57caa3d9e0679b9b2916458ae71a2880
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `caddy:2.4.2-windowsservercore` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:84c41546a31938e07bc74b9535459f62221b5fa62f50aadb3f7138ceb0a638b7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2654297157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7933e1b45a92be68914695f31f1c84c86b602c5233536557c1ccee877d1216b0`
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
# Mon, 14 Jun 2021 18:15:56 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:16:40 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8d5cf4479e471d47fd067ce2fbe34c2015a96caedab95ca042aeb633956cbc2bb89c1bc4fe6593c1f96ca58bc66b21f32caa6b099122b9d500a3902245fa5105')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 14 Jun 2021 18:16:43 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 14 Jun 2021 18:16:45 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 14 Jun 2021 18:16:48 GMT
VOLUME [c:/config]
# Mon, 14 Jun 2021 18:16:50 GMT
VOLUME [c:/data]
# Mon, 14 Jun 2021 18:16:53 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:16:55 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:16:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:17:01 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:17:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:17:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:17:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:17:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:17:15 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:17:17 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:17:20 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:17:39 GMT
RUN caddy version
# Mon, 14 Jun 2021 18:17:41 GMT
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
	-	`sha256:07802e3c606e3b9298421527979a2b9797c286d601553a4f8c11271d67919b58`  
		Last Modified: Mon, 14 Jun 2021 18:25:04 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4847967ab228abb45531c45132179ebac7d55ea85bf85ea3f3f420aff0be2863`  
		Last Modified: Mon, 14 Jun 2021 18:25:17 GMT  
		Size: 12.0 MB (12025127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e590a115b7ca0fdadc5a634f9a3b1a58db5ac8a89765f1d00351421045e7dd62`  
		Last Modified: Mon, 14 Jun 2021 18:25:03 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a698c5067c38c742726c5f427f5f07d028e7768a91c4f2fd9a973f662a750b0`  
		Last Modified: Mon, 14 Jun 2021 18:25:03 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4d9bb89edb4e6f90cfacbb81068b117b3b8affe4430a23ddc2f8aa8b1803fa`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369f1dad8944bfe55423327ebaedf96f73e356ca6fd92d4e9a8d2fdbc6b6293c`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f126fec1b223ee19a7f02455cd95a68d8275a8589273ff50b9f7ffbad72a882`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3949035d30e3b80897ac6fc2b4776dccd30680886816cfe8c27ed8bc8c0c595`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c1d9637c1841b64adc5cccf8a5ce5275754886c8c7eb26005eef69727bc101`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa902629ee85278422f20ba99ecc504972ce7c6263bdfa5f1d0a51103ed3e272`  
		Last Modified: Mon, 14 Jun 2021 18:24:59 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7795b0b452df39f057bb8fb233e6862dba05177f3c225da1443588e4e7ec3326`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b936a424e3378bda5aaa142367741f0486702c00117d08a527d36f3876cc7a0`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74ede6be2a18e8c915b5e55628de5a029cf0bb5b69edc917dd8f1c6e1426ee6`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cdf00e847ddd24f1ba768e20fd224aa86a161461a82d3a210f1d5ce1f28cb2`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51405f73ce954be2e339c2cfa1a28109cd371d9fb8986047079a8ba8cc4a9d7a`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38f74dca7b51152c809bf35c007d8affbfc36cae366903110509bdba8f3bde6`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca41d82a7c33c949c331f1ff7958f3ec1551f1bda90faaf07d7b112111a251bc`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582046a83a61d6a9e5701d72c1102b19e9e9ba65665c38d03618e34acdaa5c36`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 300.2 KB (300242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a16f8caea000f3748f024fd14e1419c77091e71e4c220b06a94dc02ffc746c`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.2-windowsservercore` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:4d5c4f12af6b434f907c262accbfeef1c9eb948d91bb5113bde117904152d9bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278396558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b0d047c64024dd8b9ee7374a59e2e19a219277308f3db92d25f22e903b4f6fb`
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
# Mon, 14 Jun 2021 18:17:52 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:19:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8d5cf4479e471d47fd067ce2fbe34c2015a96caedab95ca042aeb633956cbc2bb89c1bc4fe6593c1f96ca58bc66b21f32caa6b099122b9d500a3902245fa5105')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 14 Jun 2021 18:19:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 14 Jun 2021 18:19:41 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 14 Jun 2021 18:19:43 GMT
VOLUME [c:/config]
# Mon, 14 Jun 2021 18:19:46 GMT
VOLUME [c:/data]
# Mon, 14 Jun 2021 18:19:48 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:19:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:19:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:19:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:19:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:20:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:20:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:20:04 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:20:07 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:20:09 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:20:11 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:21:14 GMT
RUN caddy version
# Mon, 14 Jun 2021 18:21:17 GMT
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
	-	`sha256:5bd5fde0219b866984e02c69748a7c533734e7d3ce1c605e00b2794ba719ca78`  
		Last Modified: Mon, 14 Jun 2021 18:25:40 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ff67696fba822eac7dc90ce8b74a3463e180c1277ce1b5235dd553efd54d37`  
		Last Modified: Mon, 14 Jun 2021 18:25:53 GMT  
		Size: 12.0 MB (12011979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb05b150667473f58bd9ff97143e7addb941c15c23d7c0190462052e171a5d3`  
		Last Modified: Mon, 14 Jun 2021 18:25:40 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417ec686bccf8c11c7e167450f76c56e965e0d895b8a67d2959fa0cd8e0f46c6`  
		Last Modified: Mon, 14 Jun 2021 18:25:39 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e7f7e817f7b000e684b2477e658283e3bc5e32f705e2a1af3eb2171451ab1a`  
		Last Modified: Mon, 14 Jun 2021 18:25:38 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9adbfef5bd1c4ce567e8643e7eb3ac228fc89e60afffa0d4ad65188836ee10e`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46951e23f2c6f042a74af530655917c470e7e58bd428811bea889f06ece060f3`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b702d713b07cb19c098b0a4c2ad22de8111ab140c99b88deb21ffa5f10870f`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1554c780202a1e2bfb6cafbf73148847f97c535c407f63f750903997105d516f`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a72ab2ef98ce84364537328634d5a56cb6c9080cdec9988778c0e15d451dc51`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0cb0fb150ef4d4bb3e78339539c6453dcdf1d1b11d50728bb72e262b603fa9`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d8666b345f227a53b8d4cc8698ebe05b454caf116f8329e30d4328ba56896e`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bce3d7ad9504e8b1a2a5f46b50605a7e895686efeae62529b2fb0c8210a2e7`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d806bd36723a790387c5f61446d9b73da291b1e1592e6943b28686f3dc50fb39`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddf127d6e3c5443190a309b2f703cfd1d079beea71723b1507958dbbf2b5cab`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace91f2d94fe0fd5d53fce078d832db72cc38e2ef7692a44f57f9377dcbf3f8f`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f8adfaab4745797ca3869f6e54a87e5c399e56609635f7b74b039fb8f9fc00`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca3d4ed717fc9e7154ad94da8a5ea30b61ba4dfe9ec25bdcfcb55e6291cbec7`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 274.6 KB (274630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deafc6c05519d23d4709cd8504c83ff6c43943477ddcaf57ae7a871acdbdf489`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:1791c7844819a24a2bae3a297d7e61abe6b39e642e60743a94def9537939148a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `caddy:2.4.2-windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:84c41546a31938e07bc74b9535459f62221b5fa62f50aadb3f7138ceb0a638b7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2654297157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7933e1b45a92be68914695f31f1c84c86b602c5233536557c1ccee877d1216b0`
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
# Mon, 14 Jun 2021 18:15:56 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:16:40 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8d5cf4479e471d47fd067ce2fbe34c2015a96caedab95ca042aeb633956cbc2bb89c1bc4fe6593c1f96ca58bc66b21f32caa6b099122b9d500a3902245fa5105')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 14 Jun 2021 18:16:43 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 14 Jun 2021 18:16:45 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 14 Jun 2021 18:16:48 GMT
VOLUME [c:/config]
# Mon, 14 Jun 2021 18:16:50 GMT
VOLUME [c:/data]
# Mon, 14 Jun 2021 18:16:53 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:16:55 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:16:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:17:01 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:17:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:17:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:17:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:17:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:17:15 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:17:17 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:17:20 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:17:39 GMT
RUN caddy version
# Mon, 14 Jun 2021 18:17:41 GMT
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
	-	`sha256:07802e3c606e3b9298421527979a2b9797c286d601553a4f8c11271d67919b58`  
		Last Modified: Mon, 14 Jun 2021 18:25:04 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4847967ab228abb45531c45132179ebac7d55ea85bf85ea3f3f420aff0be2863`  
		Last Modified: Mon, 14 Jun 2021 18:25:17 GMT  
		Size: 12.0 MB (12025127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e590a115b7ca0fdadc5a634f9a3b1a58db5ac8a89765f1d00351421045e7dd62`  
		Last Modified: Mon, 14 Jun 2021 18:25:03 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a698c5067c38c742726c5f427f5f07d028e7768a91c4f2fd9a973f662a750b0`  
		Last Modified: Mon, 14 Jun 2021 18:25:03 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4d9bb89edb4e6f90cfacbb81068b117b3b8affe4430a23ddc2f8aa8b1803fa`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369f1dad8944bfe55423327ebaedf96f73e356ca6fd92d4e9a8d2fdbc6b6293c`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f126fec1b223ee19a7f02455cd95a68d8275a8589273ff50b9f7ffbad72a882`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3949035d30e3b80897ac6fc2b4776dccd30680886816cfe8c27ed8bc8c0c595`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c1d9637c1841b64adc5cccf8a5ce5275754886c8c7eb26005eef69727bc101`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa902629ee85278422f20ba99ecc504972ce7c6263bdfa5f1d0a51103ed3e272`  
		Last Modified: Mon, 14 Jun 2021 18:24:59 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7795b0b452df39f057bb8fb233e6862dba05177f3c225da1443588e4e7ec3326`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b936a424e3378bda5aaa142367741f0486702c00117d08a527d36f3876cc7a0`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74ede6be2a18e8c915b5e55628de5a029cf0bb5b69edc917dd8f1c6e1426ee6`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cdf00e847ddd24f1ba768e20fd224aa86a161461a82d3a210f1d5ce1f28cb2`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51405f73ce954be2e339c2cfa1a28109cd371d9fb8986047079a8ba8cc4a9d7a`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38f74dca7b51152c809bf35c007d8affbfc36cae366903110509bdba8f3bde6`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca41d82a7c33c949c331f1ff7958f3ec1551f1bda90faaf07d7b112111a251bc`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582046a83a61d6a9e5701d72c1102b19e9e9ba65665c38d03618e34acdaa5c36`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 300.2 KB (300242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a16f8caea000f3748f024fd14e1419c77091e71e4c220b06a94dc02ffc746c`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:076e0573f1533c025ab55f299e32833e09ed22b4c52605a2351aba5baa2f585d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `caddy:2.4.2-windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:4d5c4f12af6b434f907c262accbfeef1c9eb948d91bb5113bde117904152d9bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278396558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b0d047c64024dd8b9ee7374a59e2e19a219277308f3db92d25f22e903b4f6fb`
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
# Mon, 14 Jun 2021 18:17:52 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:19:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8d5cf4479e471d47fd067ce2fbe34c2015a96caedab95ca042aeb633956cbc2bb89c1bc4fe6593c1f96ca58bc66b21f32caa6b099122b9d500a3902245fa5105')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 14 Jun 2021 18:19:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 14 Jun 2021 18:19:41 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 14 Jun 2021 18:19:43 GMT
VOLUME [c:/config]
# Mon, 14 Jun 2021 18:19:46 GMT
VOLUME [c:/data]
# Mon, 14 Jun 2021 18:19:48 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:19:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:19:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:19:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:19:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:20:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:20:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:20:04 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:20:07 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:20:09 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:20:11 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:21:14 GMT
RUN caddy version
# Mon, 14 Jun 2021 18:21:17 GMT
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
	-	`sha256:5bd5fde0219b866984e02c69748a7c533734e7d3ce1c605e00b2794ba719ca78`  
		Last Modified: Mon, 14 Jun 2021 18:25:40 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ff67696fba822eac7dc90ce8b74a3463e180c1277ce1b5235dd553efd54d37`  
		Last Modified: Mon, 14 Jun 2021 18:25:53 GMT  
		Size: 12.0 MB (12011979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb05b150667473f58bd9ff97143e7addb941c15c23d7c0190462052e171a5d3`  
		Last Modified: Mon, 14 Jun 2021 18:25:40 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417ec686bccf8c11c7e167450f76c56e965e0d895b8a67d2959fa0cd8e0f46c6`  
		Last Modified: Mon, 14 Jun 2021 18:25:39 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e7f7e817f7b000e684b2477e658283e3bc5e32f705e2a1af3eb2171451ab1a`  
		Last Modified: Mon, 14 Jun 2021 18:25:38 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9adbfef5bd1c4ce567e8643e7eb3ac228fc89e60afffa0d4ad65188836ee10e`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46951e23f2c6f042a74af530655917c470e7e58bd428811bea889f06ece060f3`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b702d713b07cb19c098b0a4c2ad22de8111ab140c99b88deb21ffa5f10870f`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1554c780202a1e2bfb6cafbf73148847f97c535c407f63f750903997105d516f`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a72ab2ef98ce84364537328634d5a56cb6c9080cdec9988778c0e15d451dc51`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0cb0fb150ef4d4bb3e78339539c6453dcdf1d1b11d50728bb72e262b603fa9`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d8666b345f227a53b8d4cc8698ebe05b454caf116f8329e30d4328ba56896e`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bce3d7ad9504e8b1a2a5f46b50605a7e895686efeae62529b2fb0c8210a2e7`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d806bd36723a790387c5f61446d9b73da291b1e1592e6943b28686f3dc50fb39`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddf127d6e3c5443190a309b2f703cfd1d079beea71723b1507958dbbf2b5cab`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace91f2d94fe0fd5d53fce078d832db72cc38e2ef7692a44f57f9377dcbf3f8f`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f8adfaab4745797ca3869f6e54a87e5c399e56609635f7b74b039fb8f9fc00`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca3d4ed717fc9e7154ad94da8a5ea30b61ba4dfe9ec25bdcfcb55e6291cbec7`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 274.6 KB (274630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deafc6c05519d23d4709cd8504c83ff6c43943477ddcaf57ae7a871acdbdf489`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:2a518987da6ad50fba4fa2ce40b159460bc68d42e4d37c7784c118470e738821
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
$ docker pull caddy@sha256:c3176ebaceec5d64a4892205d7cf3d32da87e2fcbbb8a47d787ef4200ef0e6d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14649179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57e953391a547aacb19ba079ee6713b24b8400352d6d95a8a43e79fb035ec0f7`
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
# Mon, 14 Jun 2021 17:19:37 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:19:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:19:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:19:41 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:19:41 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:19:41 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:19:41 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:19:41 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:19:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:19:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:19:43 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:19:43 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:19:43 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:19:44 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:19:44 GMT
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
	-	`sha256:037bdadcf837298422d86bb75d10aa9ea21eaaf0969e1d8e99b730b07208eb03`  
		Last Modified: Mon, 14 Jun 2021 17:20:16 GMT  
		Size: 11.5 MB (11530800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9785de7e5400398efa43aedd6416426c14e3101f52a5930b52b6e8ea3a0cd96`  
		Last Modified: Mon, 14 Jun 2021 17:20:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:53bc8c15c11306be1cd426dffb91df56e5dc186ae54c22eb08996f14c647378f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13817125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dd81d0e3a6035d5df068c9af8811281698921854e5190944b1f7a079651bb7d`
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
# Mon, 14 Jun 2021 17:49:40 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:49:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:49:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:49:44 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:49:44 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:49:44 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:49:44 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:49:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:49:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:49:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:49:46 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:49:46 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:49:47 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:49:47 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:49:47 GMT
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
	-	`sha256:028e0db410d042e12d6b3f64499cc00ae7298c02382ba1105cdc5ee03aaed549`  
		Last Modified: Mon, 14 Jun 2021 17:50:59 GMT  
		Size: 10.9 MB (10888459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64dbe91d32616efff4ec27f049638b231cfd0091a68480d45a21791d44b469c`  
		Last Modified: Mon, 14 Jun 2021 17:50:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:6fc967765fceab93d7838f17d2eeceddc56e21a65654e3ba92c799437ff09280
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13593827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d1b6dc4a59a634275f3c206036245997415a7d1894697b43d1dadc232712e8e`
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
# Mon, 14 Jun 2021 17:57:41 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:57:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:57:44 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:57:45 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:57:45 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:57:45 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:57:45 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:57:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:57:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:57:47 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:57:47 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:57:48 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:57:48 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:57:48 GMT
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
	-	`sha256:e97e805578bb88faf1e3b052fe899c9818d27e0e114574198d5e3d45a8faf1b9`  
		Last Modified: Mon, 14 Jun 2021 17:59:01 GMT  
		Size: 10.9 MB (10864008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee92873b0980eae80c33cd1bd74d1b35754b48c89cbe68088f4e98b4dd04e2f`  
		Last Modified: Mon, 14 Jun 2021 17:58:59 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:1f49cc95c1e8ebd7fe139595b64b8d3b2cbdafff4c46ff46bc4516054a50e3ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13466108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:749cdbfee8dde296c03efb611b07c067ca297771a1314bbcbbba992429e899e7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:32:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 15 Jun 2021 22:32:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 15 Jun 2021 22:32:20 GMT
ENV CADDY_VERSION=v2.4.2
# Tue, 15 Jun 2021 22:32:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 15 Jun 2021 22:32:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:32:23 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 15 Jun 2021 22:32:24 GMT
ENV XDG_DATA_HOME=/data
# Tue, 15 Jun 2021 22:32:24 GMT
VOLUME [/config]
# Tue, 15 Jun 2021 22:32:24 GMT
VOLUME [/data]
# Tue, 15 Jun 2021 22:32:24 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Tue, 15 Jun 2021 22:32:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 15 Jun 2021 22:32:26 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 15 Jun 2021 22:32:26 GMT
EXPOSE 80
# Tue, 15 Jun 2021 22:32:26 GMT
EXPOSE 443
# Tue, 15 Jun 2021 22:32:26 GMT
EXPOSE 2019
# Tue, 15 Jun 2021 22:32:26 GMT
WORKDIR /srv
# Tue, 15 Jun 2021 22:32:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d0b72044755ebd2b829600b94a69aa9096bbb4bf9a01c1795b5b245261b99a`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 300.6 KB (300631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abde659ccf1d73128ef1e71a9701b014e0f27d4abf15b3d410d0474cdd0adb95`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0b93549f9104a9bb517f1ae15bd6ef4d44f83d21964728c50aa960b97098dc`  
		Last Modified: Tue, 15 Jun 2021 22:33:26 GMT  
		Size: 10.4 MB (10447450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69a851000e14247059ab07104ab76f86231aaa1a4fb5abb6b321e66a45003d3`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:7764cdcd665f8e23165bf385240e8951ab046dd6f54808b247b57e284882ecc5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13175121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c3b2d52d66b7076e6c98e715324384114a94b978294b836f566919d77faa909`
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
# Mon, 14 Jun 2021 18:16:57 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:17:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 18:17:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 18:17:56 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 18:18:00 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 18:18:08 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 18:18:15 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 18:18:26 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:18:36 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:18:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:18:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:18:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:19:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:19:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:19:27 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:19:32 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:19:38 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:19:43 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:19:49 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 18:19:56 GMT
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
	-	`sha256:d23e936288e88eac2d5280068486ab71f9023047b51d2c012a09fd305cc70e19`  
		Last Modified: Mon, 14 Jun 2021 18:21:33 GMT  
		Size: 10.1 MB (10053418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59596542df0c41e54f99fa862419a9f75ef8cfce5b1788110d747951a295518e`  
		Last Modified: Mon, 14 Jun 2021 18:21:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:c8d5cda3a4ef8a3fae917a732cd349372b1cc625071f9b3acc77a9033eb55e63
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14004446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5539a479891dabbacf899df4a9c0af209caf5e8b82799b452efd5c9093bd99`
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
# Mon, 14 Jun 2021 17:41:42 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:41:46 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:41:46 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:41:46 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:41:47 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:41:49 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:41:49 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:41:49 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:41:49 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:41:50 GMT
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
	-	`sha256:9b59880ffc79bf424b9fb38c497ec3d3edea77c4cbabb6b295bad830e4732008`  
		Last Modified: Mon, 14 Jun 2021 17:42:22 GMT  
		Size: 11.1 MB (11094948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4a0a3f3a72f3127538116c7943809378ae5921f09f19249fb98a578d261a49`  
		Last Modified: Mon, 14 Jun 2021 17:42:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:3bef1d372a9949d4c020af490ed84a192382df2217da31603fc31b5acb200ba8
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
$ docker pull caddy@sha256:03ffe16fc60ddb7be4684d7c3c8e257038b2c00864c027415e8b05fc120c28d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.9 MB (116937549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d58d2ab3ddba126c2fd014ebdac7030a6d1c5eac1d0c5ea0ac1509d9c8c882d`
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
# Thu, 10 Jun 2021 21:26:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:26:40 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:26:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:26:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:26:42 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:19:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:19:01 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:19:48 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:19:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:19:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:19:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:19:50 GMT
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
	-	`sha256:e25adedf14febf43281fc3b4750e8b0c50f2bb061ef8f5e16a829d3392fa447b`  
		Last Modified: Thu, 10 Jun 2021 21:35:42 GMT  
		Size: 106.1 MB (106136761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52c85161d43b0fdd8bb3ae8fdf77b9e4fc783bceb11f591ed3bbdf1e4722abd`  
		Last Modified: Thu, 10 Jun 2021 21:35:26 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20d66408196d46dd8f1b9f81fb5afa2219f5ca4c68a313ca1c49d3b908f755d`  
		Last Modified: Thu, 10 Jun 2021 23:19:40 GMT  
		Size: 6.4 MB (6395665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84f14058db07dc0560a9f209a7d8768b4ebd80f1426006dec9fe3b4d7c7bd25`  
		Last Modified: Mon, 14 Jun 2021 17:20:29 GMT  
		Size: 1.3 MB (1311168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86b5f727a9d842c09b761d61887e9298328559147dd8e911eb7c5f6fcf5bfc2`  
		Last Modified: Mon, 14 Jun 2021 17:20:29 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:af84e4e4719a6f04129f95de4a1dadacacae55e4b82f98cc9f883020f40860da
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.7 MB (112708776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbae3456b30daef0a0988bb5200978e3a8b2981efecdd2f7a811c692ed7bcc6d`
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
# Thu, 10 Jun 2021 22:01:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 22:01:50 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 22:01:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 22:01:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 22:01:52 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:15:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:15:37 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:49:58 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:49:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:49:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:49:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:50:00 GMT
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
	-	`sha256:f6a122050eb4da5951b1c88f56bfe65cb0c1a50d4e9869ad63787a8d0fc9ff1e`  
		Last Modified: Thu, 10 Jun 2021 22:15:45 GMT  
		Size: 102.4 MB (102351924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc08c6e1815e1794433258a6a0a93785a234db42641d49902c4f194c1d6abc82`  
		Last Modified: Thu, 10 Jun 2021 22:15:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2e5491ca84af37b9bdc0dfcb0a65b798aea4ab080785e1bba16e36672accd4`  
		Last Modified: Thu, 10 Jun 2021 23:16:52 GMT  
		Size: 6.2 MB (6230941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cecdb7ddd0ec1710ae049c902367f06a18606501ca9d1dbe17ec00349029fb8`  
		Last Modified: Mon, 14 Jun 2021 17:51:16 GMT  
		Size: 1.2 MB (1221680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1729fe2ea9a0baa2a26bc61d595958dcecfcb3f577dcebaca53051ec502bf397`  
		Last Modified: Mon, 14 Jun 2021 17:51:16 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2a428d87d883958655e8d72e6461ed205031fac28d71b943746dda7178f2e555
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.6 MB (111602497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da4e596b14ba8264520d8c3f799a567c9b7f3847ae587434759e51d9c667bf76`
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
# Thu, 10 Jun 2021 22:35:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 22:35:30 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 22:35:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 22:35:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 22:35:32 GMT
WORKDIR /go
# Fri, 11 Jun 2021 00:34:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Jun 2021 00:34:12 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:57:59 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:57:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:58:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:58:01 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:58:01 GMT
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
	-	`sha256:3e05d01ffccbffea159372f8065e42d62b484e73624dae1b567d908c12bb6fa3`  
		Last Modified: Thu, 10 Jun 2021 22:53:44 GMT  
		Size: 102.1 MB (102116599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9c0e093faea54528f8e070b0ad60f87674bf3a4654d312ccf7d110de2a6f6a`  
		Last Modified: Thu, 10 Jun 2021 22:53:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59aa8029ac012f4886ea6bced5e66e03743aff8bd41e8c7413cab0369c79c91b`  
		Last Modified: Fri, 11 Jun 2021 00:35:26 GMT  
		Size: 5.6 MB (5560992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a1e9ca701d6638943ef23a3969d9ba902fada02c041a3a797515d585882566`  
		Last Modified: Mon, 14 Jun 2021 17:59:18 GMT  
		Size: 1.2 MB (1219508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017f9bacdf7cdb13305fcaf052511ab74f9d9d2b9cbae1253957277cdb6cdd48`  
		Last Modified: Mon, 14 Jun 2021 17:59:17 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b0e22365417fa304ab483e3f2da3c7b79886ee3bced561c8113dd66b4e664fec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112151491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14b18c1aa44d74288d99db407cad68df0fb403a47cdad522a7524f856bb773f4`
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
# Thu, 10 Jun 2021 21:45:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:45:54 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:45:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:45:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:45:55 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:04:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:04:40 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:39:47 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:39:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:39:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:39:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:39:49 GMT
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
	-	`sha256:a9da95e357649360250671b270e39318d13b2ddff5d5aaac20081d588c9b6f74`  
		Last Modified: Thu, 10 Jun 2021 21:55:04 GMT  
		Size: 101.5 MB (101471730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a246c0d2a229c1d281fc3c1c9aa7fe651a820da43e66cd7ab7660e606d8d9824`  
		Last Modified: Thu, 10 Jun 2021 21:54:43 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2518188a669fe97c7d7feaf8a0ef8974bd167bc206832dc95bae562e6d972fe6`  
		Last Modified: Thu, 10 Jun 2021 23:05:37 GMT  
		Size: 6.5 MB (6483980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cb2ec8e0329ac1e5a6a5f1146f63479477cd73be5c2a0a676a12b3fda9485f`  
		Last Modified: Mon, 14 Jun 2021 17:40:46 GMT  
		Size: 1.2 MB (1201544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3538e34014117eaf3a7b09c03f2fcc11383c7bcebc701bcdfbf5a2a2a61906bb`  
		Last Modified: Mon, 14 Jun 2021 17:40:45 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:f8fc6696fb7cd73549cdc80e5889efd4c9ba480b9622ffe9f316c6e32b6068dc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (111016742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cbbf856cae07e092449ff2a67b42618d6082d532dec5969a4bfa5089b96b11c`
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
# Thu, 10 Jun 2021 21:27:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:27:48 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:27:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:28:04 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:28:11 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:16:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:16:36 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 18:20:23 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:20:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 18:20:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 18:20:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 18:20:58 GMT
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
	-	`sha256:c81f5fe451abbc39d3bdfca4378da5aa2c8b041d846b68db7b6004029734d919`  
		Last Modified: Thu, 10 Jun 2021 21:41:32 GMT  
		Size: 99.9 MB (99918197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9387c57f22b360d0c37409febd5288b34f77782689d3995e0092564a035eae10`  
		Last Modified: Thu, 10 Jun 2021 21:41:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af95f6a2bbd2f3bf752226a7020c5dcb4ba9e36df520e5b7dac8913f4f852d6e`  
		Last Modified: Thu, 10 Jun 2021 23:18:16 GMT  
		Size: 6.8 MB (6830748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994f06d8c6a86a071bc59b2d0644e6c4118c2a51d61edbf571623d36f9b1b987`  
		Last Modified: Mon, 14 Jun 2021 18:21:51 GMT  
		Size: 1.2 MB (1170526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54fa15ba38d0d74a3579bc4af43b527cc19bc368e7351ccaf85c90264bfc31c`  
		Last Modified: Mon, 14 Jun 2021 18:21:50 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:2d70ee7ce742b7eba9d3c4097f0ee5448f02a40e7cc10514c12bbd3272fa7448
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115888076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f08a6df8ec993ccbd835eee259d75804dc13b90f39ad9dccd7971136aecb356`
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
# Thu, 10 Jun 2021 21:52:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:52:35 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:52:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:52:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:52:38 GMT
WORKDIR /go
# Thu, 10 Jun 2021 22:58:58 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 22:58:59 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:41:55 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:41:55 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:41:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:41:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:41:57 GMT
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
	-	`sha256:4b203e6fc30bb6c460e0aea06ed2a200569017655c2678db9ce6fed7a17762cc`  
		Last Modified: Thu, 10 Jun 2021 22:03:02 GMT  
		Size: 105.3 MB (105259453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9fa95d716a4e0cf3f1602cd1def2172371118109ba036c7d525ac506357a1b`  
		Last Modified: Thu, 10 Jun 2021 22:02:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1ceddc3358bec9a3e7284afbcb0a578916db67c3a60fbc269cf78c11f26623`  
		Last Modified: Thu, 10 Jun 2021 22:59:42 GMT  
		Size: 6.5 MB (6479018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab4e3358d5deaa72e1a9a5207c52a6f1133bd89e6c424bb9cf4f0b9fbf2e5b6`  
		Last Modified: Mon, 14 Jun 2021 17:42:29 GMT  
		Size: 1.3 MB (1264529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29212836bbaacf27e155ad8002b1c2a6b5cd2dbe13986b27a57dc427357f2ce`  
		Last Modified: Mon, 14 Jun 2021 17:42:29 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:32914545de594aa79ff4231b61d5594f830641d124fb3cfa56e0575e940ec569
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2808449608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f1d0a4465ebc0bcefa7e5556bfb70eddabb69cf27ef61b558f45bef720fe883`
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
# Mon, 14 Jun 2021 18:21:36 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:21:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 18:22:12 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 14 Jun 2021 18:22:15 GMT
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
	-	`sha256:92f879ad577a7254271b2a27970912d5990740c6c23b65c14d3585b0b331b6b1`  
		Last Modified: Mon, 14 Jun 2021 18:26:07 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14bceb7d820e8f377e4a2d219ae96ee84dafd1055c85c1ce3deb22ea38cb8bf`  
		Last Modified: Mon, 14 Jun 2021 18:26:07 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ddb113a61bc728c0f730228bd4b782a04bcd9bec04ca60a8f46ca5b82e827a8`  
		Last Modified: Mon, 14 Jun 2021 18:26:08 GMT  
		Size: 1.7 MB (1730897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f05c3ba05a4dc7082b32ebd8dae3976fd8adb32927054b6fc0e3f137970df1`  
		Last Modified: Mon, 14 Jun 2021 18:26:07 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:3dc1e8d5170dfd5b5e6fbb34d885db2414827f33c49ca301aaaa82644bb7a6fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6437016101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:913b54138653e16a37ea51c2051dd30d0bc4ff76fece599b23b92c1aa7a11ff3`
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
# Mon, 14 Jun 2021 18:22:30 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:22:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 18:24:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 14 Jun 2021 18:24:02 GMT
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
	-	`sha256:3d01a14f10d204dac3535ad62c6b042cc9edc8c2c7c0996ecc45efbb896d5eed`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612bbd13a883cfddbf2977f7de24716a7978eea9f601ba5854f82d36f10068c4`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40a20ce35485bdd147339935426465c403bd3c52351030d040de662cec3253b`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.7 MB (1700121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a492d6062ee0783839f1bb22b289b12c884913a9018f1943add9b74a638df8f5`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:746c493872f8b672a3d07e35ca12032e8378587480dd245d512aacd2d23a9aa9
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
$ docker pull caddy@sha256:03ffe16fc60ddb7be4684d7c3c8e257038b2c00864c027415e8b05fc120c28d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.9 MB (116937549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d58d2ab3ddba126c2fd014ebdac7030a6d1c5eac1d0c5ea0ac1509d9c8c882d`
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
# Thu, 10 Jun 2021 21:26:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:26:40 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:26:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:26:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:26:42 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:19:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:19:01 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:19:48 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:19:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:19:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:19:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:19:50 GMT
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
	-	`sha256:e25adedf14febf43281fc3b4750e8b0c50f2bb061ef8f5e16a829d3392fa447b`  
		Last Modified: Thu, 10 Jun 2021 21:35:42 GMT  
		Size: 106.1 MB (106136761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52c85161d43b0fdd8bb3ae8fdf77b9e4fc783bceb11f591ed3bbdf1e4722abd`  
		Last Modified: Thu, 10 Jun 2021 21:35:26 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20d66408196d46dd8f1b9f81fb5afa2219f5ca4c68a313ca1c49d3b908f755d`  
		Last Modified: Thu, 10 Jun 2021 23:19:40 GMT  
		Size: 6.4 MB (6395665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84f14058db07dc0560a9f209a7d8768b4ebd80f1426006dec9fe3b4d7c7bd25`  
		Last Modified: Mon, 14 Jun 2021 17:20:29 GMT  
		Size: 1.3 MB (1311168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86b5f727a9d842c09b761d61887e9298328559147dd8e911eb7c5f6fcf5bfc2`  
		Last Modified: Mon, 14 Jun 2021 17:20:29 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:af84e4e4719a6f04129f95de4a1dadacacae55e4b82f98cc9f883020f40860da
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.7 MB (112708776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbae3456b30daef0a0988bb5200978e3a8b2981efecdd2f7a811c692ed7bcc6d`
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
# Thu, 10 Jun 2021 22:01:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 22:01:50 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 22:01:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 22:01:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 22:01:52 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:15:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:15:37 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:49:58 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:49:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:49:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:49:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:50:00 GMT
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
	-	`sha256:f6a122050eb4da5951b1c88f56bfe65cb0c1a50d4e9869ad63787a8d0fc9ff1e`  
		Last Modified: Thu, 10 Jun 2021 22:15:45 GMT  
		Size: 102.4 MB (102351924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc08c6e1815e1794433258a6a0a93785a234db42641d49902c4f194c1d6abc82`  
		Last Modified: Thu, 10 Jun 2021 22:15:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2e5491ca84af37b9bdc0dfcb0a65b798aea4ab080785e1bba16e36672accd4`  
		Last Modified: Thu, 10 Jun 2021 23:16:52 GMT  
		Size: 6.2 MB (6230941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cecdb7ddd0ec1710ae049c902367f06a18606501ca9d1dbe17ec00349029fb8`  
		Last Modified: Mon, 14 Jun 2021 17:51:16 GMT  
		Size: 1.2 MB (1221680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1729fe2ea9a0baa2a26bc61d595958dcecfcb3f577dcebaca53051ec502bf397`  
		Last Modified: Mon, 14 Jun 2021 17:51:16 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2a428d87d883958655e8d72e6461ed205031fac28d71b943746dda7178f2e555
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.6 MB (111602497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da4e596b14ba8264520d8c3f799a567c9b7f3847ae587434759e51d9c667bf76`
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
# Thu, 10 Jun 2021 22:35:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 22:35:30 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 22:35:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 22:35:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 22:35:32 GMT
WORKDIR /go
# Fri, 11 Jun 2021 00:34:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 11 Jun 2021 00:34:12 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:57:59 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:57:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:58:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:58:01 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:58:01 GMT
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
	-	`sha256:3e05d01ffccbffea159372f8065e42d62b484e73624dae1b567d908c12bb6fa3`  
		Last Modified: Thu, 10 Jun 2021 22:53:44 GMT  
		Size: 102.1 MB (102116599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9c0e093faea54528f8e070b0ad60f87674bf3a4654d312ccf7d110de2a6f6a`  
		Last Modified: Thu, 10 Jun 2021 22:53:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59aa8029ac012f4886ea6bced5e66e03743aff8bd41e8c7413cab0369c79c91b`  
		Last Modified: Fri, 11 Jun 2021 00:35:26 GMT  
		Size: 5.6 MB (5560992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a1e9ca701d6638943ef23a3969d9ba902fada02c041a3a797515d585882566`  
		Last Modified: Mon, 14 Jun 2021 17:59:18 GMT  
		Size: 1.2 MB (1219508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017f9bacdf7cdb13305fcaf052511ab74f9d9d2b9cbae1253957277cdb6cdd48`  
		Last Modified: Mon, 14 Jun 2021 17:59:17 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b0e22365417fa304ab483e3f2da3c7b79886ee3bced561c8113dd66b4e664fec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112151491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14b18c1aa44d74288d99db407cad68df0fb403a47cdad522a7524f856bb773f4`
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
# Thu, 10 Jun 2021 21:45:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:45:54 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:45:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:45:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:45:55 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:04:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:04:40 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:39:47 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:39:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:39:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:39:49 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:39:49 GMT
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
	-	`sha256:a9da95e357649360250671b270e39318d13b2ddff5d5aaac20081d588c9b6f74`  
		Last Modified: Thu, 10 Jun 2021 21:55:04 GMT  
		Size: 101.5 MB (101471730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a246c0d2a229c1d281fc3c1c9aa7fe651a820da43e66cd7ab7660e606d8d9824`  
		Last Modified: Thu, 10 Jun 2021 21:54:43 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2518188a669fe97c7d7feaf8a0ef8974bd167bc206832dc95bae562e6d972fe6`  
		Last Modified: Thu, 10 Jun 2021 23:05:37 GMT  
		Size: 6.5 MB (6483980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cb2ec8e0329ac1e5a6a5f1146f63479477cd73be5c2a0a676a12b3fda9485f`  
		Last Modified: Mon, 14 Jun 2021 17:40:46 GMT  
		Size: 1.2 MB (1201544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3538e34014117eaf3a7b09c03f2fcc11383c7bcebc701bcdfbf5a2a2a61906bb`  
		Last Modified: Mon, 14 Jun 2021 17:40:45 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:f8fc6696fb7cd73549cdc80e5889efd4c9ba480b9622ffe9f316c6e32b6068dc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (111016742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cbbf856cae07e092449ff2a67b42618d6082d532dec5969a4bfa5089b96b11c`
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
# Thu, 10 Jun 2021 21:27:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:27:48 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:27:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:28:04 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:28:11 GMT
WORKDIR /go
# Thu, 10 Jun 2021 23:16:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 23:16:36 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 18:20:23 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:20:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 18:20:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 18:20:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 18:20:58 GMT
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
	-	`sha256:c81f5fe451abbc39d3bdfca4378da5aa2c8b041d846b68db7b6004029734d919`  
		Last Modified: Thu, 10 Jun 2021 21:41:32 GMT  
		Size: 99.9 MB (99918197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9387c57f22b360d0c37409febd5288b34f77782689d3995e0092564a035eae10`  
		Last Modified: Thu, 10 Jun 2021 21:41:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af95f6a2bbd2f3bf752226a7020c5dcb4ba9e36df520e5b7dac8913f4f852d6e`  
		Last Modified: Thu, 10 Jun 2021 23:18:16 GMT  
		Size: 6.8 MB (6830748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994f06d8c6a86a071bc59b2d0644e6c4118c2a51d61edbf571623d36f9b1b987`  
		Last Modified: Mon, 14 Jun 2021 18:21:51 GMT  
		Size: 1.2 MB (1170526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54fa15ba38d0d74a3579bc4af43b527cc19bc368e7351ccaf85c90264bfc31c`  
		Last Modified: Mon, 14 Jun 2021 18:21:50 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:2d70ee7ce742b7eba9d3c4097f0ee5448f02a40e7cc10514c12bbd3272fa7448
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115888076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f08a6df8ec993ccbd835eee259d75804dc13b90f39ad9dccd7971136aecb356`
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
# Thu, 10 Jun 2021 21:52:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.5.src.tar.gz'; 	sha256='7bfa7e5908c7cc9e75da5ddf3066d7cbcf3fd9fa51945851325eebc17f50ba80'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		go install std; 		apk del --no-network .build-deps; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 10 Jun 2021 21:52:35 GMT
ENV GOPATH=/go
# Thu, 10 Jun 2021 21:52:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Jun 2021 21:52:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 10 Jun 2021 21:52:38 GMT
WORKDIR /go
# Thu, 10 Jun 2021 22:58:58 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 10 Jun 2021 22:58:59 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 14 Jun 2021 17:41:55 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:41:55 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 17:41:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Jun 2021 17:41:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Jun 2021 17:41:57 GMT
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
	-	`sha256:4b203e6fc30bb6c460e0aea06ed2a200569017655c2678db9ce6fed7a17762cc`  
		Last Modified: Thu, 10 Jun 2021 22:03:02 GMT  
		Size: 105.3 MB (105259453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9fa95d716a4e0cf3f1602cd1def2172371118109ba036c7d525ac506357a1b`  
		Last Modified: Thu, 10 Jun 2021 22:02:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1ceddc3358bec9a3e7284afbcb0a578916db67c3a60fbc269cf78c11f26623`  
		Last Modified: Thu, 10 Jun 2021 22:59:42 GMT  
		Size: 6.5 MB (6479018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab4e3358d5deaa72e1a9a5207c52a6f1133bd89e6c424bb9cf4f0b9fbf2e5b6`  
		Last Modified: Mon, 14 Jun 2021 17:42:29 GMT  
		Size: 1.3 MB (1264529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29212836bbaacf27e155ad8002b1c2a6b5cd2dbe13986b27a57dc427357f2ce`  
		Last Modified: Mon, 14 Jun 2021 17:42:29 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:6732f41f4155f39383864cbc74d3ac805ffda32377941904bfe0ee8d3516f679
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:32914545de594aa79ff4231b61d5594f830641d124fb3cfa56e0575e940ec569
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2808449608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f1d0a4465ebc0bcefa7e5556bfb70eddabb69cf27ef61b558f45bef720fe883`
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
# Mon, 14 Jun 2021 18:21:36 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:21:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 18:22:12 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 14 Jun 2021 18:22:15 GMT
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
	-	`sha256:92f879ad577a7254271b2a27970912d5990740c6c23b65c14d3585b0b331b6b1`  
		Last Modified: Mon, 14 Jun 2021 18:26:07 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14bceb7d820e8f377e4a2d219ae96ee84dafd1055c85c1ce3deb22ea38cb8bf`  
		Last Modified: Mon, 14 Jun 2021 18:26:07 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ddb113a61bc728c0f730228bd4b782a04bcd9bec04ca60a8f46ca5b82e827a8`  
		Last Modified: Mon, 14 Jun 2021 18:26:08 GMT  
		Size: 1.7 MB (1730897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f05c3ba05a4dc7082b32ebd8dae3976fd8adb32927054b6fc0e3f137970df1`  
		Last Modified: Mon, 14 Jun 2021 18:26:07 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:80f678464d89f88f808d926ddf79d5173f7367cc7c1e2381ecc3a7fb7307bb2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `caddy:builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:3dc1e8d5170dfd5b5e6fbb34d885db2414827f33c49ca301aaaa82644bb7a6fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6437016101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:913b54138653e16a37ea51c2051dd30d0bc4ff76fece599b23b92c1aa7a11ff3`
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
# Mon, 14 Jun 2021 18:22:30 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:22:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Jun 2021 18:24:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 14 Jun 2021 18:24:02 GMT
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
	-	`sha256:3d01a14f10d204dac3535ad62c6b042cc9edc8c2c7c0996ecc45efbb896d5eed`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612bbd13a883cfddbf2977f7de24716a7978eea9f601ba5854f82d36f10068c4`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40a20ce35485bdd147339935426465c403bd3c52351030d040de662cec3253b`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.7 MB (1700121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a492d6062ee0783839f1bb22b289b12c884913a9018f1943add9b74a638df8f5`  
		Last Modified: Mon, 14 Jun 2021 18:26:23 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:31493fd55da69e11db44f6acbd0c92070187cfd61dd0a5bfe17a0f6aa7b894d2
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
$ docker pull caddy@sha256:c3176ebaceec5d64a4892205d7cf3d32da87e2fcbbb8a47d787ef4200ef0e6d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14649179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57e953391a547aacb19ba079ee6713b24b8400352d6d95a8a43e79fb035ec0f7`
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
# Mon, 14 Jun 2021 17:19:37 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:19:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:19:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:19:41 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:19:41 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:19:41 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:19:41 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:19:41 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:19:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:19:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:19:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:19:43 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:19:43 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:19:43 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:19:44 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:19:44 GMT
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
	-	`sha256:037bdadcf837298422d86bb75d10aa9ea21eaaf0969e1d8e99b730b07208eb03`  
		Last Modified: Mon, 14 Jun 2021 17:20:16 GMT  
		Size: 11.5 MB (11530800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9785de7e5400398efa43aedd6416426c14e3101f52a5930b52b6e8ea3a0cd96`  
		Last Modified: Mon, 14 Jun 2021 17:20:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:53bc8c15c11306be1cd426dffb91df56e5dc186ae54c22eb08996f14c647378f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13817125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dd81d0e3a6035d5df068c9af8811281698921854e5190944b1f7a079651bb7d`
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
# Mon, 14 Jun 2021 17:49:40 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:49:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:49:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:49:44 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:49:44 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:49:44 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:49:44 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:49:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:49:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:49:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:49:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:49:46 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:49:46 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:49:47 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:49:47 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:49:47 GMT
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
	-	`sha256:028e0db410d042e12d6b3f64499cc00ae7298c02382ba1105cdc5ee03aaed549`  
		Last Modified: Mon, 14 Jun 2021 17:50:59 GMT  
		Size: 10.9 MB (10888459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64dbe91d32616efff4ec27f049638b231cfd0091a68480d45a21791d44b469c`  
		Last Modified: Mon, 14 Jun 2021 17:50:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:6fc967765fceab93d7838f17d2eeceddc56e21a65654e3ba92c799437ff09280
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13593827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d1b6dc4a59a634275f3c206036245997415a7d1894697b43d1dadc232712e8e`
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
# Mon, 14 Jun 2021 17:57:41 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:57:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:57:44 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:57:45 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:57:45 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:57:45 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:57:45 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:57:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:57:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:57:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:57:47 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:57:47 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:57:48 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:57:48 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:57:48 GMT
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
	-	`sha256:e97e805578bb88faf1e3b052fe899c9818d27e0e114574198d5e3d45a8faf1b9`  
		Last Modified: Mon, 14 Jun 2021 17:59:01 GMT  
		Size: 10.9 MB (10864008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee92873b0980eae80c33cd1bd74d1b35754b48c89cbe68088f4e98b4dd04e2f`  
		Last Modified: Mon, 14 Jun 2021 17:58:59 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:1f49cc95c1e8ebd7fe139595b64b8d3b2cbdafff4c46ff46bc4516054a50e3ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13466108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:749cdbfee8dde296c03efb611b07c067ca297771a1314bbcbbba992429e899e7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:32:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 15 Jun 2021 22:32:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 15 Jun 2021 22:32:20 GMT
ENV CADDY_VERSION=v2.4.2
# Tue, 15 Jun 2021 22:32:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 15 Jun 2021 22:32:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:32:23 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 15 Jun 2021 22:32:24 GMT
ENV XDG_DATA_HOME=/data
# Tue, 15 Jun 2021 22:32:24 GMT
VOLUME [/config]
# Tue, 15 Jun 2021 22:32:24 GMT
VOLUME [/data]
# Tue, 15 Jun 2021 22:32:24 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Tue, 15 Jun 2021 22:32:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 15 Jun 2021 22:32:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 15 Jun 2021 22:32:26 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 15 Jun 2021 22:32:26 GMT
EXPOSE 80
# Tue, 15 Jun 2021 22:32:26 GMT
EXPOSE 443
# Tue, 15 Jun 2021 22:32:26 GMT
EXPOSE 2019
# Tue, 15 Jun 2021 22:32:26 GMT
WORKDIR /srv
# Tue, 15 Jun 2021 22:32:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d0b72044755ebd2b829600b94a69aa9096bbb4bf9a01c1795b5b245261b99a`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 300.6 KB (300631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abde659ccf1d73128ef1e71a9701b014e0f27d4abf15b3d410d0474cdd0adb95`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0b93549f9104a9bb517f1ae15bd6ef4d44f83d21964728c50aa960b97098dc`  
		Last Modified: Tue, 15 Jun 2021 22:33:26 GMT  
		Size: 10.4 MB (10447450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69a851000e14247059ab07104ab76f86231aaa1a4fb5abb6b321e66a45003d3`  
		Last Modified: Tue, 15 Jun 2021 22:33:24 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:7764cdcd665f8e23165bf385240e8951ab046dd6f54808b247b57e284882ecc5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13175121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c3b2d52d66b7076e6c98e715324384114a94b978294b836f566919d77faa909`
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
# Mon, 14 Jun 2021 18:16:57 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:17:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 18:17:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 18:17:56 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 18:18:00 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 18:18:08 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 18:18:15 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 18:18:26 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:18:36 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:18:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:18:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:18:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:19:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:19:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:19:27 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:19:32 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:19:38 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:19:43 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:19:49 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 18:19:56 GMT
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
	-	`sha256:d23e936288e88eac2d5280068486ab71f9023047b51d2c012a09fd305cc70e19`  
		Last Modified: Mon, 14 Jun 2021 18:21:33 GMT  
		Size: 10.1 MB (10053418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59596542df0c41e54f99fa862419a9f75ef8cfce5b1788110d747951a295518e`  
		Last Modified: Mon, 14 Jun 2021 18:21:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:c8d5cda3a4ef8a3fae917a732cd349372b1cc625071f9b3acc77a9033eb55e63
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14004446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5539a479891dabbacf899df4a9c0af209caf5e8b82799b452efd5c9093bd99`
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
# Mon, 14 Jun 2021 17:41:42 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 17:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9d3320f829cfd26945ed417bc4cb52f79691db6dce52ebc8721d25c85a857888ae8db10ba500e1098aee92dc44a9d5fbe342b419d0736f525712746f884cf1ff' ;; 		armhf)   binArch='armv6'; checksum='72d9ac31519dafed67284671d3ed9d401807017d143b42bbdaaeba709123ead0f8082cc5223539622a0493fbbefb25f03c4a28c544ef1d5a02b5d8fcb36101de' ;; 		armv7)   binArch='armv7'; checksum='65d6d093a27e9699de35e436d5880f7c19287988cbb60429d979ffc0dc5855c0fa778879d9dffd3e6bb5e6efb3979f53d4e3466c9ec7e36c695cf938452e9dd9' ;; 		aarch64) binArch='arm64'; checksum='2d51dc9c49d10846f8925a0185388b3a539cebba86d80a3b838d9e85e35d80d1786a8f2e519c94f10df4f763bcf0ef3127ae9fe00d940c8a5cda8405445b68a5' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='df0c60f66f25441f3e4f2db0e5565fd632730e3d48ee0ecb2a5da763bde957b5774e085a623409d54b06ff0d0197f38ec2ac11d3642b58cce3eed3360b4de99a' ;; 		s390x)   binArch='s390x'; checksum='4b9ad777d515fe3ed79ba57f76e4443e95148c8b991b5e00ee04088ad0a0ad88d8e951d56b8001f9ded3c0ef29f674a1b5eaccc2a1f80121bd177aa7764e9245' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Jun 2021 17:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:41:46 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Jun 2021 17:41:46 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Jun 2021 17:41:46 GMT
VOLUME [/config]
# Mon, 14 Jun 2021 17:41:47 GMT
VOLUME [/data]
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 17:41:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 17:41:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 17:41:49 GMT
EXPOSE 80
# Mon, 14 Jun 2021 17:41:49 GMT
EXPOSE 443
# Mon, 14 Jun 2021 17:41:49 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 17:41:49 GMT
WORKDIR /srv
# Mon, 14 Jun 2021 17:41:50 GMT
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
	-	`sha256:9b59880ffc79bf424b9fb38c497ec3d3edea77c4cbabb6b295bad830e4732008`  
		Last Modified: Mon, 14 Jun 2021 17:42:22 GMT  
		Size: 11.1 MB (11094948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4a0a3f3a72f3127538116c7943809378ae5921f09f19249fb98a578d261a49`  
		Last Modified: Mon, 14 Jun 2021 17:42:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:84c41546a31938e07bc74b9535459f62221b5fa62f50aadb3f7138ceb0a638b7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2654297157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7933e1b45a92be68914695f31f1c84c86b602c5233536557c1ccee877d1216b0`
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
# Mon, 14 Jun 2021 18:15:56 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:16:40 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8d5cf4479e471d47fd067ce2fbe34c2015a96caedab95ca042aeb633956cbc2bb89c1bc4fe6593c1f96ca58bc66b21f32caa6b099122b9d500a3902245fa5105')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 14 Jun 2021 18:16:43 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 14 Jun 2021 18:16:45 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 14 Jun 2021 18:16:48 GMT
VOLUME [c:/config]
# Mon, 14 Jun 2021 18:16:50 GMT
VOLUME [c:/data]
# Mon, 14 Jun 2021 18:16:53 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:16:55 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:16:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:17:01 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:17:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:17:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:17:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:17:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:17:15 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:17:17 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:17:20 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:17:39 GMT
RUN caddy version
# Mon, 14 Jun 2021 18:17:41 GMT
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
	-	`sha256:07802e3c606e3b9298421527979a2b9797c286d601553a4f8c11271d67919b58`  
		Last Modified: Mon, 14 Jun 2021 18:25:04 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4847967ab228abb45531c45132179ebac7d55ea85bf85ea3f3f420aff0be2863`  
		Last Modified: Mon, 14 Jun 2021 18:25:17 GMT  
		Size: 12.0 MB (12025127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e590a115b7ca0fdadc5a634f9a3b1a58db5ac8a89765f1d00351421045e7dd62`  
		Last Modified: Mon, 14 Jun 2021 18:25:03 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a698c5067c38c742726c5f427f5f07d028e7768a91c4f2fd9a973f662a750b0`  
		Last Modified: Mon, 14 Jun 2021 18:25:03 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4d9bb89edb4e6f90cfacbb81068b117b3b8affe4430a23ddc2f8aa8b1803fa`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369f1dad8944bfe55423327ebaedf96f73e356ca6fd92d4e9a8d2fdbc6b6293c`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f126fec1b223ee19a7f02455cd95a68d8275a8589273ff50b9f7ffbad72a882`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3949035d30e3b80897ac6fc2b4776dccd30680886816cfe8c27ed8bc8c0c595`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c1d9637c1841b64adc5cccf8a5ce5275754886c8c7eb26005eef69727bc101`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa902629ee85278422f20ba99ecc504972ce7c6263bdfa5f1d0a51103ed3e272`  
		Last Modified: Mon, 14 Jun 2021 18:24:59 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7795b0b452df39f057bb8fb233e6862dba05177f3c225da1443588e4e7ec3326`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b936a424e3378bda5aaa142367741f0486702c00117d08a527d36f3876cc7a0`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74ede6be2a18e8c915b5e55628de5a029cf0bb5b69edc917dd8f1c6e1426ee6`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cdf00e847ddd24f1ba768e20fd224aa86a161461a82d3a210f1d5ce1f28cb2`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51405f73ce954be2e339c2cfa1a28109cd371d9fb8986047079a8ba8cc4a9d7a`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38f74dca7b51152c809bf35c007d8affbfc36cae366903110509bdba8f3bde6`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca41d82a7c33c949c331f1ff7958f3ec1551f1bda90faaf07d7b112111a251bc`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582046a83a61d6a9e5701d72c1102b19e9e9ba65665c38d03618e34acdaa5c36`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 300.2 KB (300242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a16f8caea000f3748f024fd14e1419c77091e71e4c220b06a94dc02ffc746c`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:4d5c4f12af6b434f907c262accbfeef1c9eb948d91bb5113bde117904152d9bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278396558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b0d047c64024dd8b9ee7374a59e2e19a219277308f3db92d25f22e903b4f6fb`
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
# Mon, 14 Jun 2021 18:17:52 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:19:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8d5cf4479e471d47fd067ce2fbe34c2015a96caedab95ca042aeb633956cbc2bb89c1bc4fe6593c1f96ca58bc66b21f32caa6b099122b9d500a3902245fa5105')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 14 Jun 2021 18:19:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 14 Jun 2021 18:19:41 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 14 Jun 2021 18:19:43 GMT
VOLUME [c:/config]
# Mon, 14 Jun 2021 18:19:46 GMT
VOLUME [c:/data]
# Mon, 14 Jun 2021 18:19:48 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:19:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:19:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:19:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:19:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:20:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:20:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:20:04 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:20:07 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:20:09 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:20:11 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:21:14 GMT
RUN caddy version
# Mon, 14 Jun 2021 18:21:17 GMT
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
	-	`sha256:5bd5fde0219b866984e02c69748a7c533734e7d3ce1c605e00b2794ba719ca78`  
		Last Modified: Mon, 14 Jun 2021 18:25:40 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ff67696fba822eac7dc90ce8b74a3463e180c1277ce1b5235dd553efd54d37`  
		Last Modified: Mon, 14 Jun 2021 18:25:53 GMT  
		Size: 12.0 MB (12011979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb05b150667473f58bd9ff97143e7addb941c15c23d7c0190462052e171a5d3`  
		Last Modified: Mon, 14 Jun 2021 18:25:40 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417ec686bccf8c11c7e167450f76c56e965e0d895b8a67d2959fa0cd8e0f46c6`  
		Last Modified: Mon, 14 Jun 2021 18:25:39 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e7f7e817f7b000e684b2477e658283e3bc5e32f705e2a1af3eb2171451ab1a`  
		Last Modified: Mon, 14 Jun 2021 18:25:38 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9adbfef5bd1c4ce567e8643e7eb3ac228fc89e60afffa0d4ad65188836ee10e`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46951e23f2c6f042a74af530655917c470e7e58bd428811bea889f06ece060f3`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b702d713b07cb19c098b0a4c2ad22de8111ab140c99b88deb21ffa5f10870f`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1554c780202a1e2bfb6cafbf73148847f97c535c407f63f750903997105d516f`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a72ab2ef98ce84364537328634d5a56cb6c9080cdec9988778c0e15d451dc51`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0cb0fb150ef4d4bb3e78339539c6453dcdf1d1b11d50728bb72e262b603fa9`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d8666b345f227a53b8d4cc8698ebe05b454caf116f8329e30d4328ba56896e`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bce3d7ad9504e8b1a2a5f46b50605a7e895686efeae62529b2fb0c8210a2e7`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d806bd36723a790387c5f61446d9b73da291b1e1592e6943b28686f3dc50fb39`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddf127d6e3c5443190a309b2f703cfd1d079beea71723b1507958dbbf2b5cab`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace91f2d94fe0fd5d53fce078d832db72cc38e2ef7692a44f57f9377dcbf3f8f`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f8adfaab4745797ca3869f6e54a87e5c399e56609635f7b74b039fb8f9fc00`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca3d4ed717fc9e7154ad94da8a5ea30b61ba4dfe9ec25bdcfcb55e6291cbec7`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 274.6 KB (274630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deafc6c05519d23d4709cd8504c83ff6c43943477ddcaf57ae7a871acdbdf489`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:6b1a7e2d64eea0fda092326bf2660a9f57caa3d9e0679b9b2916458ae71a2880
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:84c41546a31938e07bc74b9535459f62221b5fa62f50aadb3f7138ceb0a638b7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2654297157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7933e1b45a92be68914695f31f1c84c86b602c5233536557c1ccee877d1216b0`
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
# Mon, 14 Jun 2021 18:15:56 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:16:40 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8d5cf4479e471d47fd067ce2fbe34c2015a96caedab95ca042aeb633956cbc2bb89c1bc4fe6593c1f96ca58bc66b21f32caa6b099122b9d500a3902245fa5105')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 14 Jun 2021 18:16:43 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 14 Jun 2021 18:16:45 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 14 Jun 2021 18:16:48 GMT
VOLUME [c:/config]
# Mon, 14 Jun 2021 18:16:50 GMT
VOLUME [c:/data]
# Mon, 14 Jun 2021 18:16:53 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:16:55 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:16:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:17:01 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:17:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:17:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:17:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:17:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:17:15 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:17:17 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:17:20 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:17:39 GMT
RUN caddy version
# Mon, 14 Jun 2021 18:17:41 GMT
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
	-	`sha256:07802e3c606e3b9298421527979a2b9797c286d601553a4f8c11271d67919b58`  
		Last Modified: Mon, 14 Jun 2021 18:25:04 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4847967ab228abb45531c45132179ebac7d55ea85bf85ea3f3f420aff0be2863`  
		Last Modified: Mon, 14 Jun 2021 18:25:17 GMT  
		Size: 12.0 MB (12025127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e590a115b7ca0fdadc5a634f9a3b1a58db5ac8a89765f1d00351421045e7dd62`  
		Last Modified: Mon, 14 Jun 2021 18:25:03 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a698c5067c38c742726c5f427f5f07d028e7768a91c4f2fd9a973f662a750b0`  
		Last Modified: Mon, 14 Jun 2021 18:25:03 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4d9bb89edb4e6f90cfacbb81068b117b3b8affe4430a23ddc2f8aa8b1803fa`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369f1dad8944bfe55423327ebaedf96f73e356ca6fd92d4e9a8d2fdbc6b6293c`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f126fec1b223ee19a7f02455cd95a68d8275a8589273ff50b9f7ffbad72a882`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3949035d30e3b80897ac6fc2b4776dccd30680886816cfe8c27ed8bc8c0c595`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c1d9637c1841b64adc5cccf8a5ce5275754886c8c7eb26005eef69727bc101`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa902629ee85278422f20ba99ecc504972ce7c6263bdfa5f1d0a51103ed3e272`  
		Last Modified: Mon, 14 Jun 2021 18:24:59 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7795b0b452df39f057bb8fb233e6862dba05177f3c225da1443588e4e7ec3326`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b936a424e3378bda5aaa142367741f0486702c00117d08a527d36f3876cc7a0`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74ede6be2a18e8c915b5e55628de5a029cf0bb5b69edc917dd8f1c6e1426ee6`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cdf00e847ddd24f1ba768e20fd224aa86a161461a82d3a210f1d5ce1f28cb2`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51405f73ce954be2e339c2cfa1a28109cd371d9fb8986047079a8ba8cc4a9d7a`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38f74dca7b51152c809bf35c007d8affbfc36cae366903110509bdba8f3bde6`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca41d82a7c33c949c331f1ff7958f3ec1551f1bda90faaf07d7b112111a251bc`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582046a83a61d6a9e5701d72c1102b19e9e9ba65665c38d03618e34acdaa5c36`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 300.2 KB (300242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a16f8caea000f3748f024fd14e1419c77091e71e4c220b06a94dc02ffc746c`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:4d5c4f12af6b434f907c262accbfeef1c9eb948d91bb5113bde117904152d9bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278396558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b0d047c64024dd8b9ee7374a59e2e19a219277308f3db92d25f22e903b4f6fb`
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
# Mon, 14 Jun 2021 18:17:52 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:19:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8d5cf4479e471d47fd067ce2fbe34c2015a96caedab95ca042aeb633956cbc2bb89c1bc4fe6593c1f96ca58bc66b21f32caa6b099122b9d500a3902245fa5105')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 14 Jun 2021 18:19:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 14 Jun 2021 18:19:41 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 14 Jun 2021 18:19:43 GMT
VOLUME [c:/config]
# Mon, 14 Jun 2021 18:19:46 GMT
VOLUME [c:/data]
# Mon, 14 Jun 2021 18:19:48 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:19:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:19:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:19:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:19:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:20:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:20:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:20:04 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:20:07 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:20:09 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:20:11 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:21:14 GMT
RUN caddy version
# Mon, 14 Jun 2021 18:21:17 GMT
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
	-	`sha256:5bd5fde0219b866984e02c69748a7c533734e7d3ce1c605e00b2794ba719ca78`  
		Last Modified: Mon, 14 Jun 2021 18:25:40 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ff67696fba822eac7dc90ce8b74a3463e180c1277ce1b5235dd553efd54d37`  
		Last Modified: Mon, 14 Jun 2021 18:25:53 GMT  
		Size: 12.0 MB (12011979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb05b150667473f58bd9ff97143e7addb941c15c23d7c0190462052e171a5d3`  
		Last Modified: Mon, 14 Jun 2021 18:25:40 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417ec686bccf8c11c7e167450f76c56e965e0d895b8a67d2959fa0cd8e0f46c6`  
		Last Modified: Mon, 14 Jun 2021 18:25:39 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e7f7e817f7b000e684b2477e658283e3bc5e32f705e2a1af3eb2171451ab1a`  
		Last Modified: Mon, 14 Jun 2021 18:25:38 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9adbfef5bd1c4ce567e8643e7eb3ac228fc89e60afffa0d4ad65188836ee10e`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46951e23f2c6f042a74af530655917c470e7e58bd428811bea889f06ece060f3`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b702d713b07cb19c098b0a4c2ad22de8111ab140c99b88deb21ffa5f10870f`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1554c780202a1e2bfb6cafbf73148847f97c535c407f63f750903997105d516f`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a72ab2ef98ce84364537328634d5a56cb6c9080cdec9988778c0e15d451dc51`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0cb0fb150ef4d4bb3e78339539c6453dcdf1d1b11d50728bb72e262b603fa9`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d8666b345f227a53b8d4cc8698ebe05b454caf116f8329e30d4328ba56896e`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bce3d7ad9504e8b1a2a5f46b50605a7e895686efeae62529b2fb0c8210a2e7`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d806bd36723a790387c5f61446d9b73da291b1e1592e6943b28686f3dc50fb39`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddf127d6e3c5443190a309b2f703cfd1d079beea71723b1507958dbbf2b5cab`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace91f2d94fe0fd5d53fce078d832db72cc38e2ef7692a44f57f9377dcbf3f8f`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f8adfaab4745797ca3869f6e54a87e5c399e56609635f7b74b039fb8f9fc00`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca3d4ed717fc9e7154ad94da8a5ea30b61ba4dfe9ec25bdcfcb55e6291cbec7`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 274.6 KB (274630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deafc6c05519d23d4709cd8504c83ff6c43943477ddcaf57ae7a871acdbdf489`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:1791c7844819a24a2bae3a297d7e61abe6b39e642e60743a94def9537939148a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull caddy@sha256:84c41546a31938e07bc74b9535459f62221b5fa62f50aadb3f7138ceb0a638b7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2654297157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7933e1b45a92be68914695f31f1c84c86b602c5233536557c1ccee877d1216b0`
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
# Mon, 14 Jun 2021 18:15:56 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:16:40 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8d5cf4479e471d47fd067ce2fbe34c2015a96caedab95ca042aeb633956cbc2bb89c1bc4fe6593c1f96ca58bc66b21f32caa6b099122b9d500a3902245fa5105')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 14 Jun 2021 18:16:43 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 14 Jun 2021 18:16:45 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 14 Jun 2021 18:16:48 GMT
VOLUME [c:/config]
# Mon, 14 Jun 2021 18:16:50 GMT
VOLUME [c:/data]
# Mon, 14 Jun 2021 18:16:53 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:16:55 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:16:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:17:01 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:17:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:17:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:17:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:17:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:17:15 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:17:17 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:17:20 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:17:39 GMT
RUN caddy version
# Mon, 14 Jun 2021 18:17:41 GMT
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
	-	`sha256:07802e3c606e3b9298421527979a2b9797c286d601553a4f8c11271d67919b58`  
		Last Modified: Mon, 14 Jun 2021 18:25:04 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4847967ab228abb45531c45132179ebac7d55ea85bf85ea3f3f420aff0be2863`  
		Last Modified: Mon, 14 Jun 2021 18:25:17 GMT  
		Size: 12.0 MB (12025127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e590a115b7ca0fdadc5a634f9a3b1a58db5ac8a89765f1d00351421045e7dd62`  
		Last Modified: Mon, 14 Jun 2021 18:25:03 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a698c5067c38c742726c5f427f5f07d028e7768a91c4f2fd9a973f662a750b0`  
		Last Modified: Mon, 14 Jun 2021 18:25:03 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4d9bb89edb4e6f90cfacbb81068b117b3b8affe4430a23ddc2f8aa8b1803fa`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369f1dad8944bfe55423327ebaedf96f73e356ca6fd92d4e9a8d2fdbc6b6293c`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f126fec1b223ee19a7f02455cd95a68d8275a8589273ff50b9f7ffbad72a882`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3949035d30e3b80897ac6fc2b4776dccd30680886816cfe8c27ed8bc8c0c595`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c1d9637c1841b64adc5cccf8a5ce5275754886c8c7eb26005eef69727bc101`  
		Last Modified: Mon, 14 Jun 2021 18:25:01 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa902629ee85278422f20ba99ecc504972ce7c6263bdfa5f1d0a51103ed3e272`  
		Last Modified: Mon, 14 Jun 2021 18:24:59 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7795b0b452df39f057bb8fb233e6862dba05177f3c225da1443588e4e7ec3326`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b936a424e3378bda5aaa142367741f0486702c00117d08a527d36f3876cc7a0`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74ede6be2a18e8c915b5e55628de5a029cf0bb5b69edc917dd8f1c6e1426ee6`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cdf00e847ddd24f1ba768e20fd224aa86a161461a82d3a210f1d5ce1f28cb2`  
		Last Modified: Mon, 14 Jun 2021 18:24:58 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51405f73ce954be2e339c2cfa1a28109cd371d9fb8986047079a8ba8cc4a9d7a`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38f74dca7b51152c809bf35c007d8affbfc36cae366903110509bdba8f3bde6`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca41d82a7c33c949c331f1ff7958f3ec1551f1bda90faaf07d7b112111a251bc`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582046a83a61d6a9e5701d72c1102b19e9e9ba65665c38d03618e34acdaa5c36`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 300.2 KB (300242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a16f8caea000f3748f024fd14e1419c77091e71e4c220b06a94dc02ffc746c`  
		Last Modified: Mon, 14 Jun 2021 18:24:56 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:076e0573f1533c025ab55f299e32833e09ed22b4c52605a2351aba5baa2f585d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:4d5c4f12af6b434f907c262accbfeef1c9eb948d91bb5113bde117904152d9bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278396558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b0d047c64024dd8b9ee7374a59e2e19a219277308f3db92d25f22e903b4f6fb`
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
# Mon, 14 Jun 2021 18:17:52 GMT
ENV CADDY_VERSION=v2.4.2
# Mon, 14 Jun 2021 18:19:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.2/caddy_2.4.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8d5cf4479e471d47fd067ce2fbe34c2015a96caedab95ca042aeb633956cbc2bb89c1bc4fe6593c1f96ca58bc66b21f32caa6b099122b9d500a3902245fa5105')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 14 Jun 2021 18:19:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 14 Jun 2021 18:19:41 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 14 Jun 2021 18:19:43 GMT
VOLUME [c:/config]
# Mon, 14 Jun 2021 18:19:46 GMT
VOLUME [c:/data]
# Mon, 14 Jun 2021 18:19:48 GMT
LABEL org.opencontainers.image.version=v2.4.2
# Mon, 14 Jun 2021 18:19:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Jun 2021 18:19:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Jun 2021 18:19:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Jun 2021 18:19:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Jun 2021 18:20:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Jun 2021 18:20:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Jun 2021 18:20:04 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Jun 2021 18:20:07 GMT
EXPOSE 80
# Mon, 14 Jun 2021 18:20:09 GMT
EXPOSE 443
# Mon, 14 Jun 2021 18:20:11 GMT
EXPOSE 2019
# Mon, 14 Jun 2021 18:21:14 GMT
RUN caddy version
# Mon, 14 Jun 2021 18:21:17 GMT
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
	-	`sha256:5bd5fde0219b866984e02c69748a7c533734e7d3ce1c605e00b2794ba719ca78`  
		Last Modified: Mon, 14 Jun 2021 18:25:40 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ff67696fba822eac7dc90ce8b74a3463e180c1277ce1b5235dd553efd54d37`  
		Last Modified: Mon, 14 Jun 2021 18:25:53 GMT  
		Size: 12.0 MB (12011979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb05b150667473f58bd9ff97143e7addb941c15c23d7c0190462052e171a5d3`  
		Last Modified: Mon, 14 Jun 2021 18:25:40 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417ec686bccf8c11c7e167450f76c56e965e0d895b8a67d2959fa0cd8e0f46c6`  
		Last Modified: Mon, 14 Jun 2021 18:25:39 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e7f7e817f7b000e684b2477e658283e3bc5e32f705e2a1af3eb2171451ab1a`  
		Last Modified: Mon, 14 Jun 2021 18:25:38 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9adbfef5bd1c4ce567e8643e7eb3ac228fc89e60afffa0d4ad65188836ee10e`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46951e23f2c6f042a74af530655917c470e7e58bd428811bea889f06ece060f3`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b702d713b07cb19c098b0a4c2ad22de8111ab140c99b88deb21ffa5f10870f`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1554c780202a1e2bfb6cafbf73148847f97c535c407f63f750903997105d516f`  
		Last Modified: Mon, 14 Jun 2021 18:25:37 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a72ab2ef98ce84364537328634d5a56cb6c9080cdec9988778c0e15d451dc51`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0cb0fb150ef4d4bb3e78339539c6453dcdf1d1b11d50728bb72e262b603fa9`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d8666b345f227a53b8d4cc8698ebe05b454caf116f8329e30d4328ba56896e`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bce3d7ad9504e8b1a2a5f46b50605a7e895686efeae62529b2fb0c8210a2e7`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d806bd36723a790387c5f61446d9b73da291b1e1592e6943b28686f3dc50fb39`  
		Last Modified: Mon, 14 Jun 2021 18:25:35 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddf127d6e3c5443190a309b2f703cfd1d079beea71723b1507958dbbf2b5cab`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace91f2d94fe0fd5d53fce078d832db72cc38e2ef7692a44f57f9377dcbf3f8f`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f8adfaab4745797ca3869f6e54a87e5c399e56609635f7b74b039fb8f9fc00`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca3d4ed717fc9e7154ad94da8a5ea30b61ba4dfe9ec25bdcfcb55e6291cbec7`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 274.6 KB (274630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deafc6c05519d23d4709cd8504c83ff6c43943477ddcaf57ae7a871acdbdf489`  
		Last Modified: Mon, 14 Jun 2021 18:25:32 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
