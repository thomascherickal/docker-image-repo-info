<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `caddy`

-	[`caddy:2`](#caddy2)
-	[`caddy:2.0.0`](#caddy200)
-	[`caddy:2.0.0-alpine`](#caddy200-alpine)
-	[`caddy:2.0.0-builder`](#caddy200-builder)
-	[`caddy:2.0.0-windowsservercore`](#caddy200-windowsservercore)
-	[`caddy:2.0.0-windowsservercore-1809`](#caddy200-windowsservercore-1809)
-	[`caddy:2.0.0-windowsservercore-ltsc2016`](#caddy200-windowsservercore-ltsc2016)
-	[`caddy:2.1.0-beta.1`](#caddy210-beta1)
-	[`caddy:2.1.0-beta.1-alpine`](#caddy210-beta1-alpine)
-	[`caddy:2.1.0-beta.1-builder`](#caddy210-beta1-builder)
-	[`caddy:2.1.0-beta.1-windowsservercore`](#caddy210-beta1-windowsservercore)
-	[`caddy:2.1.0-beta.1-windowsservercore-1809`](#caddy210-beta1-windowsservercore-1809)
-	[`caddy:2.1.0-beta.1-windowsservercore-ltsc2016`](#caddy210-beta1-windowsservercore-ltsc2016)
-	[`caddy:2-alpine`](#caddy2-alpine)
-	[`caddy:2-builder`](#caddy2-builder)
-	[`caddy:2-windowsservercore`](#caddy2-windowsservercore)
-	[`caddy:2-windowsservercore-1809`](#caddy2-windowsservercore-1809)
-	[`caddy:2-windowsservercore-ltsc2016`](#caddy2-windowsservercore-ltsc2016)
-	[`caddy:alpine`](#caddyalpine)
-	[`caddy:builder`](#caddybuilder)
-	[`caddy:latest`](#caddylatest)
-	[`caddy:windowsservercore`](#caddywindowsservercore)
-	[`caddy:windowsservercore-1809`](#caddywindowsservercore-1809)
-	[`caddy:windowsservercore-ltsc2016`](#caddywindowsservercore-ltsc2016)

## `caddy:2`

```console
$ docker pull caddy@sha256:906e32bdd357959838cd20f8a5fdb487afe307542c31b0269d9cb5c3731d0ca5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1282; amd64
	-	windows version 10.0.14393.3750; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:262f58e0836d0be11253e500e3b32e78e6d6149a90ed54e4a4ed5ca736e844fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15145372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:313ad00e425a86a5b5f39170ac018ada5d833fae55ab101712e80f52b4b986de`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 13:39:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 24 Apr 2020 13:39:03 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Fri, 24 Apr 2020 13:39:05 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 19:20:49 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 16:21:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:19:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:19:44 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:19:44 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:19:44 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:19:44 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:19:44 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:19:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:19:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:19:46 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:19:46 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:19:46 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:19:47 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:19:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c92d2df695a8e1549e487fe6691311b8c3ccfdd90383c6ae37c578c4465c76`  
		Last Modified: Fri, 24 Apr 2020 13:39:22 GMT  
		Size: 318.6 KB (318554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d779d752c63b3ccba5c5fbec57ae2361cef2059d83ea0770f389f1d9849ccde`  
		Last Modified: Fri, 24 Apr 2020 13:39:22 GMT  
		Size: 5.8 KB (5765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e321d52b548add190f8f5974453da203fc605ed33865ced7b83cc1e8fddc904e`  
		Last Modified: Wed, 06 May 2020 16:21:33 GMT  
		Size: 12.0 MB (12007584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c780a87c731befe76e920c134aaa9d393de1437f0c3940f40b355bc61de8f7a6`  
		Last Modified: Fri, 26 Jun 2020 01:20:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e304abe5082419b9f5b33d893544fd83a96932dcb7e064f871bee67716222091
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.4 MB (14390760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76f2894818f3ff916764fc8e6f3111c24629f11662bd03135b07492053d9dc86`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:42:29 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 23 Apr 2020 17:42:31 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Thu, 23 Apr 2020 17:42:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 18:49:25 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:49:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 00:50:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 00:50:46 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 00:50:47 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 00:50:47 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 00:50:48 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 00:50:49 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 00:50:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 00:50:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 00:50:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 00:50:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 00:50:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 00:50:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 00:50:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 00:50:55 GMT
EXPOSE 80
# Fri, 26 Jun 2020 00:50:56 GMT
EXPOSE 443
# Fri, 26 Jun 2020 00:50:57 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 00:50:58 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 00:50:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4aecf4b3c455b15219e7ae2914078c1796d34e6b1c2916aab2fa79d0aecc97`  
		Last Modified: Thu, 23 Apr 2020 17:43:07 GMT  
		Size: 318.9 KB (318932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78f3e6c459120cfcfb844a46e1d5fa39f425743ad39e3265fdb6b4c4ea312b6`  
		Last Modified: Thu, 23 Apr 2020 17:43:07 GMT  
		Size: 5.8 KB (5842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6977aa451d29e02cfa0a60ee52aadf3bfa7fad7712ac1687007cbb0bd812f996`  
		Last Modified: Wed, 06 May 2020 15:50:14 GMT  
		Size: 11.4 MB (11445896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2e1a3cae97c62afbdf067d2b1201f2e96a4ae8bb2320a3883f82fd1aec2824`  
		Last Modified: Fri, 26 Jun 2020 00:51:21 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2653b633a6ecc87fdf8ab9941be387a42f25f1c17580878c9cd47055a726d734
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14164711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87f56b16af8dc7e3d49ffb1018e82def382e00da18d024561d9c1fbc0a392938`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 23:22:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 23 Apr 2020 23:22:58 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Thu, 23 Apr 2020 23:23:03 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 18:57:29 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:57:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 00:59:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 00:59:31 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 00:59:31 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 00:59:32 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 00:59:32 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 00:59:33 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 00:59:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 00:59:34 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 00:59:35 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 00:59:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 00:59:36 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 00:59:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 00:59:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 00:59:39 GMT
EXPOSE 80
# Fri, 26 Jun 2020 00:59:39 GMT
EXPOSE 443
# Fri, 26 Jun 2020 00:59:40 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 00:59:41 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 00:59:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf760b044fed05d609c6cc0dbc0163d673af839c2bd8b93be46a9dd9b3235d8d`  
		Last Modified: Thu, 23 Apr 2020 23:23:51 GMT  
		Size: 317.9 KB (317871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702db93291bb8c691008d86b00d866d87fd9904461e56e447408436f67069d12`  
		Last Modified: Thu, 23 Apr 2020 23:23:50 GMT  
		Size: 5.8 KB (5843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a240b5e189e2da028c9e14c55e560dda7eebabe89a0fdc68bd063df8ac5403`  
		Last Modified: Wed, 06 May 2020 15:58:14 GMT  
		Size: 11.4 MB (11418780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febb3ae65834fee908dad31bb9b1fe5dbffd24c31bd7b4d6eb3f7e0cc0be6524`  
		Last Modified: Fri, 26 Jun 2020 01:00:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:d9aef3ac6d0885fa20fd11f612c78377e9b9e12bca0d92e77205e7c90e65d07c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14099502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d385c1b96da99f80af54a8b12302cb050f0b91d661b1d5d3c876b6ae33003cfc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 03:41:26 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 24 Apr 2020 03:41:27 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Fri, 24 Apr 2020 03:41:30 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 18:39:39 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 16:39:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:40:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:40:07 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:40:08 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:40:09 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:40:09 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:40:10 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:40:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:40:11 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:40:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:40:13 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:40:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:40:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:40:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:40:16 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:40:16 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:40:17 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:40:18 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:40:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1dd90474a5634d83eea66237a34342ba1aa7b9660127d7a6168f9dd16a6800`  
		Last Modified: Fri, 24 Apr 2020 03:42:02 GMT  
		Size: 319.1 KB (319109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523ce157ee2040adfd1d897f97c884c8df6de54df4581f3982d4114fea063843`  
		Last Modified: Fri, 24 Apr 2020 03:42:02 GMT  
		Size: 5.8 KB (5843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45586f3cd2c78aa4e4ec308b720449bd298ff8184489fc23ed1b63329d5bfba`  
		Last Modified: Wed, 06 May 2020 16:40:28 GMT  
		Size: 11.0 MB (11049973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f00aaba3fbdd96271be17e7a6a5b181a398f7c2f05bc510c8fb471d69578081`  
		Last Modified: Fri, 26 Jun 2020 01:40:41 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:084bd1339d1118c2e8a50d81da5761d085ebb079eb47faa49957cbcc89168f1a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14000418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c23735b817347971b241008c1dc978437390ce830fce6cf006d678d61b8b21af`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Wed, 06 May 2020 15:29:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 06 May 2020 15:30:01 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Wed, 06 May 2020 15:30:08 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Wed, 06 May 2020 15:30:10 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:30:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:18:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:18:24 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:18:27 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:18:29 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:18:33 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:18:38 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:18:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:18:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:18:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:18:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:18:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:19:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:19:04 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:19:08 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:19:12 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:19:17 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:19:21 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5a8966b60d898cbfd9fb53281860fcb82df54d8f66c9142f4038d0e3d8afb8`  
		Last Modified: Wed, 06 May 2020 15:36:35 GMT  
		Size: 321.6 KB (321641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcdcee6bf7f07bf2e87c36762756faa63a587b445b5112371d799d9983a38d7f`  
		Last Modified: Wed, 06 May 2020 15:36:34 GMT  
		Size: 5.8 KB (5845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912d87d0a8415f3b9ba60c72fc6309c0c67fb08b2834913add34eb8344ce0826`  
		Last Modified: Wed, 06 May 2020 15:36:42 GMT  
		Size: 10.9 MB (10850936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a992aa5354ab6566aa182b0b2122386db6d1143f1bfac22dc492fd1e1c9483`  
		Last Modified: Fri, 26 Jun 2020 01:20:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:16c31b5a11f0b34504a63c04a8b8a84c455e1669a3994f207a0d2d12047f7413
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14740730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d4431f588c0c1832ba15b0e102a300b97eb5374c9434a6c17cfb6ad324eee24`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Wed, 06 May 2020 15:30:02 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 06 May 2020 15:30:03 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Wed, 06 May 2020 15:30:05 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Wed, 06 May 2020 15:30:05 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:30:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:41:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:41:44 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:41:44 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:41:44 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:41:45 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:41:45 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:41:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:41:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:41:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:41:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:41:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:41:47 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:41:47 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:41:48 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:41:48 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:41:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1098bec6a96fa022c5d1e1043cbd10f41d1b5e0788cdeb71e1cbdf3ba0f6b6`  
		Last Modified: Wed, 06 May 2020 15:32:28 GMT  
		Size: 319.2 KB (319200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b06bf33ed224c71042842eaa50af6440423bb48f5cf032ce51277c7d08cb79f`  
		Last Modified: Wed, 06 May 2020 15:32:27 GMT  
		Size: 5.8 KB (5840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b3c02c4f07ca031406ddeefa20f1428b199d11370f5548cffe6bf3c294088c`  
		Last Modified: Wed, 06 May 2020 15:32:29 GMT  
		Size: 11.8 MB (11832677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b274cabb90bbeb4aafa4418e77b128c5caf6aed9aa6b6f1f756a905af241d2cd`  
		Last Modified: Fri, 26 Jun 2020 01:42:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:4846f66a1cfa0fa858f8ae2a6c348f14be435ca26312f365ed041203bb35f48a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2311249634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94450ec6f1472f8ab0cfd101f7f68644f92c8b2262f9ea2153fdc9a0798b3917`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Tue, 09 Jun 2020 22:33:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:02:29 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:03:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Jun 2020 18:03:16 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 10 Jun 2020 18:03:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('636bb25c9738400b480ca243a605da74988deb1bc856a1cabe7ee36511db0e048ec0a2688b1640d7b157bc239d437944e43500d91881c8acc7f2b8aa138945f9')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Jun 2020 18:03:56 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Jun 2020 18:03:56 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Jun 2020 18:03:57 GMT
VOLUME [c:/config]
# Wed, 10 Jun 2020 18:03:58 GMT
VOLUME [c:/data]
# Wed, 10 Jun 2020 18:03:59 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 10 Jun 2020 18:04:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Jun 2020 18:04:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Jun 2020 18:04:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Jun 2020 18:04:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Jun 2020 18:04:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Jun 2020 18:04:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Jun 2020 18:04:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Jun 2020 18:04:07 GMT
EXPOSE 80
# Wed, 10 Jun 2020 18:04:08 GMT
EXPOSE 443
# Wed, 10 Jun 2020 18:04:08 GMT
EXPOSE 2019
# Wed, 10 Jun 2020 18:04:31 GMT
RUN caddy version
# Wed, 10 Jun 2020 18:04:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f841c6a0c622cd36b5b2688011a224ac3e8e96273758f4a2804f2f3f099f267d`  
		Last Modified: Tue, 09 Jun 2020 23:17:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e676deb3766189ea2b008f69205017c9ee31a77f9c7001fb5a07fb2e2d4fbb0`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba576338ed5242ba3fb838ce5fa930abb61e22fc422ba46b260dbca773cb9`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 4.8 MB (4772911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82aa7b0db5bd44f058750b70c9ca192d7af8986578dd9900fa68f08a53d56d7`  
		Last Modified: Wed, 10 Jun 2020 18:09:46 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6f36d669bbd2a660d47e342775c1705e6b990b004cfb461b66aeb6d978fa60`  
		Last Modified: Wed, 10 Jun 2020 18:09:50 GMT  
		Size: 12.3 MB (12262241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4caa471f3ff12126859610d5fb7a1eee050fdcd24f4c26c840a49072698064`  
		Last Modified: Wed, 10 Jun 2020 18:09:46 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f92da22ed9f6eaba0eb6cb98ff0182e5bf96b672aa9a2a5fc004584af897f91`  
		Last Modified: Wed, 10 Jun 2020 18:09:45 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ca7d66806087b4fb8e9aba7aa8c8d913f6c00b136833ce130ad342601fbcce`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2f91baaa6ad75f37691004649e965eb02f770c8901034ec1d508ac0e198c9f`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490c3bc1055c4210b37fa961535859113aa2a9e83d5373f1edb7664fec3d44a4`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d6ca5a24db2b4dabbd352548aaabc3057e21b5b1d13a3e09ff8d5b4a9f99e4`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6b40d207638f35eb44e6d1c604c7939e68829fe4e04a1ca286eea436d3b3b5`  
		Last Modified: Wed, 10 Jun 2020 18:09:42 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d137f3abb4ef203c2caea5f8b50defc1384938cae41fab9c5f751193dd801e`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ff6d828fdc817dccd02e18fb68f60dfb77e5f91b61e4039622748fdacec123`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce68242ed36c05b1696a9aed8843408c0d3df159bdd08a6f89273aea8cf2a52`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8857e417a7cd480ddc26cd312eb34880b8e76040cd4f2ea589b21fbc5d54e274`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a31891b746d7cffa5744afba11ca2c1e207076488f863fe4cb519147cbc359`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e936bc871ff19fb19ebb325dc0b2a592fd9347488450d772e434000811f5d8c`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500e96dcc8873265379cfdace5e5c75b28080e5042969250c1656de746a3eb17`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7c3e99413b53ef84bebebfb04ec29d95aa84e3f0e040dc9cbf355afca92009`  
		Last Modified: Wed, 10 Jun 2020 18:09:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790f2340b769609f7c8716568b843cd0723c59c8dc64142f1e927d5536bd9f7c`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 278.2 KB (278231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e765bd24f285691b433b20a6296e67d067e6e2918c7e1cd2ad2bef1bbd356dfc`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:64246e00b3c6726a42b20440c70003c72bc6e652f821982345b87928bc79cae5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756998229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb6c0b59ae11bc16763ab0732bf43ae0dead1bbded3284e54191f687f4a670e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:04:40 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:06:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Jun 2020 18:06:15 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 10 Jun 2020 18:07:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('636bb25c9738400b480ca243a605da74988deb1bc856a1cabe7ee36511db0e048ec0a2688b1640d7b157bc239d437944e43500d91881c8acc7f2b8aa138945f9')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Jun 2020 18:08:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Jun 2020 18:08:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Jun 2020 18:08:03 GMT
VOLUME [c:/config]
# Wed, 10 Jun 2020 18:08:04 GMT
VOLUME [c:/data]
# Wed, 10 Jun 2020 18:08:05 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 10 Jun 2020 18:08:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Jun 2020 18:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Jun 2020 18:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Jun 2020 18:08:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Jun 2020 18:08:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Jun 2020 18:08:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Jun 2020 18:08:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Jun 2020 18:08:12 GMT
EXPOSE 80
# Wed, 10 Jun 2020 18:08:13 GMT
EXPOSE 443
# Wed, 10 Jun 2020 18:08:14 GMT
EXPOSE 2019
# Wed, 10 Jun 2020 18:09:10 GMT
RUN caddy version
# Wed, 10 Jun 2020 18:09:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22985925139cd6a6e83b6eb5286a8a6e1053a5c6ddd9762f34deea2aa6bcaacc`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43c028d6768e901bc64b3edb7e2e5f72050d3ed78ea4e7337fe85725d250c15`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 5.4 MB (5404509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab96ccdd2dbffb13487e758409eaae25905b86a83e7b7a51a692c7ff18579b8d`  
		Last Modified: Wed, 10 Jun 2020 18:10:14 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aac2a7ea7e1f98bb6027b5090912006abeb6f367523aac337f6705ba4d7bb6b`  
		Last Modified: Wed, 10 Jun 2020 18:10:19 GMT  
		Size: 17.3 MB (17325836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7acf530d8fe0b1ea1f35f0e20ca267e447936a8edbae3889184d180b44c1a6`  
		Last Modified: Wed, 10 Jun 2020 18:10:13 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7609e5df44616b1f91e5434a43518cf253a69c406c062ef6b99035b20a437`  
		Last Modified: Wed, 10 Jun 2020 18:10:13 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1384cb066181208a5bb3be7023fe3f0b9cedf5483885cf330f7dcd95525302`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f2a49d3e0a25e1871a3dcb23fa333268062b4d027ae041e3bb5c0827dd0c2a`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5ec5b8bc911e1426e8c8dcc06a149b90edee45636d75da5b63e83fe91398a`  
		Last Modified: Wed, 10 Jun 2020 18:10:12 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dab68d41796a58e20ae80dc2528cfe6a2e71a04c8c88bb5595a6e0a5d7f7646`  
		Last Modified: Wed, 10 Jun 2020 18:10:10 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68da8c08840ea413933ac718a42b86738f90a6a5647e151252d4b5193ee40a8d`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946bc1b557fc88846697a1a1308c7af5ef52918f700f7dc8bd4c53e915c4a1a3`  
		Last Modified: Wed, 10 Jun 2020 18:10:09 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7ea127cbc59b2799852a077baa3bc9e46ad415abc4de6305396739a257a25e`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e77ea136bb911d1a64b32d1d139522e0e52ca1bc43b5d12aeeef7be91483d50`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a29c745913025b3a12451ab689a6186ec7756b5d99d0fa379a39ae81d510b0b`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4ae08e24e91168918350e7422b8f47200d09a7313216990ba6a672b5372280`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e219b4ef296fd92d145bf1f1a7b7d79e09c26a996daf350eb5ee70cbfeed02`  
		Last Modified: Wed, 10 Jun 2020 18:10:05 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc81bd4365ed96954980b554e769048c1e4cc97035385e22ee8364bd2856d4af`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec6f99a5c3e003e6dd16b75770a2762bb5de2737ffdd11b1c707f6aefce201a`  
		Last Modified: Wed, 10 Jun 2020 18:10:05 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26ba6de29355852954f97260ed4e96f1d30d7e675356cc21cac59feb841cf3e`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 248.4 KB (248359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef895a3d9501c41dd42a22a3e2a0458c59b35892005f5fb18b8937101a1fb50`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.0.0`

```console
$ docker pull caddy@sha256:906e32bdd357959838cd20f8a5fdb487afe307542c31b0269d9cb5c3731d0ca5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1282; amd64
	-	windows version 10.0.14393.3750; amd64

### `caddy:2.0.0` - linux; amd64

```console
$ docker pull caddy@sha256:262f58e0836d0be11253e500e3b32e78e6d6149a90ed54e4a4ed5ca736e844fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15145372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:313ad00e425a86a5b5f39170ac018ada5d833fae55ab101712e80f52b4b986de`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 13:39:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 24 Apr 2020 13:39:03 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Fri, 24 Apr 2020 13:39:05 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 19:20:49 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 16:21:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:19:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:19:44 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:19:44 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:19:44 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:19:44 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:19:44 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:19:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:19:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:19:46 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:19:46 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:19:46 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:19:47 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:19:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c92d2df695a8e1549e487fe6691311b8c3ccfdd90383c6ae37c578c4465c76`  
		Last Modified: Fri, 24 Apr 2020 13:39:22 GMT  
		Size: 318.6 KB (318554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d779d752c63b3ccba5c5fbec57ae2361cef2059d83ea0770f389f1d9849ccde`  
		Last Modified: Fri, 24 Apr 2020 13:39:22 GMT  
		Size: 5.8 KB (5765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e321d52b548add190f8f5974453da203fc605ed33865ced7b83cc1e8fddc904e`  
		Last Modified: Wed, 06 May 2020 16:21:33 GMT  
		Size: 12.0 MB (12007584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c780a87c731befe76e920c134aaa9d393de1437f0c3940f40b355bc61de8f7a6`  
		Last Modified: Fri, 26 Jun 2020 01:20:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e304abe5082419b9f5b33d893544fd83a96932dcb7e064f871bee67716222091
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.4 MB (14390760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76f2894818f3ff916764fc8e6f3111c24629f11662bd03135b07492053d9dc86`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:42:29 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 23 Apr 2020 17:42:31 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Thu, 23 Apr 2020 17:42:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 18:49:25 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:49:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 00:50:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 00:50:46 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 00:50:47 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 00:50:47 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 00:50:48 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 00:50:49 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 00:50:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 00:50:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 00:50:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 00:50:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 00:50:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 00:50:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 00:50:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 00:50:55 GMT
EXPOSE 80
# Fri, 26 Jun 2020 00:50:56 GMT
EXPOSE 443
# Fri, 26 Jun 2020 00:50:57 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 00:50:58 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 00:50:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4aecf4b3c455b15219e7ae2914078c1796d34e6b1c2916aab2fa79d0aecc97`  
		Last Modified: Thu, 23 Apr 2020 17:43:07 GMT  
		Size: 318.9 KB (318932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78f3e6c459120cfcfb844a46e1d5fa39f425743ad39e3265fdb6b4c4ea312b6`  
		Last Modified: Thu, 23 Apr 2020 17:43:07 GMT  
		Size: 5.8 KB (5842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6977aa451d29e02cfa0a60ee52aadf3bfa7fad7712ac1687007cbb0bd812f996`  
		Last Modified: Wed, 06 May 2020 15:50:14 GMT  
		Size: 11.4 MB (11445896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2e1a3cae97c62afbdf067d2b1201f2e96a4ae8bb2320a3883f82fd1aec2824`  
		Last Modified: Fri, 26 Jun 2020 00:51:21 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2653b633a6ecc87fdf8ab9941be387a42f25f1c17580878c9cd47055a726d734
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14164711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87f56b16af8dc7e3d49ffb1018e82def382e00da18d024561d9c1fbc0a392938`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 23:22:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 23 Apr 2020 23:22:58 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Thu, 23 Apr 2020 23:23:03 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 18:57:29 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:57:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 00:59:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 00:59:31 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 00:59:31 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 00:59:32 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 00:59:32 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 00:59:33 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 00:59:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 00:59:34 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 00:59:35 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 00:59:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 00:59:36 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 00:59:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 00:59:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 00:59:39 GMT
EXPOSE 80
# Fri, 26 Jun 2020 00:59:39 GMT
EXPOSE 443
# Fri, 26 Jun 2020 00:59:40 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 00:59:41 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 00:59:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf760b044fed05d609c6cc0dbc0163d673af839c2bd8b93be46a9dd9b3235d8d`  
		Last Modified: Thu, 23 Apr 2020 23:23:51 GMT  
		Size: 317.9 KB (317871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702db93291bb8c691008d86b00d866d87fd9904461e56e447408436f67069d12`  
		Last Modified: Thu, 23 Apr 2020 23:23:50 GMT  
		Size: 5.8 KB (5843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a240b5e189e2da028c9e14c55e560dda7eebabe89a0fdc68bd063df8ac5403`  
		Last Modified: Wed, 06 May 2020 15:58:14 GMT  
		Size: 11.4 MB (11418780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febb3ae65834fee908dad31bb9b1fe5dbffd24c31bd7b4d6eb3f7e0cc0be6524`  
		Last Modified: Fri, 26 Jun 2020 01:00:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:d9aef3ac6d0885fa20fd11f612c78377e9b9e12bca0d92e77205e7c90e65d07c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14099502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d385c1b96da99f80af54a8b12302cb050f0b91d661b1d5d3c876b6ae33003cfc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 03:41:26 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 24 Apr 2020 03:41:27 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Fri, 24 Apr 2020 03:41:30 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 18:39:39 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 16:39:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:40:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:40:07 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:40:08 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:40:09 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:40:09 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:40:10 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:40:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:40:11 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:40:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:40:13 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:40:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:40:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:40:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:40:16 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:40:16 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:40:17 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:40:18 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:40:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1dd90474a5634d83eea66237a34342ba1aa7b9660127d7a6168f9dd16a6800`  
		Last Modified: Fri, 24 Apr 2020 03:42:02 GMT  
		Size: 319.1 KB (319109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523ce157ee2040adfd1d897f97c884c8df6de54df4581f3982d4114fea063843`  
		Last Modified: Fri, 24 Apr 2020 03:42:02 GMT  
		Size: 5.8 KB (5843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45586f3cd2c78aa4e4ec308b720449bd298ff8184489fc23ed1b63329d5bfba`  
		Last Modified: Wed, 06 May 2020 16:40:28 GMT  
		Size: 11.0 MB (11049973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f00aaba3fbdd96271be17e7a6a5b181a398f7c2f05bc510c8fb471d69578081`  
		Last Modified: Fri, 26 Jun 2020 01:40:41 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0` - linux; ppc64le

```console
$ docker pull caddy@sha256:084bd1339d1118c2e8a50d81da5761d085ebb079eb47faa49957cbcc89168f1a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14000418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c23735b817347971b241008c1dc978437390ce830fce6cf006d678d61b8b21af`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Wed, 06 May 2020 15:29:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 06 May 2020 15:30:01 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Wed, 06 May 2020 15:30:08 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Wed, 06 May 2020 15:30:10 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:30:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:18:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:18:24 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:18:27 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:18:29 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:18:33 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:18:38 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:18:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:18:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:18:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:18:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:18:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:19:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:19:04 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:19:08 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:19:12 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:19:17 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:19:21 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5a8966b60d898cbfd9fb53281860fcb82df54d8f66c9142f4038d0e3d8afb8`  
		Last Modified: Wed, 06 May 2020 15:36:35 GMT  
		Size: 321.6 KB (321641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcdcee6bf7f07bf2e87c36762756faa63a587b445b5112371d799d9983a38d7f`  
		Last Modified: Wed, 06 May 2020 15:36:34 GMT  
		Size: 5.8 KB (5845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912d87d0a8415f3b9ba60c72fc6309c0c67fb08b2834913add34eb8344ce0826`  
		Last Modified: Wed, 06 May 2020 15:36:42 GMT  
		Size: 10.9 MB (10850936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a992aa5354ab6566aa182b0b2122386db6d1143f1bfac22dc492fd1e1c9483`  
		Last Modified: Fri, 26 Jun 2020 01:20:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0` - linux; s390x

```console
$ docker pull caddy@sha256:16c31b5a11f0b34504a63c04a8b8a84c455e1669a3994f207a0d2d12047f7413
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14740730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d4431f588c0c1832ba15b0e102a300b97eb5374c9434a6c17cfb6ad324eee24`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Wed, 06 May 2020 15:30:02 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 06 May 2020 15:30:03 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Wed, 06 May 2020 15:30:05 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Wed, 06 May 2020 15:30:05 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:30:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:41:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:41:44 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:41:44 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:41:44 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:41:45 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:41:45 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:41:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:41:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:41:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:41:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:41:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:41:47 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:41:47 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:41:48 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:41:48 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:41:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1098bec6a96fa022c5d1e1043cbd10f41d1b5e0788cdeb71e1cbdf3ba0f6b6`  
		Last Modified: Wed, 06 May 2020 15:32:28 GMT  
		Size: 319.2 KB (319200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b06bf33ed224c71042842eaa50af6440423bb48f5cf032ce51277c7d08cb79f`  
		Last Modified: Wed, 06 May 2020 15:32:27 GMT  
		Size: 5.8 KB (5840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b3c02c4f07ca031406ddeefa20f1428b199d11370f5548cffe6bf3c294088c`  
		Last Modified: Wed, 06 May 2020 15:32:29 GMT  
		Size: 11.8 MB (11832677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b274cabb90bbeb4aafa4418e77b128c5caf6aed9aa6b6f1f756a905af241d2cd`  
		Last Modified: Fri, 26 Jun 2020 01:42:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:4846f66a1cfa0fa858f8ae2a6c348f14be435ca26312f365ed041203bb35f48a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2311249634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94450ec6f1472f8ab0cfd101f7f68644f92c8b2262f9ea2153fdc9a0798b3917`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Tue, 09 Jun 2020 22:33:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:02:29 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:03:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Jun 2020 18:03:16 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 10 Jun 2020 18:03:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('636bb25c9738400b480ca243a605da74988deb1bc856a1cabe7ee36511db0e048ec0a2688b1640d7b157bc239d437944e43500d91881c8acc7f2b8aa138945f9')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Jun 2020 18:03:56 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Jun 2020 18:03:56 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Jun 2020 18:03:57 GMT
VOLUME [c:/config]
# Wed, 10 Jun 2020 18:03:58 GMT
VOLUME [c:/data]
# Wed, 10 Jun 2020 18:03:59 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 10 Jun 2020 18:04:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Jun 2020 18:04:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Jun 2020 18:04:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Jun 2020 18:04:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Jun 2020 18:04:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Jun 2020 18:04:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Jun 2020 18:04:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Jun 2020 18:04:07 GMT
EXPOSE 80
# Wed, 10 Jun 2020 18:04:08 GMT
EXPOSE 443
# Wed, 10 Jun 2020 18:04:08 GMT
EXPOSE 2019
# Wed, 10 Jun 2020 18:04:31 GMT
RUN caddy version
# Wed, 10 Jun 2020 18:04:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f841c6a0c622cd36b5b2688011a224ac3e8e96273758f4a2804f2f3f099f267d`  
		Last Modified: Tue, 09 Jun 2020 23:17:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e676deb3766189ea2b008f69205017c9ee31a77f9c7001fb5a07fb2e2d4fbb0`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba576338ed5242ba3fb838ce5fa930abb61e22fc422ba46b260dbca773cb9`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 4.8 MB (4772911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82aa7b0db5bd44f058750b70c9ca192d7af8986578dd9900fa68f08a53d56d7`  
		Last Modified: Wed, 10 Jun 2020 18:09:46 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6f36d669bbd2a660d47e342775c1705e6b990b004cfb461b66aeb6d978fa60`  
		Last Modified: Wed, 10 Jun 2020 18:09:50 GMT  
		Size: 12.3 MB (12262241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4caa471f3ff12126859610d5fb7a1eee050fdcd24f4c26c840a49072698064`  
		Last Modified: Wed, 10 Jun 2020 18:09:46 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f92da22ed9f6eaba0eb6cb98ff0182e5bf96b672aa9a2a5fc004584af897f91`  
		Last Modified: Wed, 10 Jun 2020 18:09:45 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ca7d66806087b4fb8e9aba7aa8c8d913f6c00b136833ce130ad342601fbcce`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2f91baaa6ad75f37691004649e965eb02f770c8901034ec1d508ac0e198c9f`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490c3bc1055c4210b37fa961535859113aa2a9e83d5373f1edb7664fec3d44a4`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d6ca5a24db2b4dabbd352548aaabc3057e21b5b1d13a3e09ff8d5b4a9f99e4`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6b40d207638f35eb44e6d1c604c7939e68829fe4e04a1ca286eea436d3b3b5`  
		Last Modified: Wed, 10 Jun 2020 18:09:42 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d137f3abb4ef203c2caea5f8b50defc1384938cae41fab9c5f751193dd801e`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ff6d828fdc817dccd02e18fb68f60dfb77e5f91b61e4039622748fdacec123`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce68242ed36c05b1696a9aed8843408c0d3df159bdd08a6f89273aea8cf2a52`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8857e417a7cd480ddc26cd312eb34880b8e76040cd4f2ea589b21fbc5d54e274`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a31891b746d7cffa5744afba11ca2c1e207076488f863fe4cb519147cbc359`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e936bc871ff19fb19ebb325dc0b2a592fd9347488450d772e434000811f5d8c`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500e96dcc8873265379cfdace5e5c75b28080e5042969250c1656de746a3eb17`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7c3e99413b53ef84bebebfb04ec29d95aa84e3f0e040dc9cbf355afca92009`  
		Last Modified: Wed, 10 Jun 2020 18:09:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790f2340b769609f7c8716568b843cd0723c59c8dc64142f1e927d5536bd9f7c`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 278.2 KB (278231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e765bd24f285691b433b20a6296e67d067e6e2918c7e1cd2ad2bef1bbd356dfc`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:64246e00b3c6726a42b20440c70003c72bc6e652f821982345b87928bc79cae5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756998229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb6c0b59ae11bc16763ab0732bf43ae0dead1bbded3284e54191f687f4a670e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:04:40 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:06:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Jun 2020 18:06:15 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 10 Jun 2020 18:07:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('636bb25c9738400b480ca243a605da74988deb1bc856a1cabe7ee36511db0e048ec0a2688b1640d7b157bc239d437944e43500d91881c8acc7f2b8aa138945f9')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Jun 2020 18:08:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Jun 2020 18:08:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Jun 2020 18:08:03 GMT
VOLUME [c:/config]
# Wed, 10 Jun 2020 18:08:04 GMT
VOLUME [c:/data]
# Wed, 10 Jun 2020 18:08:05 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 10 Jun 2020 18:08:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Jun 2020 18:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Jun 2020 18:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Jun 2020 18:08:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Jun 2020 18:08:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Jun 2020 18:08:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Jun 2020 18:08:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Jun 2020 18:08:12 GMT
EXPOSE 80
# Wed, 10 Jun 2020 18:08:13 GMT
EXPOSE 443
# Wed, 10 Jun 2020 18:08:14 GMT
EXPOSE 2019
# Wed, 10 Jun 2020 18:09:10 GMT
RUN caddy version
# Wed, 10 Jun 2020 18:09:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22985925139cd6a6e83b6eb5286a8a6e1053a5c6ddd9762f34deea2aa6bcaacc`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43c028d6768e901bc64b3edb7e2e5f72050d3ed78ea4e7337fe85725d250c15`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 5.4 MB (5404509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab96ccdd2dbffb13487e758409eaae25905b86a83e7b7a51a692c7ff18579b8d`  
		Last Modified: Wed, 10 Jun 2020 18:10:14 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aac2a7ea7e1f98bb6027b5090912006abeb6f367523aac337f6705ba4d7bb6b`  
		Last Modified: Wed, 10 Jun 2020 18:10:19 GMT  
		Size: 17.3 MB (17325836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7acf530d8fe0b1ea1f35f0e20ca267e447936a8edbae3889184d180b44c1a6`  
		Last Modified: Wed, 10 Jun 2020 18:10:13 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7609e5df44616b1f91e5434a43518cf253a69c406c062ef6b99035b20a437`  
		Last Modified: Wed, 10 Jun 2020 18:10:13 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1384cb066181208a5bb3be7023fe3f0b9cedf5483885cf330f7dcd95525302`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f2a49d3e0a25e1871a3dcb23fa333268062b4d027ae041e3bb5c0827dd0c2a`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5ec5b8bc911e1426e8c8dcc06a149b90edee45636d75da5b63e83fe91398a`  
		Last Modified: Wed, 10 Jun 2020 18:10:12 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dab68d41796a58e20ae80dc2528cfe6a2e71a04c8c88bb5595a6e0a5d7f7646`  
		Last Modified: Wed, 10 Jun 2020 18:10:10 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68da8c08840ea413933ac718a42b86738f90a6a5647e151252d4b5193ee40a8d`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946bc1b557fc88846697a1a1308c7af5ef52918f700f7dc8bd4c53e915c4a1a3`  
		Last Modified: Wed, 10 Jun 2020 18:10:09 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7ea127cbc59b2799852a077baa3bc9e46ad415abc4de6305396739a257a25e`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e77ea136bb911d1a64b32d1d139522e0e52ca1bc43b5d12aeeef7be91483d50`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a29c745913025b3a12451ab689a6186ec7756b5d99d0fa379a39ae81d510b0b`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4ae08e24e91168918350e7422b8f47200d09a7313216990ba6a672b5372280`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e219b4ef296fd92d145bf1f1a7b7d79e09c26a996daf350eb5ee70cbfeed02`  
		Last Modified: Wed, 10 Jun 2020 18:10:05 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc81bd4365ed96954980b554e769048c1e4cc97035385e22ee8364bd2856d4af`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec6f99a5c3e003e6dd16b75770a2762bb5de2737ffdd11b1c707f6aefce201a`  
		Last Modified: Wed, 10 Jun 2020 18:10:05 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26ba6de29355852954f97260ed4e96f1d30d7e675356cc21cac59feb841cf3e`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 248.4 KB (248359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef895a3d9501c41dd42a22a3e2a0458c59b35892005f5fb18b8937101a1fb50`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.0.0-alpine`

```console
$ docker pull caddy@sha256:a985dd43871e9cb6c6ab3f9e45dd7bac9732f9f8d7c35f5d1b78a160b57bee4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.0.0-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:262f58e0836d0be11253e500e3b32e78e6d6149a90ed54e4a4ed5ca736e844fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15145372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:313ad00e425a86a5b5f39170ac018ada5d833fae55ab101712e80f52b4b986de`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 13:39:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 24 Apr 2020 13:39:03 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Fri, 24 Apr 2020 13:39:05 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 19:20:49 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 16:21:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:19:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:19:44 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:19:44 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:19:44 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:19:44 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:19:44 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:19:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:19:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:19:46 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:19:46 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:19:46 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:19:47 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:19:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c92d2df695a8e1549e487fe6691311b8c3ccfdd90383c6ae37c578c4465c76`  
		Last Modified: Fri, 24 Apr 2020 13:39:22 GMT  
		Size: 318.6 KB (318554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d779d752c63b3ccba5c5fbec57ae2361cef2059d83ea0770f389f1d9849ccde`  
		Last Modified: Fri, 24 Apr 2020 13:39:22 GMT  
		Size: 5.8 KB (5765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e321d52b548add190f8f5974453da203fc605ed33865ced7b83cc1e8fddc904e`  
		Last Modified: Wed, 06 May 2020 16:21:33 GMT  
		Size: 12.0 MB (12007584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c780a87c731befe76e920c134aaa9d393de1437f0c3940f40b355bc61de8f7a6`  
		Last Modified: Fri, 26 Jun 2020 01:20:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e304abe5082419b9f5b33d893544fd83a96932dcb7e064f871bee67716222091
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.4 MB (14390760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76f2894818f3ff916764fc8e6f3111c24629f11662bd03135b07492053d9dc86`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:42:29 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 23 Apr 2020 17:42:31 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Thu, 23 Apr 2020 17:42:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 18:49:25 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:49:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 00:50:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 00:50:46 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 00:50:47 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 00:50:47 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 00:50:48 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 00:50:49 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 00:50:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 00:50:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 00:50:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 00:50:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 00:50:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 00:50:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 00:50:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 00:50:55 GMT
EXPOSE 80
# Fri, 26 Jun 2020 00:50:56 GMT
EXPOSE 443
# Fri, 26 Jun 2020 00:50:57 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 00:50:58 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 00:50:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4aecf4b3c455b15219e7ae2914078c1796d34e6b1c2916aab2fa79d0aecc97`  
		Last Modified: Thu, 23 Apr 2020 17:43:07 GMT  
		Size: 318.9 KB (318932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78f3e6c459120cfcfb844a46e1d5fa39f425743ad39e3265fdb6b4c4ea312b6`  
		Last Modified: Thu, 23 Apr 2020 17:43:07 GMT  
		Size: 5.8 KB (5842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6977aa451d29e02cfa0a60ee52aadf3bfa7fad7712ac1687007cbb0bd812f996`  
		Last Modified: Wed, 06 May 2020 15:50:14 GMT  
		Size: 11.4 MB (11445896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2e1a3cae97c62afbdf067d2b1201f2e96a4ae8bb2320a3883f82fd1aec2824`  
		Last Modified: Fri, 26 Jun 2020 00:51:21 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2653b633a6ecc87fdf8ab9941be387a42f25f1c17580878c9cd47055a726d734
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14164711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87f56b16af8dc7e3d49ffb1018e82def382e00da18d024561d9c1fbc0a392938`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 23:22:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 23 Apr 2020 23:22:58 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Thu, 23 Apr 2020 23:23:03 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 18:57:29 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:57:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 00:59:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 00:59:31 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 00:59:31 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 00:59:32 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 00:59:32 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 00:59:33 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 00:59:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 00:59:34 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 00:59:35 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 00:59:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 00:59:36 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 00:59:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 00:59:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 00:59:39 GMT
EXPOSE 80
# Fri, 26 Jun 2020 00:59:39 GMT
EXPOSE 443
# Fri, 26 Jun 2020 00:59:40 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 00:59:41 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 00:59:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf760b044fed05d609c6cc0dbc0163d673af839c2bd8b93be46a9dd9b3235d8d`  
		Last Modified: Thu, 23 Apr 2020 23:23:51 GMT  
		Size: 317.9 KB (317871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702db93291bb8c691008d86b00d866d87fd9904461e56e447408436f67069d12`  
		Last Modified: Thu, 23 Apr 2020 23:23:50 GMT  
		Size: 5.8 KB (5843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a240b5e189e2da028c9e14c55e560dda7eebabe89a0fdc68bd063df8ac5403`  
		Last Modified: Wed, 06 May 2020 15:58:14 GMT  
		Size: 11.4 MB (11418780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febb3ae65834fee908dad31bb9b1fe5dbffd24c31bd7b4d6eb3f7e0cc0be6524`  
		Last Modified: Fri, 26 Jun 2020 01:00:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:d9aef3ac6d0885fa20fd11f612c78377e9b9e12bca0d92e77205e7c90e65d07c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14099502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d385c1b96da99f80af54a8b12302cb050f0b91d661b1d5d3c876b6ae33003cfc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 03:41:26 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 24 Apr 2020 03:41:27 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Fri, 24 Apr 2020 03:41:30 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 18:39:39 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 16:39:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:40:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:40:07 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:40:08 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:40:09 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:40:09 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:40:10 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:40:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:40:11 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:40:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:40:13 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:40:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:40:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:40:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:40:16 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:40:16 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:40:17 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:40:18 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:40:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1dd90474a5634d83eea66237a34342ba1aa7b9660127d7a6168f9dd16a6800`  
		Last Modified: Fri, 24 Apr 2020 03:42:02 GMT  
		Size: 319.1 KB (319109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523ce157ee2040adfd1d897f97c884c8df6de54df4581f3982d4114fea063843`  
		Last Modified: Fri, 24 Apr 2020 03:42:02 GMT  
		Size: 5.8 KB (5843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45586f3cd2c78aa4e4ec308b720449bd298ff8184489fc23ed1b63329d5bfba`  
		Last Modified: Wed, 06 May 2020 16:40:28 GMT  
		Size: 11.0 MB (11049973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f00aaba3fbdd96271be17e7a6a5b181a398f7c2f05bc510c8fb471d69578081`  
		Last Modified: Fri, 26 Jun 2020 01:40:41 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:084bd1339d1118c2e8a50d81da5761d085ebb079eb47faa49957cbcc89168f1a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14000418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c23735b817347971b241008c1dc978437390ce830fce6cf006d678d61b8b21af`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Wed, 06 May 2020 15:29:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 06 May 2020 15:30:01 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Wed, 06 May 2020 15:30:08 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Wed, 06 May 2020 15:30:10 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:30:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:18:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:18:24 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:18:27 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:18:29 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:18:33 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:18:38 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:18:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:18:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:18:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:18:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:18:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:19:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:19:04 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:19:08 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:19:12 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:19:17 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:19:21 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5a8966b60d898cbfd9fb53281860fcb82df54d8f66c9142f4038d0e3d8afb8`  
		Last Modified: Wed, 06 May 2020 15:36:35 GMT  
		Size: 321.6 KB (321641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcdcee6bf7f07bf2e87c36762756faa63a587b445b5112371d799d9983a38d7f`  
		Last Modified: Wed, 06 May 2020 15:36:34 GMT  
		Size: 5.8 KB (5845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912d87d0a8415f3b9ba60c72fc6309c0c67fb08b2834913add34eb8344ce0826`  
		Last Modified: Wed, 06 May 2020 15:36:42 GMT  
		Size: 10.9 MB (10850936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a992aa5354ab6566aa182b0b2122386db6d1143f1bfac22dc492fd1e1c9483`  
		Last Modified: Fri, 26 Jun 2020 01:20:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:16c31b5a11f0b34504a63c04a8b8a84c455e1669a3994f207a0d2d12047f7413
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14740730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d4431f588c0c1832ba15b0e102a300b97eb5374c9434a6c17cfb6ad324eee24`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Wed, 06 May 2020 15:30:02 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 06 May 2020 15:30:03 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Wed, 06 May 2020 15:30:05 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Wed, 06 May 2020 15:30:05 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:30:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:41:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:41:44 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:41:44 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:41:44 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:41:45 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:41:45 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:41:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:41:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:41:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:41:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:41:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:41:47 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:41:47 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:41:48 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:41:48 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:41:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1098bec6a96fa022c5d1e1043cbd10f41d1b5e0788cdeb71e1cbdf3ba0f6b6`  
		Last Modified: Wed, 06 May 2020 15:32:28 GMT  
		Size: 319.2 KB (319200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b06bf33ed224c71042842eaa50af6440423bb48f5cf032ce51277c7d08cb79f`  
		Last Modified: Wed, 06 May 2020 15:32:27 GMT  
		Size: 5.8 KB (5840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b3c02c4f07ca031406ddeefa20f1428b199d11370f5548cffe6bf3c294088c`  
		Last Modified: Wed, 06 May 2020 15:32:29 GMT  
		Size: 11.8 MB (11832677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b274cabb90bbeb4aafa4418e77b128c5caf6aed9aa6b6f1f756a905af241d2cd`  
		Last Modified: Fri, 26 Jun 2020 01:42:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.0.0-builder`

```console
$ docker pull caddy@sha256:e7f19375fb2af512955ebfe845d8ea78b32cae8c608d367d393cbc209fc2cf3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.0.0-builder` - linux; amd64

```console
$ docker pull caddy@sha256:0750762062e92c7e2e8aa0c2c7e80d5762f6771f9c38aee0d4369b562bdad52b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.8 MB (322833946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed310fb9f0cd01f3920b3f64f1697fea83efa462d6fefdd30cc519a005c6910b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:29:00 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 24 Apr 2020 14:29:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:32:50 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:35:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:35:10 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:35:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:35:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:35:11 GMT
WORKDIR /go
# Tue, 02 Jun 2020 02:32:26 GMT
WORKDIR /src
# Tue, 02 Jun 2020 02:32:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 02 Jun 2020 02:32:27 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0
# Tue, 02 Jun 2020 02:32:28 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 02 Jun 2020 02:32:29 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 02 Jun 2020 02:32:42 GMT
RUN go get -d ./...
# Tue, 02 Jun 2020 02:32:42 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 02 Jun 2020 02:32:42 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408f875501273f3af2a9cbff2a23e736585641e73da80dd81712518b28e7843c`  
		Last Modified: Fri, 24 Apr 2020 14:36:50 GMT  
		Size: 301.3 KB (301282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe522b08c9798748151fec9b7a908aca712cd102cfcbb8ed79d57d05b71e6cc4`  
		Last Modified: Fri, 24 Apr 2020 14:36:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1be7d07969680a19c74f96783bb978cfc281d9eb21dd6377a1ba0c60b22161`  
		Last Modified: Tue, 02 Jun 2020 01:45:12 GMT  
		Size: 132.1 MB (132121186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed5455f4aa4c7ceedfadd2f093fffcda763951c5ae506c6d92151ad6e4dae0e`  
		Last Modified: Tue, 02 Jun 2020 01:44:46 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45598100dcda08511c93d19c558a05a901b1a183efefa4cda30b7c7e6f93d03c`  
		Last Modified: Tue, 02 Jun 2020 02:32:53 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89489597245daae1172eaaf4fc1db5044f7684053f7428c9e2b93b567d6d50d`  
		Last Modified: Tue, 02 Jun 2020 02:32:54 GMT  
		Size: 8.2 MB (8177829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc24cd02350289621830e1a9e35520aaa1bc92133dd8b9f775d5d108f93126cc`  
		Last Modified: Tue, 02 Jun 2020 02:32:52 GMT  
		Size: 2.7 MB (2706286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4dbcd3eb953512768ffac90d7561911f8d07b650519e87a8f150417c4210b3`  
		Last Modified: Tue, 02 Jun 2020 02:33:13 GMT  
		Size: 176.7 MB (176713022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461dd6e5ccc455d939c9a53d58c106ce85ec9f7f0c674299b3d974445993dc8c`  
		Last Modified: Tue, 02 Jun 2020 02:32:52 GMT  
		Size: 502.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71023d2750548230f0a4dc5e3687b6c7a8faa42933147a45edaf1d1b0e7155a`  
		Last Modified: Tue, 02 Jun 2020 02:32:52 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f722d703d3a5a30563460536bd3a850b5175ad79c43c8a9397b0b3a5c8f100d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.4 MB (318375279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcb7124899c5889d20b2be36389f5a3f3741f34b9afba1078c43835dea3cd923`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:43:41 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 23 Apr 2020 17:43:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 02:56:25 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 03:51:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 03:51:21 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 03:51:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 03:51:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 03:51:26 GMT
WORKDIR /go
# Tue, 02 Jun 2020 05:40:14 GMT
WORKDIR /src
# Tue, 02 Jun 2020 05:40:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 02 Jun 2020 05:40:17 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0
# Tue, 02 Jun 2020 05:40:19 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 02 Jun 2020 05:40:20 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 02 Jun 2020 05:41:15 GMT
RUN go get -d ./...
# Tue, 02 Jun 2020 05:41:20 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 02 Jun 2020 05:41:21 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ace047eafbdd1d41e753db1fd1004be452f749a7de56a3d24b2614a64577f5`  
		Last Modified: Thu, 23 Apr 2020 18:03:18 GMT  
		Size: 301.6 KB (301629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d0031acb1953f56f2c2592c1c5882b29aa828d45deccabbb9a1b5483090a43`  
		Last Modified: Thu, 23 Apr 2020 18:03:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c18b24b5eeba6322ca5f9b2eedb021ca9618b062bdf48b250ed4b201dc8050`  
		Last Modified: Tue, 02 Jun 2020 05:23:03 GMT  
		Size: 128.2 MB (128229189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de88420151b6ca5c6fc039fda4383cb82cf3566fa1cc6b2858d6fb47afe6ceb`  
		Last Modified: Tue, 02 Jun 2020 05:22:20 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f480e87ad21aa1d6eeb3d546b707aaaef59a9dc5dc0c6e5e14dcbe96c28cd9c`  
		Last Modified: Tue, 02 Jun 2020 05:41:39 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f74f503577c8c19df94e7f595796fd4e4e15166602d5843a4e28a694ef5e28f`  
		Last Modified: Tue, 02 Jun 2020 05:41:40 GMT  
		Size: 7.8 MB (7794708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12265e99f76b1fae972b3d710b32e05095595f8f0a5c088f78a217027939799`  
		Last Modified: Tue, 02 Jun 2020 05:41:38 GMT  
		Size: 2.7 MB (2712506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c581c17f5029909335c44e9a561b604aa98c4db79d38d9e87cae2749bcc658ce`  
		Last Modified: Tue, 02 Jun 2020 05:42:22 GMT  
		Size: 176.7 MB (176716184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57481f1b24f0912bad71decaec966f45bf686c9b218bd73fa4335d867d765ed7`  
		Last Modified: Tue, 02 Jun 2020 05:41:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd612876bd12eb68ab6685845a9b5cc04abca31e2e6292058dee233260487cf`  
		Last Modified: Tue, 02 Jun 2020 05:41:38 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0c21b0ed54253ffdfa14547e326d48beebbf4b92bb8da76b92edb8c3c6abf04c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.0 MB (317037998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4388ab5685329446df0ddd799ba01c8a93d5feb07b8e6347d7c48a4827f0ac0c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:27:40 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 24 Apr 2020 02:27:42 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:35:08 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:59:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:59:49 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:59:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:59:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:59:54 GMT
WORKDIR /go
# Tue, 02 Jun 2020 04:45:11 GMT
WORKDIR /src
# Tue, 02 Jun 2020 04:45:33 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 02 Jun 2020 04:45:42 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0
# Tue, 02 Jun 2020 04:46:08 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 02 Jun 2020 04:46:18 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 02 Jun 2020 04:48:25 GMT
RUN go get -d ./...
# Tue, 02 Jun 2020 04:48:36 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 02 Jun 2020 04:48:46 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a35d9f7887ef683587262c6f5ed88364f59775ff882c71bde03cc59f382ffd`  
		Last Modified: Fri, 24 Apr 2020 03:39:46 GMT  
		Size: 300.6 KB (300593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce21b09ea3d1107df35d9f41a664183faabfc461b8f093ab8e9a34d91e8e71b`  
		Last Modified: Fri, 24 Apr 2020 03:39:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f154a497a43d3932627d4ed19f8a725b92bc6ff032696fd7d02c923aabfdfcd`  
		Last Modified: Tue, 02 Jun 2020 03:53:43 GMT  
		Size: 127.9 MB (127859153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356485fde635696dcdacee878dba8a58e09b58537b064b5f1661e5bbede500c1`  
		Last Modified: Tue, 02 Jun 2020 03:52:31 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955b3271dbcc86df5de81f5274c182306cd2a0e95581acd9a21262668cf2b88a`  
		Last Modified: Tue, 02 Jun 2020 04:49:24 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9e684ca35cc26b7059bb60e83771de2a6b96091a053dd7ecb7b81deeb696fd`  
		Last Modified: Tue, 02 Jun 2020 04:49:20 GMT  
		Size: 7.0 MB (7026779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1d162e820fa1c08e63c96be54a52b452f50218eeeee10b1260cd22d2250215`  
		Last Modified: Tue, 02 Jun 2020 04:49:20 GMT  
		Size: 2.7 MB (2712499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8138743a5c1e38d4db8ff61f24498d97cd9294a19cd9f2c6d88e8be776aa557e`  
		Last Modified: Tue, 02 Jun 2020 04:50:16 GMT  
		Size: 176.7 MB (176715788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e9777f9df18524b4ce10bcb6db5fb00912bde1d57de9ee77e0485b7ca87149`  
		Last Modified: Tue, 02 Jun 2020 04:49:20 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dbf791500a5a018208ecaed66e5d8afc28ca5be7ae31fb54c8b02c6dc02f68`  
		Last Modified: Tue, 02 Jun 2020 04:49:20 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:fa63e1ed3b5857fc2afa0da0e5f87e46c465ca4285b2f4256f033c7d0e075e16
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.3 MB (317306406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa08366dd0271d82e7194ee208f71f532fe0ef0edc70f7f2e9ace0fe35e206c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 24 Apr 2020 09:30:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 02:01:25 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 02:05:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 02:05:51 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 02:06:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 02:07:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 02:07:23 GMT
WORKDIR /go
# Tue, 02 Jun 2020 03:54:39 GMT
WORKDIR /src
# Tue, 02 Jun 2020 03:55:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 02 Jun 2020 03:55:25 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0
# Tue, 02 Jun 2020 03:56:04 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 02 Jun 2020 03:56:07 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 02 Jun 2020 03:57:15 GMT
RUN go get -d ./...
# Tue, 02 Jun 2020 03:57:23 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 02 Jun 2020 03:57:32 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fc45ca0357821724e2824e141e2062d236dedad3d8654e0a390419ec9fe393`  
		Last Modified: Fri, 24 Apr 2020 09:38:53 GMT  
		Size: 301.8 KB (301770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6332e392c90a454bd9f70a303cda942eb0e131e321e82cb70b9346ece4a52a64`  
		Last Modified: Fri, 24 Apr 2020 09:38:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d8f54f55a2670968860ca35a8c2a0e2e526b543894d26874eae63fc6ce1532`  
		Last Modified: Tue, 02 Jun 2020 02:30:54 GMT  
		Size: 126.5 MB (126491009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2603d501b5a4a0cd3f6da1f592af79cba3b33143d7e3c4abd674ddc768193ec`  
		Last Modified: Tue, 02 Jun 2020 02:30:16 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2a6789a8ae4894bb21533776d982f6c268fcdcf9f33941f162b63755960e3b`  
		Last Modified: Tue, 02 Jun 2020 03:57:57 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248984096d3b57adf469c453ec30db708388da2d14aab956f1204e917ca27c4`  
		Last Modified: Tue, 02 Jun 2020 03:57:58 GMT  
		Size: 8.4 MB (8365435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d43f4d0862815e18a79d45498f2fbcfd99029a2863caf46b05618fd0e1cd5fd`  
		Last Modified: Tue, 02 Jun 2020 03:57:54 GMT  
		Size: 2.7 MB (2706372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bafe3a72624764aa34e658d59aff5bb317ff49f7624c43d47d9e5c575902a984`  
		Last Modified: Tue, 02 Jun 2020 03:58:33 GMT  
		Size: 176.7 MB (176716269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905e846552ef4792a1bc0924a7fafdf9fe2e669c5e91a25b222fc69a0ef958d0`  
		Last Modified: Tue, 02 Jun 2020 03:57:53 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ba0a8ecba94bf6fe06e59d7631f3e6ba4f79bbeccac3628b0b9bdb13825406`  
		Last Modified: Tue, 02 Jun 2020 03:57:53 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:6891c6d6490e09d98441446daa3f60dc3c0b1eef350bd60f15da70ce0c66e22d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.6 MB (316596303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d43482e81b370ae7732fbdf178f88ef7b057e0a406359ccbce7ad214d309fbf`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:54:40 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 24 Apr 2020 02:54:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:32:58 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:36:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:36:14 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:36:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:36:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:36:38 GMT
WORKDIR /go
# Tue, 02 Jun 2020 02:07:41 GMT
WORKDIR /src
# Tue, 02 Jun 2020 02:07:52 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 02 Jun 2020 02:07:56 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0
# Tue, 02 Jun 2020 02:08:01 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 02 Jun 2020 02:08:03 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 02 Jun 2020 02:10:04 GMT
RUN go get -d ./...
# Tue, 02 Jun 2020 02:10:07 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 02 Jun 2020 02:10:10 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20efe26326b88a40e960e9cd11fce1b701b2cf370e8328f66fc846d23b5408`  
		Last Modified: Fri, 24 Apr 2020 03:02:11 GMT  
		Size: 304.0 KB (303974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7438e1bdec433812841560459973aca70d85a3b7661615d9c632998dd366f248`  
		Last Modified: Fri, 24 Apr 2020 03:02:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665e10aea526140928afce65b052e28ac4f223162c45360135430121de27c7d7`  
		Last Modified: Tue, 02 Jun 2020 01:49:39 GMT  
		Size: 125.3 MB (125264184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1501bdd7b2a43f71acacc2d8a1122da868e702b75b2b680b69707544a4d2a6`  
		Last Modified: Tue, 02 Jun 2020 01:49:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e91f288ec567edbbf295fad3a3dadb1e59f32db4395eed7839b6ec89b8e2e1b`  
		Last Modified: Tue, 02 Jun 2020 02:10:32 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61996a2194cfe615b8d4f165ab0698f11f77f099cacb4305e2b4a48ecb23d85`  
		Last Modified: Tue, 02 Jun 2020 02:10:32 GMT  
		Size: 8.8 MB (8784628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5252de731606eac2f54796e9249033424cc547c2f7cfda78819e9bad6336d64b`  
		Last Modified: Tue, 02 Jun 2020 02:10:33 GMT  
		Size: 2.7 MB (2706339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3b270c7436a0d3b6f52d2c3ca32e87b1aa6b6cb910d93c8d8c146c281cb098`  
		Last Modified: Tue, 02 Jun 2020 02:10:57 GMT  
		Size: 176.7 MB (176714209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb2be7c1dce157b09712be8befda6ffc7db62d04638eb8de0ffcedc9c72ef9e`  
		Last Modified: Tue, 02 Jun 2020 02:10:29 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1a34918806b67ebe40004ce44428f56acf696819686c01055ec4bba3e40147`  
		Last Modified: Tue, 02 Jun 2020 02:10:30 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0-builder` - linux; s390x

```console
$ docker pull caddy@sha256:947edd15c7a7b1de99ef6de49bfdba2c2f48b5ac85cdd68429a8d2b308b9fd39
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.3 MB (322334003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:732919a18d2ee22b245cf74dbe9e1e6119e7364d09f35705c4641f8ab310185b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 20:01:10 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 23 Apr 2020 20:01:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:54:47 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:56:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:56:06 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:56:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:56:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:56:07 GMT
WORKDIR /go
# Tue, 02 Jun 2020 02:18:58 GMT
WORKDIR /src
# Tue, 02 Jun 2020 02:18:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 02 Jun 2020 02:19:00 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0
# Tue, 02 Jun 2020 02:19:01 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 02 Jun 2020 02:19:01 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 02 Jun 2020 02:19:20 GMT
RUN go get -d ./...
# Tue, 02 Jun 2020 02:19:28 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 02 Jun 2020 02:19:28 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bb5699ff3d626466b57d4c92bbf8a5410490fcece2b350c368cad50778b96d`  
		Last Modified: Thu, 23 Apr 2020 20:06:33 GMT  
		Size: 301.9 KB (301908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf86b8de56aab63659ca622083cd8174db3525f6baa42836863267efa18de0e2`  
		Last Modified: Thu, 23 Apr 2020 20:06:33 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fc33aefc5654dc9f18f8874ec5df3f0054d95efb6068093b66a806c1a47e54`  
		Last Modified: Tue, 02 Jun 2020 02:02:05 GMT  
		Size: 131.8 MB (131813328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb93b54892812fb36828c107902c548f3819372e46c12a6ecc0a7f79d29bdfd7`  
		Last Modified: Tue, 02 Jun 2020 02:01:43 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b29c909e9fef1d56ec58cb008cf363dead738a814985e79695e537b0d72ea53`  
		Last Modified: Tue, 02 Jun 2020 02:19:40 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1432be465a87de431d75d8d1cf02c7e3a11afc2f17e74071f56a6992f9f79ec`  
		Last Modified: Tue, 02 Jun 2020 02:19:40 GMT  
		Size: 8.2 MB (8212445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4868624099c4b67147b2c3310067ca317b998e011da3445bd20b30e6ea4a1f83`  
		Last Modified: Tue, 02 Jun 2020 02:19:39 GMT  
		Size: 2.7 MB (2706327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7621f436be1cd0adc948c7f4c2b6047e4fdf87b7f63644e5b832ab43cbea5a38`  
		Last Modified: Tue, 02 Jun 2020 02:20:13 GMT  
		Size: 176.7 MB (176716012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7181db5ca0fa079aa4c35d3206d2913d4d544419ff434d64f403c84b766044`  
		Last Modified: Tue, 02 Jun 2020 02:19:39 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eead0c695ec3fd46a6b5f762603d74e1b7757c7fd0f547ecd1ce7f1ab5d3a5`  
		Last Modified: Tue, 02 Jun 2020 02:20:09 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.0.0-windowsservercore`

```console
$ docker pull caddy@sha256:e4dedf67fc59354c08ec74b75e15f126b2761a88a35522e86d1bb43ec182ab22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64
	-	windows version 10.0.14393.3750; amd64

### `caddy:2.0.0-windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:4846f66a1cfa0fa858f8ae2a6c348f14be435ca26312f365ed041203bb35f48a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2311249634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94450ec6f1472f8ab0cfd101f7f68644f92c8b2262f9ea2153fdc9a0798b3917`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Tue, 09 Jun 2020 22:33:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:02:29 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:03:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Jun 2020 18:03:16 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 10 Jun 2020 18:03:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('636bb25c9738400b480ca243a605da74988deb1bc856a1cabe7ee36511db0e048ec0a2688b1640d7b157bc239d437944e43500d91881c8acc7f2b8aa138945f9')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Jun 2020 18:03:56 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Jun 2020 18:03:56 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Jun 2020 18:03:57 GMT
VOLUME [c:/config]
# Wed, 10 Jun 2020 18:03:58 GMT
VOLUME [c:/data]
# Wed, 10 Jun 2020 18:03:59 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 10 Jun 2020 18:04:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Jun 2020 18:04:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Jun 2020 18:04:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Jun 2020 18:04:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Jun 2020 18:04:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Jun 2020 18:04:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Jun 2020 18:04:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Jun 2020 18:04:07 GMT
EXPOSE 80
# Wed, 10 Jun 2020 18:04:08 GMT
EXPOSE 443
# Wed, 10 Jun 2020 18:04:08 GMT
EXPOSE 2019
# Wed, 10 Jun 2020 18:04:31 GMT
RUN caddy version
# Wed, 10 Jun 2020 18:04:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f841c6a0c622cd36b5b2688011a224ac3e8e96273758f4a2804f2f3f099f267d`  
		Last Modified: Tue, 09 Jun 2020 23:17:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e676deb3766189ea2b008f69205017c9ee31a77f9c7001fb5a07fb2e2d4fbb0`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba576338ed5242ba3fb838ce5fa930abb61e22fc422ba46b260dbca773cb9`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 4.8 MB (4772911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82aa7b0db5bd44f058750b70c9ca192d7af8986578dd9900fa68f08a53d56d7`  
		Last Modified: Wed, 10 Jun 2020 18:09:46 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6f36d669bbd2a660d47e342775c1705e6b990b004cfb461b66aeb6d978fa60`  
		Last Modified: Wed, 10 Jun 2020 18:09:50 GMT  
		Size: 12.3 MB (12262241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4caa471f3ff12126859610d5fb7a1eee050fdcd24f4c26c840a49072698064`  
		Last Modified: Wed, 10 Jun 2020 18:09:46 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f92da22ed9f6eaba0eb6cb98ff0182e5bf96b672aa9a2a5fc004584af897f91`  
		Last Modified: Wed, 10 Jun 2020 18:09:45 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ca7d66806087b4fb8e9aba7aa8c8d913f6c00b136833ce130ad342601fbcce`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2f91baaa6ad75f37691004649e965eb02f770c8901034ec1d508ac0e198c9f`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490c3bc1055c4210b37fa961535859113aa2a9e83d5373f1edb7664fec3d44a4`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d6ca5a24db2b4dabbd352548aaabc3057e21b5b1d13a3e09ff8d5b4a9f99e4`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6b40d207638f35eb44e6d1c604c7939e68829fe4e04a1ca286eea436d3b3b5`  
		Last Modified: Wed, 10 Jun 2020 18:09:42 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d137f3abb4ef203c2caea5f8b50defc1384938cae41fab9c5f751193dd801e`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ff6d828fdc817dccd02e18fb68f60dfb77e5f91b61e4039622748fdacec123`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce68242ed36c05b1696a9aed8843408c0d3df159bdd08a6f89273aea8cf2a52`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8857e417a7cd480ddc26cd312eb34880b8e76040cd4f2ea589b21fbc5d54e274`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a31891b746d7cffa5744afba11ca2c1e207076488f863fe4cb519147cbc359`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e936bc871ff19fb19ebb325dc0b2a592fd9347488450d772e434000811f5d8c`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500e96dcc8873265379cfdace5e5c75b28080e5042969250c1656de746a3eb17`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7c3e99413b53ef84bebebfb04ec29d95aa84e3f0e040dc9cbf355afca92009`  
		Last Modified: Wed, 10 Jun 2020 18:09:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790f2340b769609f7c8716568b843cd0723c59c8dc64142f1e927d5536bd9f7c`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 278.2 KB (278231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e765bd24f285691b433b20a6296e67d067e6e2918c7e1cd2ad2bef1bbd356dfc`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.0.0-windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:64246e00b3c6726a42b20440c70003c72bc6e652f821982345b87928bc79cae5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756998229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb6c0b59ae11bc16763ab0732bf43ae0dead1bbded3284e54191f687f4a670e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:04:40 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:06:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Jun 2020 18:06:15 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 10 Jun 2020 18:07:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('636bb25c9738400b480ca243a605da74988deb1bc856a1cabe7ee36511db0e048ec0a2688b1640d7b157bc239d437944e43500d91881c8acc7f2b8aa138945f9')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Jun 2020 18:08:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Jun 2020 18:08:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Jun 2020 18:08:03 GMT
VOLUME [c:/config]
# Wed, 10 Jun 2020 18:08:04 GMT
VOLUME [c:/data]
# Wed, 10 Jun 2020 18:08:05 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 10 Jun 2020 18:08:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Jun 2020 18:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Jun 2020 18:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Jun 2020 18:08:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Jun 2020 18:08:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Jun 2020 18:08:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Jun 2020 18:08:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Jun 2020 18:08:12 GMT
EXPOSE 80
# Wed, 10 Jun 2020 18:08:13 GMT
EXPOSE 443
# Wed, 10 Jun 2020 18:08:14 GMT
EXPOSE 2019
# Wed, 10 Jun 2020 18:09:10 GMT
RUN caddy version
# Wed, 10 Jun 2020 18:09:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22985925139cd6a6e83b6eb5286a8a6e1053a5c6ddd9762f34deea2aa6bcaacc`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43c028d6768e901bc64b3edb7e2e5f72050d3ed78ea4e7337fe85725d250c15`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 5.4 MB (5404509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab96ccdd2dbffb13487e758409eaae25905b86a83e7b7a51a692c7ff18579b8d`  
		Last Modified: Wed, 10 Jun 2020 18:10:14 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aac2a7ea7e1f98bb6027b5090912006abeb6f367523aac337f6705ba4d7bb6b`  
		Last Modified: Wed, 10 Jun 2020 18:10:19 GMT  
		Size: 17.3 MB (17325836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7acf530d8fe0b1ea1f35f0e20ca267e447936a8edbae3889184d180b44c1a6`  
		Last Modified: Wed, 10 Jun 2020 18:10:13 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7609e5df44616b1f91e5434a43518cf253a69c406c062ef6b99035b20a437`  
		Last Modified: Wed, 10 Jun 2020 18:10:13 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1384cb066181208a5bb3be7023fe3f0b9cedf5483885cf330f7dcd95525302`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f2a49d3e0a25e1871a3dcb23fa333268062b4d027ae041e3bb5c0827dd0c2a`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5ec5b8bc911e1426e8c8dcc06a149b90edee45636d75da5b63e83fe91398a`  
		Last Modified: Wed, 10 Jun 2020 18:10:12 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dab68d41796a58e20ae80dc2528cfe6a2e71a04c8c88bb5595a6e0a5d7f7646`  
		Last Modified: Wed, 10 Jun 2020 18:10:10 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68da8c08840ea413933ac718a42b86738f90a6a5647e151252d4b5193ee40a8d`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946bc1b557fc88846697a1a1308c7af5ef52918f700f7dc8bd4c53e915c4a1a3`  
		Last Modified: Wed, 10 Jun 2020 18:10:09 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7ea127cbc59b2799852a077baa3bc9e46ad415abc4de6305396739a257a25e`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e77ea136bb911d1a64b32d1d139522e0e52ca1bc43b5d12aeeef7be91483d50`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a29c745913025b3a12451ab689a6186ec7756b5d99d0fa379a39ae81d510b0b`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4ae08e24e91168918350e7422b8f47200d09a7313216990ba6a672b5372280`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e219b4ef296fd92d145bf1f1a7b7d79e09c26a996daf350eb5ee70cbfeed02`  
		Last Modified: Wed, 10 Jun 2020 18:10:05 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc81bd4365ed96954980b554e769048c1e4cc97035385e22ee8364bd2856d4af`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec6f99a5c3e003e6dd16b75770a2762bb5de2737ffdd11b1c707f6aefce201a`  
		Last Modified: Wed, 10 Jun 2020 18:10:05 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26ba6de29355852954f97260ed4e96f1d30d7e675356cc21cac59feb841cf3e`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 248.4 KB (248359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef895a3d9501c41dd42a22a3e2a0458c59b35892005f5fb18b8937101a1fb50`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.0.0-windowsservercore-1809`

```console
$ docker pull caddy@sha256:8104954610b79ec4831237b7893ddd0da8ca6886fb2d4acc184412fcdca0b72c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `caddy:2.0.0-windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:4846f66a1cfa0fa858f8ae2a6c348f14be435ca26312f365ed041203bb35f48a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2311249634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94450ec6f1472f8ab0cfd101f7f68644f92c8b2262f9ea2153fdc9a0798b3917`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Tue, 09 Jun 2020 22:33:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:02:29 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:03:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Jun 2020 18:03:16 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 10 Jun 2020 18:03:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('636bb25c9738400b480ca243a605da74988deb1bc856a1cabe7ee36511db0e048ec0a2688b1640d7b157bc239d437944e43500d91881c8acc7f2b8aa138945f9')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Jun 2020 18:03:56 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Jun 2020 18:03:56 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Jun 2020 18:03:57 GMT
VOLUME [c:/config]
# Wed, 10 Jun 2020 18:03:58 GMT
VOLUME [c:/data]
# Wed, 10 Jun 2020 18:03:59 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 10 Jun 2020 18:04:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Jun 2020 18:04:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Jun 2020 18:04:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Jun 2020 18:04:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Jun 2020 18:04:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Jun 2020 18:04:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Jun 2020 18:04:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Jun 2020 18:04:07 GMT
EXPOSE 80
# Wed, 10 Jun 2020 18:04:08 GMT
EXPOSE 443
# Wed, 10 Jun 2020 18:04:08 GMT
EXPOSE 2019
# Wed, 10 Jun 2020 18:04:31 GMT
RUN caddy version
# Wed, 10 Jun 2020 18:04:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f841c6a0c622cd36b5b2688011a224ac3e8e96273758f4a2804f2f3f099f267d`  
		Last Modified: Tue, 09 Jun 2020 23:17:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e676deb3766189ea2b008f69205017c9ee31a77f9c7001fb5a07fb2e2d4fbb0`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba576338ed5242ba3fb838ce5fa930abb61e22fc422ba46b260dbca773cb9`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 4.8 MB (4772911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82aa7b0db5bd44f058750b70c9ca192d7af8986578dd9900fa68f08a53d56d7`  
		Last Modified: Wed, 10 Jun 2020 18:09:46 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6f36d669bbd2a660d47e342775c1705e6b990b004cfb461b66aeb6d978fa60`  
		Last Modified: Wed, 10 Jun 2020 18:09:50 GMT  
		Size: 12.3 MB (12262241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4caa471f3ff12126859610d5fb7a1eee050fdcd24f4c26c840a49072698064`  
		Last Modified: Wed, 10 Jun 2020 18:09:46 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f92da22ed9f6eaba0eb6cb98ff0182e5bf96b672aa9a2a5fc004584af897f91`  
		Last Modified: Wed, 10 Jun 2020 18:09:45 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ca7d66806087b4fb8e9aba7aa8c8d913f6c00b136833ce130ad342601fbcce`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2f91baaa6ad75f37691004649e965eb02f770c8901034ec1d508ac0e198c9f`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490c3bc1055c4210b37fa961535859113aa2a9e83d5373f1edb7664fec3d44a4`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d6ca5a24db2b4dabbd352548aaabc3057e21b5b1d13a3e09ff8d5b4a9f99e4`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6b40d207638f35eb44e6d1c604c7939e68829fe4e04a1ca286eea436d3b3b5`  
		Last Modified: Wed, 10 Jun 2020 18:09:42 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d137f3abb4ef203c2caea5f8b50defc1384938cae41fab9c5f751193dd801e`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ff6d828fdc817dccd02e18fb68f60dfb77e5f91b61e4039622748fdacec123`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce68242ed36c05b1696a9aed8843408c0d3df159bdd08a6f89273aea8cf2a52`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8857e417a7cd480ddc26cd312eb34880b8e76040cd4f2ea589b21fbc5d54e274`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a31891b746d7cffa5744afba11ca2c1e207076488f863fe4cb519147cbc359`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e936bc871ff19fb19ebb325dc0b2a592fd9347488450d772e434000811f5d8c`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500e96dcc8873265379cfdace5e5c75b28080e5042969250c1656de746a3eb17`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7c3e99413b53ef84bebebfb04ec29d95aa84e3f0e040dc9cbf355afca92009`  
		Last Modified: Wed, 10 Jun 2020 18:09:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790f2340b769609f7c8716568b843cd0723c59c8dc64142f1e927d5536bd9f7c`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 278.2 KB (278231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e765bd24f285691b433b20a6296e67d067e6e2918c7e1cd2ad2bef1bbd356dfc`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.0.0-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:c5e137c3575e37688a5ec6f3a628bde1fade7f6c99278fae9f865f24a52accc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `caddy:2.0.0-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:64246e00b3c6726a42b20440c70003c72bc6e652f821982345b87928bc79cae5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756998229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb6c0b59ae11bc16763ab0732bf43ae0dead1bbded3284e54191f687f4a670e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:04:40 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:06:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Jun 2020 18:06:15 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 10 Jun 2020 18:07:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('636bb25c9738400b480ca243a605da74988deb1bc856a1cabe7ee36511db0e048ec0a2688b1640d7b157bc239d437944e43500d91881c8acc7f2b8aa138945f9')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Jun 2020 18:08:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Jun 2020 18:08:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Jun 2020 18:08:03 GMT
VOLUME [c:/config]
# Wed, 10 Jun 2020 18:08:04 GMT
VOLUME [c:/data]
# Wed, 10 Jun 2020 18:08:05 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 10 Jun 2020 18:08:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Jun 2020 18:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Jun 2020 18:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Jun 2020 18:08:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Jun 2020 18:08:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Jun 2020 18:08:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Jun 2020 18:08:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Jun 2020 18:08:12 GMT
EXPOSE 80
# Wed, 10 Jun 2020 18:08:13 GMT
EXPOSE 443
# Wed, 10 Jun 2020 18:08:14 GMT
EXPOSE 2019
# Wed, 10 Jun 2020 18:09:10 GMT
RUN caddy version
# Wed, 10 Jun 2020 18:09:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22985925139cd6a6e83b6eb5286a8a6e1053a5c6ddd9762f34deea2aa6bcaacc`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43c028d6768e901bc64b3edb7e2e5f72050d3ed78ea4e7337fe85725d250c15`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 5.4 MB (5404509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab96ccdd2dbffb13487e758409eaae25905b86a83e7b7a51a692c7ff18579b8d`  
		Last Modified: Wed, 10 Jun 2020 18:10:14 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aac2a7ea7e1f98bb6027b5090912006abeb6f367523aac337f6705ba4d7bb6b`  
		Last Modified: Wed, 10 Jun 2020 18:10:19 GMT  
		Size: 17.3 MB (17325836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7acf530d8fe0b1ea1f35f0e20ca267e447936a8edbae3889184d180b44c1a6`  
		Last Modified: Wed, 10 Jun 2020 18:10:13 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7609e5df44616b1f91e5434a43518cf253a69c406c062ef6b99035b20a437`  
		Last Modified: Wed, 10 Jun 2020 18:10:13 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1384cb066181208a5bb3be7023fe3f0b9cedf5483885cf330f7dcd95525302`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f2a49d3e0a25e1871a3dcb23fa333268062b4d027ae041e3bb5c0827dd0c2a`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5ec5b8bc911e1426e8c8dcc06a149b90edee45636d75da5b63e83fe91398a`  
		Last Modified: Wed, 10 Jun 2020 18:10:12 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dab68d41796a58e20ae80dc2528cfe6a2e71a04c8c88bb5595a6e0a5d7f7646`  
		Last Modified: Wed, 10 Jun 2020 18:10:10 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68da8c08840ea413933ac718a42b86738f90a6a5647e151252d4b5193ee40a8d`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946bc1b557fc88846697a1a1308c7af5ef52918f700f7dc8bd4c53e915c4a1a3`  
		Last Modified: Wed, 10 Jun 2020 18:10:09 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7ea127cbc59b2799852a077baa3bc9e46ad415abc4de6305396739a257a25e`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e77ea136bb911d1a64b32d1d139522e0e52ca1bc43b5d12aeeef7be91483d50`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a29c745913025b3a12451ab689a6186ec7756b5d99d0fa379a39ae81d510b0b`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4ae08e24e91168918350e7422b8f47200d09a7313216990ba6a672b5372280`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e219b4ef296fd92d145bf1f1a7b7d79e09c26a996daf350eb5ee70cbfeed02`  
		Last Modified: Wed, 10 Jun 2020 18:10:05 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc81bd4365ed96954980b554e769048c1e4cc97035385e22ee8364bd2856d4af`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec6f99a5c3e003e6dd16b75770a2762bb5de2737ffdd11b1c707f6aefce201a`  
		Last Modified: Wed, 10 Jun 2020 18:10:05 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26ba6de29355852954f97260ed4e96f1d30d7e675356cc21cac59feb841cf3e`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 248.4 KB (248359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef895a3d9501c41dd42a22a3e2a0458c59b35892005f5fb18b8937101a1fb50`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.0-beta.1`

```console
$ docker pull caddy@sha256:ff5d5f0126a2c5024f8fd5acd5217aa9a16fb08935f92126cffe8d25d519b23c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1282; amd64
	-	windows version 10.0.14393.3750; amd64

### `caddy:2.1.0-beta.1` - linux; amd64

```console
$ docker pull caddy@sha256:eaf071c90be849e4f0bf52d6118060a03aaec95da2a3d2fd018ed3a64e96d343
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16327923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e236a41a3591bd0310c119e9d4b407366f1862fb3abbcecb04ce807c116eaf5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:21:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 21:21:16 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 21:21:18 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 15 Jun 2020 21:21:18 GMT
ENV CADDY_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 21:21:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='88c141648d1b2f77a3176d36d7448e0409118fa39572dd46f853928033fddc9c593d02101d6923f20acefc8fd7ac701d84dc4276dbc42c3a6c1b8c1e9d26eebd' ;; 		armhf)   binArch='armv6'; checksum='af8bb19b0c72d0c6e2cf748a62046102cf52c82454bbd32f1c75404188145da585dd2f9cc3848bf99ad9ebb94f546b56b1d2a4db73bdcf4c262e0441cf55af5d' ;; 		armv7)   binArch='armv7'; checksum='ba1a123791c531d69f677fbd2652429f37eb0298491fd25ae23629a12bec6ad4a33b5e6d25069ccd98773c3036b599054ccf152bf56e791a7435c1592042ca22' ;; 		aarch64) binArch='arm64'; checksum='e425bd8b3514990de3bfed50375dac6abef9308a3e49d0098b2151b3b5dd74cb1e545e0b15bc2b57b21941a1d8cb4e1dcb1a50c93ea3c3e60d14a30394059b34' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='90cdeda18af8634fdfcaab60d58f246d88756ebae5c716a93e3c09ae266d86812b9e258f894447a3126dd6b37a8e19d5ea7fe0e33543d2a6f2e41bc947de0fd4' ;; 		s390x)   binArch='s390x'; checksum='db3eea7f378400ff4e12baca105997b8ff5cc4725fc901027e80d6bd4ce127fba7debefd52bbd5e40b54db30d6b2ca96d1221e4179044876ae39cf27e3bdf475' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0-beta.1/caddy_2.1.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:19:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:19:33 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:19:33 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:19:33 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:19:33 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:19:34 GMT
LABEL org.opencontainers.image.version=v2.1.0-beta.1
# Fri, 26 Jun 2020 01:19:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:19:34 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:19:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:19:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:19:34 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:19:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:19:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:19:35 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:19:35 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:19:35 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:19:36 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:19:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed237faf7b90187b720d5e863fb021a1ca678304744dad14ff8ad6434e4e1da`  
		Last Modified: Mon, 15 Jun 2020 21:22:02 GMT  
		Size: 300.0 KB (299981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e49a2f7ba4b80caa31bb2874b39f9c4bbb447708f3a0e07ff43892744e63a4`  
		Last Modified: Mon, 15 Jun 2020 21:22:02 GMT  
		Size: 5.8 KB (5767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a1674670cc1ac29d639ea74cdfd32b9ecbbed97d75a865987a4d368f47a5aa`  
		Last Modified: Mon, 15 Jun 2020 21:22:05 GMT  
		Size: 13.2 MB (13224478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db22687770ffb51ac7ea9853be5af0336b15be293c0885d0acb2cf047df6103f`  
		Last Modified: Fri, 26 Jun 2020 01:20:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.0-beta.1` - linux; arm variant v6

```console
$ docker pull caddy@sha256:50e0d158d394e4e3b20ecb22cd6dec5e429e3ea5f34afc149d41cd6b996077b8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.5 MB (15491201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e0c98fe095e2f8fcd1a77ed0e5fdf2a7995c8296b5d161ea90dbd9692c5e66`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:52:06 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 20:52:07 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 20:52:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 15 Jun 2020 20:52:11 GMT
ENV CADDY_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 20:52:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='88c141648d1b2f77a3176d36d7448e0409118fa39572dd46f853928033fddc9c593d02101d6923f20acefc8fd7ac701d84dc4276dbc42c3a6c1b8c1e9d26eebd' ;; 		armhf)   binArch='armv6'; checksum='af8bb19b0c72d0c6e2cf748a62046102cf52c82454bbd32f1c75404188145da585dd2f9cc3848bf99ad9ebb94f546b56b1d2a4db73bdcf4c262e0441cf55af5d' ;; 		armv7)   binArch='armv7'; checksum='ba1a123791c531d69f677fbd2652429f37eb0298491fd25ae23629a12bec6ad4a33b5e6d25069ccd98773c3036b599054ccf152bf56e791a7435c1592042ca22' ;; 		aarch64) binArch='arm64'; checksum='e425bd8b3514990de3bfed50375dac6abef9308a3e49d0098b2151b3b5dd74cb1e545e0b15bc2b57b21941a1d8cb4e1dcb1a50c93ea3c3e60d14a30394059b34' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='90cdeda18af8634fdfcaab60d58f246d88756ebae5c716a93e3c09ae266d86812b9e258f894447a3126dd6b37a8e19d5ea7fe0e33543d2a6f2e41bc947de0fd4' ;; 		s390x)   binArch='s390x'; checksum='db3eea7f378400ff4e12baca105997b8ff5cc4725fc901027e80d6bd4ce127fba7debefd52bbd5e40b54db30d6b2ca96d1221e4179044876ae39cf27e3bdf475' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0-beta.1/caddy_2.1.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 00:50:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 00:50:23 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 00:50:24 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 00:50:24 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 00:50:25 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 00:50:25 GMT
LABEL org.opencontainers.image.version=v2.1.0-beta.1
# Fri, 26 Jun 2020 00:50:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 00:50:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 00:50:27 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 00:50:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 00:50:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 00:50:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 00:50:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 00:50:31 GMT
EXPOSE 80
# Fri, 26 Jun 2020 00:50:31 GMT
EXPOSE 443
# Fri, 26 Jun 2020 00:50:32 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 00:50:32 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 00:50:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2a5a47b7ff29cc165cee9824ba874fa6cb56d737ce18f841fc3ed5e937cb75`  
		Last Modified: Mon, 15 Jun 2020 20:54:38 GMT  
		Size: 300.1 KB (300144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3243ce9c25dc28a597c553cc7f0d4816c4b75789e4ebc37225ac58d5bd078995`  
		Last Modified: Mon, 15 Jun 2020 20:54:38 GMT  
		Size: 5.8 KB (5842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732c51547d0432a08f1326dd9caf4c8ab5381227e7c28382002707d7fde62011`  
		Last Modified: Mon, 15 Jun 2020 20:54:43 GMT  
		Size: 12.6 MB (12581775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef648a9eebd2584542a6d9950c63fb8da0fa93c707f1e774e1fcf34d9b779a2`  
		Last Modified: Fri, 26 Jun 2020 00:51:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.0-beta.1` - linux; arm variant v7

```console
$ docker pull caddy@sha256:4c0882eda2e74ae5ec7a74f9b89c2f62e79019a5ed7959cc311193b049884769
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15267428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a552395a8eb3cd6fd933cb97457a6dc8119637a7e3c6f13e7d692f7c81548e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:59:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 21:00:00 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 21:00:03 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 15 Jun 2020 21:00:04 GMT
ENV CADDY_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 21:00:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='88c141648d1b2f77a3176d36d7448e0409118fa39572dd46f853928033fddc9c593d02101d6923f20acefc8fd7ac701d84dc4276dbc42c3a6c1b8c1e9d26eebd' ;; 		armhf)   binArch='armv6'; checksum='af8bb19b0c72d0c6e2cf748a62046102cf52c82454bbd32f1c75404188145da585dd2f9cc3848bf99ad9ebb94f546b56b1d2a4db73bdcf4c262e0441cf55af5d' ;; 		armv7)   binArch='armv7'; checksum='ba1a123791c531d69f677fbd2652429f37eb0298491fd25ae23629a12bec6ad4a33b5e6d25069ccd98773c3036b599054ccf152bf56e791a7435c1592042ca22' ;; 		aarch64) binArch='arm64'; checksum='e425bd8b3514990de3bfed50375dac6abef9308a3e49d0098b2151b3b5dd74cb1e545e0b15bc2b57b21941a1d8cb4e1dcb1a50c93ea3c3e60d14a30394059b34' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='90cdeda18af8634fdfcaab60d58f246d88756ebae5c716a93e3c09ae266d86812b9e258f894447a3126dd6b37a8e19d5ea7fe0e33543d2a6f2e41bc947de0fd4' ;; 		s390x)   binArch='s390x'; checksum='db3eea7f378400ff4e12baca105997b8ff5cc4725fc901027e80d6bd4ce127fba7debefd52bbd5e40b54db30d6b2ca96d1221e4179044876ae39cf27e3bdf475' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0-beta.1/caddy_2.1.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 00:59:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 00:59:08 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 00:59:09 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 00:59:09 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 00:59:10 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 00:59:10 GMT
LABEL org.opencontainers.image.version=v2.1.0-beta.1
# Fri, 26 Jun 2020 00:59:11 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 00:59:12 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 00:59:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 00:59:13 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 00:59:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 00:59:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 00:59:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 00:59:16 GMT
EXPOSE 80
# Fri, 26 Jun 2020 00:59:17 GMT
EXPOSE 443
# Fri, 26 Jun 2020 00:59:17 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 00:59:18 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 00:59:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2aa34f01f2f9112772fdaebe7083b7dcdb4313768e0d6533a3e5b99597c98d`  
		Last Modified: Mon, 15 Jun 2020 21:02:12 GMT  
		Size: 299.2 KB (299237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b107a7bf1560d80dcded532795715f77765cf1a3d9464665d42acab82d366e`  
		Last Modified: Mon, 15 Jun 2020 21:02:12 GMT  
		Size: 5.8 KB (5845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967915987b3a992d9002998ed87607ec38d821ddfa699e1977947d701c7be51b`  
		Last Modified: Mon, 15 Jun 2020 21:02:16 GMT  
		Size: 12.6 MB (12555429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e53f8fadc72987278ef5b53319e6078db333123b5bce64d56f63023f6136097`  
		Last Modified: Fri, 26 Jun 2020 01:00:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.0-beta.1` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f9e022c998b81c59c7944995985f06882f5bb9e2a7b7aad877faf99bf31b535d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15175624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b41f0fd0f628ee5d840ac13bcded95b9e990d6b2f3f3da48bd78b23ef0e28740`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:42:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 20:42:33 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 20:42:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 15 Jun 2020 20:42:36 GMT
ENV CADDY_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 20:42:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='88c141648d1b2f77a3176d36d7448e0409118fa39572dd46f853928033fddc9c593d02101d6923f20acefc8fd7ac701d84dc4276dbc42c3a6c1b8c1e9d26eebd' ;; 		armhf)   binArch='armv6'; checksum='af8bb19b0c72d0c6e2cf748a62046102cf52c82454bbd32f1c75404188145da585dd2f9cc3848bf99ad9ebb94f546b56b1d2a4db73bdcf4c262e0441cf55af5d' ;; 		armv7)   binArch='armv7'; checksum='ba1a123791c531d69f677fbd2652429f37eb0298491fd25ae23629a12bec6ad4a33b5e6d25069ccd98773c3036b599054ccf152bf56e791a7435c1592042ca22' ;; 		aarch64) binArch='arm64'; checksum='e425bd8b3514990de3bfed50375dac6abef9308a3e49d0098b2151b3b5dd74cb1e545e0b15bc2b57b21941a1d8cb4e1dcb1a50c93ea3c3e60d14a30394059b34' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='90cdeda18af8634fdfcaab60d58f246d88756ebae5c716a93e3c09ae266d86812b9e258f894447a3126dd6b37a8e19d5ea7fe0e33543d2a6f2e41bc947de0fd4' ;; 		s390x)   binArch='s390x'; checksum='db3eea7f378400ff4e12baca105997b8ff5cc4725fc901027e80d6bd4ce127fba7debefd52bbd5e40b54db30d6b2ca96d1221e4179044876ae39cf27e3bdf475' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0-beta.1/caddy_2.1.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:39:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:39:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:39:42 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:39:43 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:39:44 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:39:45 GMT
LABEL org.opencontainers.image.version=v2.1.0-beta.1
# Fri, 26 Jun 2020 01:39:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:39:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:39:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:39:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:39:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:39:49 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:39:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:39:50 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:39:51 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:39:52 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:39:52 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:39:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f33282aee1a51127f669c7222e26bd0d5107b28d68819a6ead7f68076a73dc`  
		Last Modified: Mon, 15 Jun 2020 20:44:05 GMT  
		Size: 300.4 KB (300393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b85f4621f67650b74dc2db70b30f9593bc6695d3e91ff3899b3ee7c34cffc04`  
		Last Modified: Mon, 15 Jun 2020 20:44:04 GMT  
		Size: 5.8 KB (5846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c4b107fc4b1eaed154176164b59c74fcd6457e880f0c6546faf2d34d149b78`  
		Last Modified: Mon, 15 Jun 2020 20:44:08 GMT  
		Size: 12.2 MB (12161267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a68a56ab072aff607c272b535b031020ab0600c0fbfc38de1be683f93bae808`  
		Last Modified: Fri, 26 Jun 2020 01:40:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.0-beta.1` - linux; ppc64le

```console
$ docker pull caddy@sha256:e3dd7f9b270d127cfa2f780d19070debaa663de1f41504f2a8b9ff0f2412811a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.0 MB (15042389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e5712224a99bd347ac07739417c73a343c4008f5b89e1caab4f9a84c1b1fe2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:19:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 21:19:13 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 21:19:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 15 Jun 2020 21:19:21 GMT
ENV CADDY_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 21:19:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='88c141648d1b2f77a3176d36d7448e0409118fa39572dd46f853928033fddc9c593d02101d6923f20acefc8fd7ac701d84dc4276dbc42c3a6c1b8c1e9d26eebd' ;; 		armhf)   binArch='armv6'; checksum='af8bb19b0c72d0c6e2cf748a62046102cf52c82454bbd32f1c75404188145da585dd2f9cc3848bf99ad9ebb94f546b56b1d2a4db73bdcf4c262e0441cf55af5d' ;; 		armv7)   binArch='armv7'; checksum='ba1a123791c531d69f677fbd2652429f37eb0298491fd25ae23629a12bec6ad4a33b5e6d25069ccd98773c3036b599054ccf152bf56e791a7435c1592042ca22' ;; 		aarch64) binArch='arm64'; checksum='e425bd8b3514990de3bfed50375dac6abef9308a3e49d0098b2151b3b5dd74cb1e545e0b15bc2b57b21941a1d8cb4e1dcb1a50c93ea3c3e60d14a30394059b34' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='90cdeda18af8634fdfcaab60d58f246d88756ebae5c716a93e3c09ae266d86812b9e258f894447a3126dd6b37a8e19d5ea7fe0e33543d2a6f2e41bc947de0fd4' ;; 		s390x)   binArch='s390x'; checksum='db3eea7f378400ff4e12baca105997b8ff5cc4725fc901027e80d6bd4ce127fba7debefd52bbd5e40b54db30d6b2ca96d1221e4179044876ae39cf27e3bdf475' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0-beta.1/caddy_2.1.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:16:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:16:41 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:16:45 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:16:48 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:16:53 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:16:56 GMT
LABEL org.opencontainers.image.version=v2.1.0-beta.1
# Fri, 26 Jun 2020 01:17:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:17:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:17:14 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:17:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:17:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:17:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:17:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:17:39 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:17:42 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:17:45 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:17:50 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:17:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b28df4c8a155654ad705e08f459bd177acc1005644ce2173ac62e954d6d4d2`  
		Last Modified: Mon, 15 Jun 2020 21:24:35 GMT  
		Size: 302.4 KB (302369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2288431c86a795754eb4d3a678e778c534a14e9243aea01a7cf9feff8d8e4e`  
		Last Modified: Mon, 15 Jun 2020 21:24:35 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7209a53971081ce93e14e316f2ba60b8055bffd05a4d99e637161191d7fa6d6`  
		Last Modified: Mon, 15 Jun 2020 21:24:38 GMT  
		Size: 11.9 MB (11928820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04afaf9f3075f38bac61579a0d3a8946b65109dffe0534fb7904c6e4d5acd95c`  
		Last Modified: Fri, 26 Jun 2020 01:19:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.0-beta.1` - linux; s390x

```console
$ docker pull caddy@sha256:96538f54c12919a30d26b81cba65396f45944702709b9fd79bd64f99f33c3ebe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15881784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0004092087cf1595e2c57354a8a3c7f1535d5881f2f57e730216ce5c6a952099`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:43:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 20:43:15 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 20:43:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 15 Jun 2020 20:43:16 GMT
ENV CADDY_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 20:43:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='88c141648d1b2f77a3176d36d7448e0409118fa39572dd46f853928033fddc9c593d02101d6923f20acefc8fd7ac701d84dc4276dbc42c3a6c1b8c1e9d26eebd' ;; 		armhf)   binArch='armv6'; checksum='af8bb19b0c72d0c6e2cf748a62046102cf52c82454bbd32f1c75404188145da585dd2f9cc3848bf99ad9ebb94f546b56b1d2a4db73bdcf4c262e0441cf55af5d' ;; 		armv7)   binArch='armv7'; checksum='ba1a123791c531d69f677fbd2652429f37eb0298491fd25ae23629a12bec6ad4a33b5e6d25069ccd98773c3036b599054ccf152bf56e791a7435c1592042ca22' ;; 		aarch64) binArch='arm64'; checksum='e425bd8b3514990de3bfed50375dac6abef9308a3e49d0098b2151b3b5dd74cb1e545e0b15bc2b57b21941a1d8cb4e1dcb1a50c93ea3c3e60d14a30394059b34' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='90cdeda18af8634fdfcaab60d58f246d88756ebae5c716a93e3c09ae266d86812b9e258f894447a3126dd6b37a8e19d5ea7fe0e33543d2a6f2e41bc947de0fd4' ;; 		s390x)   binArch='s390x'; checksum='db3eea7f378400ff4e12baca105997b8ff5cc4725fc901027e80d6bd4ce127fba7debefd52bbd5e40b54db30d6b2ca96d1221e4179044876ae39cf27e3bdf475' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0-beta.1/caddy_2.1.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:41:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:41:30 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:41:30 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:41:30 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:41:31 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:41:31 GMT
LABEL org.opencontainers.image.version=v2.1.0-beta.1
# Fri, 26 Jun 2020 01:41:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:41:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:41:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:41:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:41:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:41:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:41:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:41:33 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:41:33 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:41:34 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:41:34 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:41:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc47bdcaea173dfb029a09265c41846030477dc696b22fed52acad2b2078bb7`  
		Last Modified: Mon, 15 Jun 2020 20:44:21 GMT  
		Size: 300.5 KB (300524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf084f3ceb3b3b1196400fa251cc45e01de7ece41b7605bb40ae5178d849b47d`  
		Last Modified: Mon, 15 Jun 2020 20:44:26 GMT  
		Size: 5.8 KB (5841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d34155d08428f26786712fcdbc9c270779e8d7520b8d09a209dfb3de4b70780`  
		Last Modified: Mon, 15 Jun 2020 20:44:23 GMT  
		Size: 13.0 MB (13009076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00d36bbc65cb4aa4293ffd2284daf453dd6385b2574f156823f0ff8e3751b8a`  
		Last Modified: Fri, 26 Jun 2020 01:42:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.0-beta.1` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:637c6c607ab7ca56a590bb0ae86295010557a84dbdf3dc99fbf4cc591eb1e5bb
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2312521998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20942c19259da51445c3e6c4b6ddc9fedf01b3fb05b07099004d0857bb395936`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Tue, 09 Jun 2020 22:33:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:02:29 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:03:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 15 Jun 2020 21:15:46 GMT
ENV CADDY_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 21:16:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.0-beta.1/caddy_2.1.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8c87f1d5a4f94a5532fdf2b2f63890f4e88e19b8cb409b11cec5a34be263d42ffc17b76eb38bfff7f27b27e9e932f8c15783e96cce98448013fcc516dacf1d0b')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 15 Jun 2020 21:16:22 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 15 Jun 2020 21:16:23 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 15 Jun 2020 21:16:24 GMT
VOLUME [c:/config]
# Mon, 15 Jun 2020 21:16:25 GMT
VOLUME [c:/data]
# Mon, 15 Jun 2020 21:16:26 GMT
LABEL org.opencontainers.image.version=v2.1.0-beta.1
# Mon, 15 Jun 2020 21:16:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 15 Jun 2020 21:16:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 15 Jun 2020 21:16:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 15 Jun 2020 21:16:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 15 Jun 2020 21:16:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 15 Jun 2020 21:16:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 15 Jun 2020 21:16:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 15 Jun 2020 21:16:33 GMT
EXPOSE 80
# Mon, 15 Jun 2020 21:16:34 GMT
EXPOSE 443
# Mon, 15 Jun 2020 21:16:35 GMT
EXPOSE 2019
# Mon, 15 Jun 2020 21:16:52 GMT
RUN caddy version
# Mon, 15 Jun 2020 21:16:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f841c6a0c622cd36b5b2688011a224ac3e8e96273758f4a2804f2f3f099f267d`  
		Last Modified: Tue, 09 Jun 2020 23:17:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e676deb3766189ea2b008f69205017c9ee31a77f9c7001fb5a07fb2e2d4fbb0`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba576338ed5242ba3fb838ce5fa930abb61e22fc422ba46b260dbca773cb9`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 4.8 MB (4772911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e3e4a9deb067045cd0c24b717ffc454d12b87b5f184498f199a4500fcc39ea`  
		Last Modified: Mon, 15 Jun 2020 21:20:18 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed77eefd9fab412b04cfe83746a7d782cf06fb7e26076961fdf01629bf3178b`  
		Last Modified: Mon, 15 Jun 2020 21:20:22 GMT  
		Size: 13.5 MB (13514542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db36924581cd6c03fbc76c1f2536196031f85d7f0632d8ba14ec83dc16e8ca5d`  
		Last Modified: Mon, 15 Jun 2020 21:20:18 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ac6eae76c670d7ba4b0b7c71ec62e7b2985130093837a063cda8cfb6fdb014`  
		Last Modified: Mon, 15 Jun 2020 21:20:17 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ced9b1ae0ee4451dff19cfd6cbc3518ca9fd63b08a3b298846336eec9a92db7`  
		Last Modified: Mon, 15 Jun 2020 21:20:16 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ef23d879b1c5fa266b603fa2ec1ab8f448c51688b2bbbd026a3cdd61e3239`  
		Last Modified: Mon, 15 Jun 2020 21:20:16 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77ba47e8b13bad632b11a83940626505edd75e01c8de4dc24855721e9f48d3f`  
		Last Modified: Mon, 15 Jun 2020 21:20:15 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ed31c38dafc3492acdf4272645ef61c97c18c553777d342c317e70773b9c76`  
		Last Modified: Mon, 15 Jun 2020 21:20:16 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2365dc868a8422756f8ae8f40d061c1b09dc409bc982b25cc8c9c23bce7837d`  
		Last Modified: Mon, 15 Jun 2020 21:20:15 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af8bc08af2758e7f6a18b9a9ec78cec98975121415b3575c33539fc2033d390`  
		Last Modified: Mon, 15 Jun 2020 21:20:14 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fde35a97b738c5b8b6eec76486e86738045f0f6d27863f7d0991c034210bcef`  
		Last Modified: Mon, 15 Jun 2020 21:20:13 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ab21673c985472de4bead86534ff719ac16032d2bb4588b5edd8eb2db504de`  
		Last Modified: Mon, 15 Jun 2020 21:20:13 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e2e941122550083392e2d1271f6c18c3a8dc0872c51727b783a19231bfef33`  
		Last Modified: Mon, 15 Jun 2020 21:20:12 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5f95d02c4e9e331b8eb2f59baa2eab2cb29219fef1b0b235062833c7879ccd`  
		Last Modified: Mon, 15 Jun 2020 21:20:13 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe8f7ad33f8d57d12301a1812d501e197b329152f2d55b99e8863c3ae3a10e9`  
		Last Modified: Mon, 15 Jun 2020 21:20:10 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aea5478316d530d122395a14076ab5093a59eadd6ab6be4c99f9c3185327248`  
		Last Modified: Mon, 15 Jun 2020 21:20:10 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb3d364dd289b26eeda93175144e40522e3447db2f70987a5ca69e9972e0b21`  
		Last Modified: Mon, 15 Jun 2020 21:20:10 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7261589e0957fb07bbb94cd24f9650b976302660138ea35d0b8b47ddf75cef7`  
		Last Modified: Mon, 15 Jun 2020 21:20:10 GMT  
		Size: 298.5 KB (298457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e977c97431a52c4b2c351a5e8cf85767c61a968cec76dbcfbbeca0e4374fa4`  
		Last Modified: Mon, 15 Jun 2020 21:20:10 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.0-beta.1` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:6201786c3d7a42cac215b169cdfe88681e266ee7d6d390988a8f68fb83bea620
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758217462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a25a49441e73129c3e36057198e872fcf40750007748ea8e2816815dda841ef`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:04:40 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:06:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 15 Jun 2020 21:17:09 GMT
ENV CADDY_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 21:18:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.0-beta.1/caddy_2.1.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8c87f1d5a4f94a5532fdf2b2f63890f4e88e19b8cb409b11cec5a34be263d42ffc17b76eb38bfff7f27b27e9e932f8c15783e96cce98448013fcc516dacf1d0b')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 15 Jun 2020 21:18:35 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 15 Jun 2020 21:18:36 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 15 Jun 2020 21:18:37 GMT
VOLUME [c:/config]
# Mon, 15 Jun 2020 21:18:38 GMT
VOLUME [c:/data]
# Mon, 15 Jun 2020 21:18:39 GMT
LABEL org.opencontainers.image.version=v2.1.0-beta.1
# Mon, 15 Jun 2020 21:18:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 15 Jun 2020 21:18:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 15 Jun 2020 21:18:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 15 Jun 2020 21:18:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 15 Jun 2020 21:18:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 15 Jun 2020 21:18:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 15 Jun 2020 21:18:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 15 Jun 2020 21:18:46 GMT
EXPOSE 80
# Mon, 15 Jun 2020 21:18:47 GMT
EXPOSE 443
# Mon, 15 Jun 2020 21:18:48 GMT
EXPOSE 2019
# Mon, 15 Jun 2020 21:19:29 GMT
RUN caddy version
# Mon, 15 Jun 2020 21:19:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22985925139cd6a6e83b6eb5286a8a6e1053a5c6ddd9762f34deea2aa6bcaacc`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43c028d6768e901bc64b3edb7e2e5f72050d3ed78ea4e7337fe85725d250c15`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 5.4 MB (5404509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c22ecccbfcd030d10a64153d97b05414a12a6e4391fc7727f205d250f82d29b`  
		Last Modified: Mon, 15 Jun 2020 21:20:43 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043abd7aae9c81cfb27da0a6048b753f5d13342428c4351210380b2ef34f1797`  
		Last Modified: Mon, 15 Jun 2020 21:20:47 GMT  
		Size: 18.5 MB (18548536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a94d03da17df89277ff8583569c9cf95187fd10568cb0b9f44bc6dd23b4ab9`  
		Last Modified: Mon, 15 Jun 2020 21:20:42 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054637bf72793f6d35a09b82643d312e8350a19c05a84badcb60eed66e05f9e3`  
		Last Modified: Mon, 15 Jun 2020 21:20:41 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab0ca47076e559a31592d3daac2783f528bce5460203b265a1bf8161d6f1178`  
		Last Modified: Mon, 15 Jun 2020 21:20:40 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b248096abce77da76924f7399bc6942dc8b9e2f025f871c57433971441a246`  
		Last Modified: Mon, 15 Jun 2020 21:20:40 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81455e02f083bd2146af80776e9cc46b0aafaae7593b24b520577b6ab8031ce4`  
		Last Modified: Mon, 15 Jun 2020 21:20:40 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0150fc8e2c153b78027f67e85f6a2bac3bd57be7eae71251c36443cab1eaff40`  
		Last Modified: Mon, 15 Jun 2020 21:20:40 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578d4cdda9428605fe5933f3e16e4c40d18d4f15f486c2bde43f5ad12a84405f`  
		Last Modified: Mon, 15 Jun 2020 21:20:39 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213fe93c05e7b9c8152020cc11bb769e0d0a5670fcec11f5e10054379ade4b91`  
		Last Modified: Mon, 15 Jun 2020 21:20:37 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bef0c8ef4c5321e14235137d7b40bd580a931189d447c53e4902b4b0bfdb4d`  
		Last Modified: Mon, 15 Jun 2020 21:20:37 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d954a308c87819fe2e19d1bf5ef936453ab1e92b386b0cafaac37507e52f4eea`  
		Last Modified: Mon, 15 Jun 2020 21:20:37 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2335b8f54fc31963d6843047a2bdd2a234ca726e9061869551369f6623d7c60a`  
		Last Modified: Mon, 15 Jun 2020 21:20:37 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d17720617ae9cf3b603669655085a68016364f67a23446289006a68f20e13fd`  
		Last Modified: Mon, 15 Jun 2020 21:20:37 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1105a52fd3f7d8ccfab34c3a84c52c70ef4916f12c188775357d544344b495e5`  
		Last Modified: Mon, 15 Jun 2020 21:20:34 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a02dd52c835be30792e049cff4d4bbc6beb11a71718b78f5f20bc8cf474308b`  
		Last Modified: Mon, 15 Jun 2020 21:20:34 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:158c3526d0ace10490df86298bd0fd6a8ee0b0539735e2bf19cb99f93e283bd6`  
		Last Modified: Mon, 15 Jun 2020 21:20:34 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0963f5b2777be491c70973c436712d0c0a0e851be8d75a1a5443bdc07d5b7d9`  
		Last Modified: Mon, 15 Jun 2020 21:20:35 GMT  
		Size: 244.9 KB (244942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d861ed92a97bfd175d80668a81b3da55db1f527c5f453b65182240af0bed640`  
		Last Modified: Mon, 15 Jun 2020 21:20:34 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.0-beta.1-alpine`

```console
$ docker pull caddy@sha256:a5176244825a31176d337ac0a96a4163f6e7f8bbd2f68d8fb1bed14d64704553
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.1.0-beta.1-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:eaf071c90be849e4f0bf52d6118060a03aaec95da2a3d2fd018ed3a64e96d343
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16327923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e236a41a3591bd0310c119e9d4b407366f1862fb3abbcecb04ce807c116eaf5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:21:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 21:21:16 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 21:21:18 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 15 Jun 2020 21:21:18 GMT
ENV CADDY_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 21:21:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='88c141648d1b2f77a3176d36d7448e0409118fa39572dd46f853928033fddc9c593d02101d6923f20acefc8fd7ac701d84dc4276dbc42c3a6c1b8c1e9d26eebd' ;; 		armhf)   binArch='armv6'; checksum='af8bb19b0c72d0c6e2cf748a62046102cf52c82454bbd32f1c75404188145da585dd2f9cc3848bf99ad9ebb94f546b56b1d2a4db73bdcf4c262e0441cf55af5d' ;; 		armv7)   binArch='armv7'; checksum='ba1a123791c531d69f677fbd2652429f37eb0298491fd25ae23629a12bec6ad4a33b5e6d25069ccd98773c3036b599054ccf152bf56e791a7435c1592042ca22' ;; 		aarch64) binArch='arm64'; checksum='e425bd8b3514990de3bfed50375dac6abef9308a3e49d0098b2151b3b5dd74cb1e545e0b15bc2b57b21941a1d8cb4e1dcb1a50c93ea3c3e60d14a30394059b34' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='90cdeda18af8634fdfcaab60d58f246d88756ebae5c716a93e3c09ae266d86812b9e258f894447a3126dd6b37a8e19d5ea7fe0e33543d2a6f2e41bc947de0fd4' ;; 		s390x)   binArch='s390x'; checksum='db3eea7f378400ff4e12baca105997b8ff5cc4725fc901027e80d6bd4ce127fba7debefd52bbd5e40b54db30d6b2ca96d1221e4179044876ae39cf27e3bdf475' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0-beta.1/caddy_2.1.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:19:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:19:33 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:19:33 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:19:33 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:19:33 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:19:34 GMT
LABEL org.opencontainers.image.version=v2.1.0-beta.1
# Fri, 26 Jun 2020 01:19:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:19:34 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:19:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:19:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:19:34 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:19:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:19:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:19:35 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:19:35 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:19:35 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:19:36 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:19:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed237faf7b90187b720d5e863fb021a1ca678304744dad14ff8ad6434e4e1da`  
		Last Modified: Mon, 15 Jun 2020 21:22:02 GMT  
		Size: 300.0 KB (299981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e49a2f7ba4b80caa31bb2874b39f9c4bbb447708f3a0e07ff43892744e63a4`  
		Last Modified: Mon, 15 Jun 2020 21:22:02 GMT  
		Size: 5.8 KB (5767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a1674670cc1ac29d639ea74cdfd32b9ecbbed97d75a865987a4d368f47a5aa`  
		Last Modified: Mon, 15 Jun 2020 21:22:05 GMT  
		Size: 13.2 MB (13224478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db22687770ffb51ac7ea9853be5af0336b15be293c0885d0acb2cf047df6103f`  
		Last Modified: Fri, 26 Jun 2020 01:20:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.0-beta.1-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:50e0d158d394e4e3b20ecb22cd6dec5e429e3ea5f34afc149d41cd6b996077b8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.5 MB (15491201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e0c98fe095e2f8fcd1a77ed0e5fdf2a7995c8296b5d161ea90dbd9692c5e66`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:52:06 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 20:52:07 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 20:52:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 15 Jun 2020 20:52:11 GMT
ENV CADDY_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 20:52:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='88c141648d1b2f77a3176d36d7448e0409118fa39572dd46f853928033fddc9c593d02101d6923f20acefc8fd7ac701d84dc4276dbc42c3a6c1b8c1e9d26eebd' ;; 		armhf)   binArch='armv6'; checksum='af8bb19b0c72d0c6e2cf748a62046102cf52c82454bbd32f1c75404188145da585dd2f9cc3848bf99ad9ebb94f546b56b1d2a4db73bdcf4c262e0441cf55af5d' ;; 		armv7)   binArch='armv7'; checksum='ba1a123791c531d69f677fbd2652429f37eb0298491fd25ae23629a12bec6ad4a33b5e6d25069ccd98773c3036b599054ccf152bf56e791a7435c1592042ca22' ;; 		aarch64) binArch='arm64'; checksum='e425bd8b3514990de3bfed50375dac6abef9308a3e49d0098b2151b3b5dd74cb1e545e0b15bc2b57b21941a1d8cb4e1dcb1a50c93ea3c3e60d14a30394059b34' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='90cdeda18af8634fdfcaab60d58f246d88756ebae5c716a93e3c09ae266d86812b9e258f894447a3126dd6b37a8e19d5ea7fe0e33543d2a6f2e41bc947de0fd4' ;; 		s390x)   binArch='s390x'; checksum='db3eea7f378400ff4e12baca105997b8ff5cc4725fc901027e80d6bd4ce127fba7debefd52bbd5e40b54db30d6b2ca96d1221e4179044876ae39cf27e3bdf475' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0-beta.1/caddy_2.1.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 00:50:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 00:50:23 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 00:50:24 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 00:50:24 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 00:50:25 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 00:50:25 GMT
LABEL org.opencontainers.image.version=v2.1.0-beta.1
# Fri, 26 Jun 2020 00:50:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 00:50:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 00:50:27 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 00:50:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 00:50:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 00:50:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 00:50:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 00:50:31 GMT
EXPOSE 80
# Fri, 26 Jun 2020 00:50:31 GMT
EXPOSE 443
# Fri, 26 Jun 2020 00:50:32 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 00:50:32 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 00:50:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2a5a47b7ff29cc165cee9824ba874fa6cb56d737ce18f841fc3ed5e937cb75`  
		Last Modified: Mon, 15 Jun 2020 20:54:38 GMT  
		Size: 300.1 KB (300144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3243ce9c25dc28a597c553cc7f0d4816c4b75789e4ebc37225ac58d5bd078995`  
		Last Modified: Mon, 15 Jun 2020 20:54:38 GMT  
		Size: 5.8 KB (5842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732c51547d0432a08f1326dd9caf4c8ab5381227e7c28382002707d7fde62011`  
		Last Modified: Mon, 15 Jun 2020 20:54:43 GMT  
		Size: 12.6 MB (12581775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef648a9eebd2584542a6d9950c63fb8da0fa93c707f1e774e1fcf34d9b779a2`  
		Last Modified: Fri, 26 Jun 2020 00:51:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.0-beta.1-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:4c0882eda2e74ae5ec7a74f9b89c2f62e79019a5ed7959cc311193b049884769
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15267428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a552395a8eb3cd6fd933cb97457a6dc8119637a7e3c6f13e7d692f7c81548e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:59:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 21:00:00 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 21:00:03 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 15 Jun 2020 21:00:04 GMT
ENV CADDY_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 21:00:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='88c141648d1b2f77a3176d36d7448e0409118fa39572dd46f853928033fddc9c593d02101d6923f20acefc8fd7ac701d84dc4276dbc42c3a6c1b8c1e9d26eebd' ;; 		armhf)   binArch='armv6'; checksum='af8bb19b0c72d0c6e2cf748a62046102cf52c82454bbd32f1c75404188145da585dd2f9cc3848bf99ad9ebb94f546b56b1d2a4db73bdcf4c262e0441cf55af5d' ;; 		armv7)   binArch='armv7'; checksum='ba1a123791c531d69f677fbd2652429f37eb0298491fd25ae23629a12bec6ad4a33b5e6d25069ccd98773c3036b599054ccf152bf56e791a7435c1592042ca22' ;; 		aarch64) binArch='arm64'; checksum='e425bd8b3514990de3bfed50375dac6abef9308a3e49d0098b2151b3b5dd74cb1e545e0b15bc2b57b21941a1d8cb4e1dcb1a50c93ea3c3e60d14a30394059b34' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='90cdeda18af8634fdfcaab60d58f246d88756ebae5c716a93e3c09ae266d86812b9e258f894447a3126dd6b37a8e19d5ea7fe0e33543d2a6f2e41bc947de0fd4' ;; 		s390x)   binArch='s390x'; checksum='db3eea7f378400ff4e12baca105997b8ff5cc4725fc901027e80d6bd4ce127fba7debefd52bbd5e40b54db30d6b2ca96d1221e4179044876ae39cf27e3bdf475' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0-beta.1/caddy_2.1.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 00:59:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 00:59:08 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 00:59:09 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 00:59:09 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 00:59:10 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 00:59:10 GMT
LABEL org.opencontainers.image.version=v2.1.0-beta.1
# Fri, 26 Jun 2020 00:59:11 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 00:59:12 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 00:59:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 00:59:13 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 00:59:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 00:59:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 00:59:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 00:59:16 GMT
EXPOSE 80
# Fri, 26 Jun 2020 00:59:17 GMT
EXPOSE 443
# Fri, 26 Jun 2020 00:59:17 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 00:59:18 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 00:59:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2aa34f01f2f9112772fdaebe7083b7dcdb4313768e0d6533a3e5b99597c98d`  
		Last Modified: Mon, 15 Jun 2020 21:02:12 GMT  
		Size: 299.2 KB (299237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b107a7bf1560d80dcded532795715f77765cf1a3d9464665d42acab82d366e`  
		Last Modified: Mon, 15 Jun 2020 21:02:12 GMT  
		Size: 5.8 KB (5845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967915987b3a992d9002998ed87607ec38d821ddfa699e1977947d701c7be51b`  
		Last Modified: Mon, 15 Jun 2020 21:02:16 GMT  
		Size: 12.6 MB (12555429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e53f8fadc72987278ef5b53319e6078db333123b5bce64d56f63023f6136097`  
		Last Modified: Fri, 26 Jun 2020 01:00:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.0-beta.1-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f9e022c998b81c59c7944995985f06882f5bb9e2a7b7aad877faf99bf31b535d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15175624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b41f0fd0f628ee5d840ac13bcded95b9e990d6b2f3f3da48bd78b23ef0e28740`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:42:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 20:42:33 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 20:42:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 15 Jun 2020 20:42:36 GMT
ENV CADDY_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 20:42:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='88c141648d1b2f77a3176d36d7448e0409118fa39572dd46f853928033fddc9c593d02101d6923f20acefc8fd7ac701d84dc4276dbc42c3a6c1b8c1e9d26eebd' ;; 		armhf)   binArch='armv6'; checksum='af8bb19b0c72d0c6e2cf748a62046102cf52c82454bbd32f1c75404188145da585dd2f9cc3848bf99ad9ebb94f546b56b1d2a4db73bdcf4c262e0441cf55af5d' ;; 		armv7)   binArch='armv7'; checksum='ba1a123791c531d69f677fbd2652429f37eb0298491fd25ae23629a12bec6ad4a33b5e6d25069ccd98773c3036b599054ccf152bf56e791a7435c1592042ca22' ;; 		aarch64) binArch='arm64'; checksum='e425bd8b3514990de3bfed50375dac6abef9308a3e49d0098b2151b3b5dd74cb1e545e0b15bc2b57b21941a1d8cb4e1dcb1a50c93ea3c3e60d14a30394059b34' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='90cdeda18af8634fdfcaab60d58f246d88756ebae5c716a93e3c09ae266d86812b9e258f894447a3126dd6b37a8e19d5ea7fe0e33543d2a6f2e41bc947de0fd4' ;; 		s390x)   binArch='s390x'; checksum='db3eea7f378400ff4e12baca105997b8ff5cc4725fc901027e80d6bd4ce127fba7debefd52bbd5e40b54db30d6b2ca96d1221e4179044876ae39cf27e3bdf475' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0-beta.1/caddy_2.1.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:39:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:39:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:39:42 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:39:43 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:39:44 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:39:45 GMT
LABEL org.opencontainers.image.version=v2.1.0-beta.1
# Fri, 26 Jun 2020 01:39:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:39:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:39:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:39:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:39:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:39:49 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:39:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:39:50 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:39:51 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:39:52 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:39:52 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:39:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f33282aee1a51127f669c7222e26bd0d5107b28d68819a6ead7f68076a73dc`  
		Last Modified: Mon, 15 Jun 2020 20:44:05 GMT  
		Size: 300.4 KB (300393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b85f4621f67650b74dc2db70b30f9593bc6695d3e91ff3899b3ee7c34cffc04`  
		Last Modified: Mon, 15 Jun 2020 20:44:04 GMT  
		Size: 5.8 KB (5846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c4b107fc4b1eaed154176164b59c74fcd6457e880f0c6546faf2d34d149b78`  
		Last Modified: Mon, 15 Jun 2020 20:44:08 GMT  
		Size: 12.2 MB (12161267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a68a56ab072aff607c272b535b031020ab0600c0fbfc38de1be683f93bae808`  
		Last Modified: Fri, 26 Jun 2020 01:40:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.0-beta.1-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:e3dd7f9b270d127cfa2f780d19070debaa663de1f41504f2a8b9ff0f2412811a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.0 MB (15042389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e5712224a99bd347ac07739417c73a343c4008f5b89e1caab4f9a84c1b1fe2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:19:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 21:19:13 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 21:19:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 15 Jun 2020 21:19:21 GMT
ENV CADDY_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 21:19:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='88c141648d1b2f77a3176d36d7448e0409118fa39572dd46f853928033fddc9c593d02101d6923f20acefc8fd7ac701d84dc4276dbc42c3a6c1b8c1e9d26eebd' ;; 		armhf)   binArch='armv6'; checksum='af8bb19b0c72d0c6e2cf748a62046102cf52c82454bbd32f1c75404188145da585dd2f9cc3848bf99ad9ebb94f546b56b1d2a4db73bdcf4c262e0441cf55af5d' ;; 		armv7)   binArch='armv7'; checksum='ba1a123791c531d69f677fbd2652429f37eb0298491fd25ae23629a12bec6ad4a33b5e6d25069ccd98773c3036b599054ccf152bf56e791a7435c1592042ca22' ;; 		aarch64) binArch='arm64'; checksum='e425bd8b3514990de3bfed50375dac6abef9308a3e49d0098b2151b3b5dd74cb1e545e0b15bc2b57b21941a1d8cb4e1dcb1a50c93ea3c3e60d14a30394059b34' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='90cdeda18af8634fdfcaab60d58f246d88756ebae5c716a93e3c09ae266d86812b9e258f894447a3126dd6b37a8e19d5ea7fe0e33543d2a6f2e41bc947de0fd4' ;; 		s390x)   binArch='s390x'; checksum='db3eea7f378400ff4e12baca105997b8ff5cc4725fc901027e80d6bd4ce127fba7debefd52bbd5e40b54db30d6b2ca96d1221e4179044876ae39cf27e3bdf475' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0-beta.1/caddy_2.1.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:16:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:16:41 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:16:45 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:16:48 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:16:53 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:16:56 GMT
LABEL org.opencontainers.image.version=v2.1.0-beta.1
# Fri, 26 Jun 2020 01:17:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:17:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:17:14 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:17:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:17:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:17:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:17:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:17:39 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:17:42 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:17:45 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:17:50 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:17:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b28df4c8a155654ad705e08f459bd177acc1005644ce2173ac62e954d6d4d2`  
		Last Modified: Mon, 15 Jun 2020 21:24:35 GMT  
		Size: 302.4 KB (302369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2288431c86a795754eb4d3a678e778c534a14e9243aea01a7cf9feff8d8e4e`  
		Last Modified: Mon, 15 Jun 2020 21:24:35 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7209a53971081ce93e14e316f2ba60b8055bffd05a4d99e637161191d7fa6d6`  
		Last Modified: Mon, 15 Jun 2020 21:24:38 GMT  
		Size: 11.9 MB (11928820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04afaf9f3075f38bac61579a0d3a8946b65109dffe0534fb7904c6e4d5acd95c`  
		Last Modified: Fri, 26 Jun 2020 01:19:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.0-beta.1-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:96538f54c12919a30d26b81cba65396f45944702709b9fd79bd64f99f33c3ebe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15881784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0004092087cf1595e2c57354a8a3c7f1535d5881f2f57e730216ce5c6a952099`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:43:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 20:43:15 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 20:43:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 15 Jun 2020 20:43:16 GMT
ENV CADDY_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 20:43:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='88c141648d1b2f77a3176d36d7448e0409118fa39572dd46f853928033fddc9c593d02101d6923f20acefc8fd7ac701d84dc4276dbc42c3a6c1b8c1e9d26eebd' ;; 		armhf)   binArch='armv6'; checksum='af8bb19b0c72d0c6e2cf748a62046102cf52c82454bbd32f1c75404188145da585dd2f9cc3848bf99ad9ebb94f546b56b1d2a4db73bdcf4c262e0441cf55af5d' ;; 		armv7)   binArch='armv7'; checksum='ba1a123791c531d69f677fbd2652429f37eb0298491fd25ae23629a12bec6ad4a33b5e6d25069ccd98773c3036b599054ccf152bf56e791a7435c1592042ca22' ;; 		aarch64) binArch='arm64'; checksum='e425bd8b3514990de3bfed50375dac6abef9308a3e49d0098b2151b3b5dd74cb1e545e0b15bc2b57b21941a1d8cb4e1dcb1a50c93ea3c3e60d14a30394059b34' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='90cdeda18af8634fdfcaab60d58f246d88756ebae5c716a93e3c09ae266d86812b9e258f894447a3126dd6b37a8e19d5ea7fe0e33543d2a6f2e41bc947de0fd4' ;; 		s390x)   binArch='s390x'; checksum='db3eea7f378400ff4e12baca105997b8ff5cc4725fc901027e80d6bd4ce127fba7debefd52bbd5e40b54db30d6b2ca96d1221e4179044876ae39cf27e3bdf475' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0-beta.1/caddy_2.1.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:41:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:41:30 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:41:30 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:41:30 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:41:31 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:41:31 GMT
LABEL org.opencontainers.image.version=v2.1.0-beta.1
# Fri, 26 Jun 2020 01:41:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:41:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:41:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:41:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:41:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:41:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:41:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:41:33 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:41:33 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:41:34 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:41:34 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:41:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc47bdcaea173dfb029a09265c41846030477dc696b22fed52acad2b2078bb7`  
		Last Modified: Mon, 15 Jun 2020 20:44:21 GMT  
		Size: 300.5 KB (300524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf084f3ceb3b3b1196400fa251cc45e01de7ece41b7605bb40ae5178d849b47d`  
		Last Modified: Mon, 15 Jun 2020 20:44:26 GMT  
		Size: 5.8 KB (5841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d34155d08428f26786712fcdbc9c270779e8d7520b8d09a209dfb3de4b70780`  
		Last Modified: Mon, 15 Jun 2020 20:44:23 GMT  
		Size: 13.0 MB (13009076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00d36bbc65cb4aa4293ffd2284daf453dd6385b2574f156823f0ff8e3751b8a`  
		Last Modified: Fri, 26 Jun 2020 01:42:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.0-beta.1-builder`

```console
$ docker pull caddy@sha256:e1243f8135b7178f6012627992b436f30a1e42a8a7a3c3bcf053da51748e855e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.1.0-beta.1-builder` - linux; amd64

```console
$ docker pull caddy@sha256:6a73c0afaa9c695dae46c0e3809c9d81cfb549d610cebc506dec64489cf2db6c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.0 MB (330963648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb99c6045a91a75e2feed3a3fee17c3f3dcafb807e27dddabb9f3f38bba5094f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:30:20 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:32:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:32:35 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:32:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:32:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:32:36 GMT
WORKDIR /go
# Mon, 15 Jun 2020 21:21:27 GMT
WORKDIR /src
# Mon, 15 Jun 2020 21:21:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 15 Jun 2020 21:21:29 GMT
ENV CADDY_SOURCE_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 21:21:30 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Mon, 15 Jun 2020 21:21:30 GMT
WORKDIR /src/caddy/cmd/caddy
# Mon, 15 Jun 2020 21:21:44 GMT
RUN go get -d ./...
# Mon, 15 Jun 2020 21:21:45 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Mon, 15 Jun 2020 21:21:45 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0cccf56431698a0981b191f61dcb4ba6afa272d35deb14eaccf2cb46ed0f9d`  
		Last Modified: Tue, 02 Jun 2020 01:44:38 GMT  
		Size: 132.1 MB (132120859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbe0275821fc905c0321a44449b7ca670963f2cc0824150bea2125dee8dc7376`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8183c72c683b23caab534e2ddeef5f4a54ed1040c87f05484e0248e21bb74954`  
		Last Modified: Mon, 15 Jun 2020 21:22:10 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404f93ac2221d032b0fca7fdb3d4bc6d9156768ffc95251e0607652cfbecc8b8`  
		Last Modified: Mon, 15 Jun 2020 21:22:10 GMT  
		Size: 8.3 MB (8309926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eccefc2722a022bc353c22d1cfc06b41f8a32814ee742a4c00528896407ad85`  
		Last Modified: Mon, 15 Jun 2020 21:22:09 GMT  
		Size: 2.9 MB (2948822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0172ad31a9d4233b1fcca6fed379e6f1a185800e03c00c5cb94ad11cfc8a4179`  
		Last Modified: Mon, 15 Jun 2020 21:22:31 GMT  
		Size: 184.5 MB (184502866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea9b0307c6e5035db2a880e05d014d54d7f171443a6ce819b3171ac6ce10723`  
		Last Modified: Mon, 15 Jun 2020 21:22:09 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e349cc4afb0e5c1fbeb356296b436036487b0dbcaaceb882adc32062b4a4a8e`  
		Last Modified: Mon, 15 Jun 2020 21:22:09 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.0-beta.1-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b584c7cc30238909b12f2d24aa28d5f228e644186649db0c178f7aec284305ae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.5 MB (326479733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5d2ee13d21dc94605aa5a355f47f3c81014332b0078c1c1d7736946c434c0c7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:02:10 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 02:02:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 02:02:29 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 02:55:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 02:56:02 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 02:56:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 02:56:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 02:56:07 GMT
WORKDIR /go
# Mon, 15 Jun 2020 20:52:46 GMT
WORKDIR /src
# Mon, 15 Jun 2020 20:52:50 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 15 Jun 2020 20:52:50 GMT
ENV CADDY_SOURCE_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 20:52:53 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Mon, 15 Jun 2020 20:52:54 GMT
WORKDIR /src/caddy/cmd/caddy
# Mon, 15 Jun 2020 20:54:10 GMT
RUN go get -d ./...
# Mon, 15 Jun 2020 20:54:12 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Mon, 15 Jun 2020 20:54:14 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c276dc457bae632c9eadd1ac69c1a756a9a67e050b0350a475b19663722191cf`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 282.8 KB (282778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f0819b703e39c232c6d0a8ac0f76d8f3c6856629db16fd6dd7b7ae69368281`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e66763a2c2fd4a68d63d58e30f372cf4ebdc811274c6979d891e5e0cb676d73`  
		Last Modified: Tue, 02 Jun 2020 05:22:08 GMT  
		Size: 128.2 MB (128209215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7367c813a205e4503e365f0492c4c2de22baead5b600a620d362655aa9cd483`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce88b922cbeaa0f67211b29ad7ed76847d7725e329cc620ff7dcc9257fba77e3`  
		Last Modified: Mon, 15 Jun 2020 20:54:49 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720f093e5ede770f019c0c7a14a3361e9648d5b00f7a171f8feaefab719955aa`  
		Last Modified: Mon, 15 Jun 2020 20:54:50 GMT  
		Size: 7.9 MB (7928846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68db8f46ba8dbe5baed560fc8319503cbf909feb5588475796c8fdbeba31a4dc`  
		Last Modified: Mon, 15 Jun 2020 20:54:49 GMT  
		Size: 2.9 MB (2947642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234e27e6530d4cb104e662579ea028b612d79536b539a6e3fc95544bece1424a`  
		Last Modified: Mon, 15 Jun 2020 20:55:35 GMT  
		Size: 184.5 MB (184506842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cda957a3dfc8a6532f3f775c3751827e65234d5c81fc8dc179a1f2757d615ca`  
		Last Modified: Mon, 15 Jun 2020 20:54:48 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ca1b0c3b2083e3a3337a0c3a4a8916ad34e46d7a33c64938fabd2e247115f2`  
		Last Modified: Mon, 15 Jun 2020 20:54:48 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.0-beta.1-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:b793ebf3223797abf26fb13be83041fc3f2795d390804af0842b6bae0143cf5f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.1 MB (325135045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54ab1c9963d7d28bf4572b2025bff00835960ac6f9a233f838027139824d7321`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:10:58 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:11:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:11:01 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:34:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:34:38 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:34:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:34:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:34:44 GMT
WORKDIR /go
# Mon, 15 Jun 2020 21:00:34 GMT
WORKDIR /src
# Mon, 15 Jun 2020 21:00:37 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 15 Jun 2020 21:00:40 GMT
ENV CADDY_SOURCE_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 21:00:43 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Mon, 15 Jun 2020 21:00:44 GMT
WORKDIR /src/caddy/cmd/caddy
# Mon, 15 Jun 2020 21:01:41 GMT
RUN go get -d ./...
# Mon, 15 Jun 2020 21:01:47 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Mon, 15 Jun 2020 21:01:48 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512c25ce227edddad11326504a9bab47e83f8b61c090c9dc95882452984ac62`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 281.9 KB (281892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87928ee7e6c788309b46621e351321410e4dde5374869ffa75f404b19e0e0c12`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754691c4bcf20eb06087104e5fc82d340991d9bf26c21cae6979f36e3bd38ca7`  
		Last Modified: Tue, 02 Jun 2020 03:52:16 GMT  
		Size: 127.8 MB (127846663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63238be1b74c86ab98841c3959a33d79a903d58ac50518d4fa65b2ea8c6a75ba`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a1abd4bf80876cf553a554662e0cb3c5c310601b937ee7749c6f828de9dfea`  
		Last Modified: Mon, 15 Jun 2020 21:02:23 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac591f152779d4cfd93fb1e2f29dfeb27073f3559e8cb0daf8ee5c6f58310dc`  
		Last Modified: Mon, 15 Jun 2020 21:02:23 GMT  
		Size: 7.1 MB (7144878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86db61689f6f2b91f38163e2e30c4545a2427ebfacefb2b38c78648f50ca5c4d`  
		Last Modified: Mon, 15 Jun 2020 21:02:22 GMT  
		Size: 2.9 MB (2947630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe46c1743c26d39ab3f6784401d0ba72b36209c166664c187e7a11548dafd07`  
		Last Modified: Mon, 15 Jun 2020 21:03:08 GMT  
		Size: 184.5 MB (184506094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752f0cd018670630a157b1a4af43a8be0f27b314f6a110a7fc8ba6c03020b259`  
		Last Modified: Mon, 15 Jun 2020 21:02:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d71ed669fb0a8652915f691b3ba40fe33d24e739bb08f551066e02d4a082b7b`  
		Last Modified: Mon, 15 Jun 2020 21:02:21 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.0-beta.1-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7e7725ab9b625048b243442b3bbad690b15affe8b97d69adfddaa25b4047c234
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.5 MB (325450151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0664839a58e5a650639b09c514e3a30a069f5734c4e9f93638f310ddd96c9eac`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:58:16 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 02:00:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 02:00:34 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 02:00:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 02:00:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 02:01:01 GMT
WORKDIR /go
# Mon, 15 Jun 2020 20:42:55 GMT
WORKDIR /src
# Mon, 15 Jun 2020 20:42:58 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 15 Jun 2020 20:42:59 GMT
ENV CADDY_SOURCE_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 20:43:02 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Mon, 15 Jun 2020 20:43:02 GMT
WORKDIR /src/caddy/cmd/caddy
# Mon, 15 Jun 2020 20:43:31 GMT
RUN go get -d ./...
# Mon, 15 Jun 2020 20:43:36 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Mon, 15 Jun 2020 20:43:37 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a10f6d585c919680bed516e83e217d8bb824ee48306a00ce36c94a2a42e127`  
		Last Modified: Tue, 02 Jun 2020 02:30:00 GMT  
		Size: 126.5 MB (126505030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fdc7971b1eac6baae4423fc0ecca822c4d0372de7bfbdb5a7451e3cdd06be30`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9d4bc6b21331beadc7877a16034ab0b38c0afcf3434fba21ae30649336cb92`  
		Last Modified: Mon, 15 Jun 2020 20:44:13 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebe763a900953fc839be7c307bee96cc4464502cd2cf875941354458648b2b4`  
		Last Modified: Mon, 15 Jun 2020 20:44:13 GMT  
		Size: 8.5 MB (8499921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ebc8d0d57594e456fbcbb78e7f133d3ea4941682adc9012eee5db1f77be4d5`  
		Last Modified: Mon, 15 Jun 2020 20:44:12 GMT  
		Size: 2.9 MB (2947643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43451deb765ed7055418a57402bc811911bbd4b8d91412b7ffba479946459e4`  
		Last Modified: Mon, 15 Jun 2020 20:44:50 GMT  
		Size: 184.5 MB (184505472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5cd10e58555d40808623875cd96c716f43edc6d6d6c4d85808a9028387da5f`  
		Last Modified: Mon, 15 Jun 2020 20:44:12 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24b0e792e6ee3483908061816a958e42cbe9c42e28fb4b9f6e8cd1719b57725`  
		Last Modified: Mon, 15 Jun 2020 20:44:11 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.0-beta.1-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:3d697e383006406074fc94dbcf2ab039897bcc27beee4529e285aef28034ddd0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.7 MB (324725151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc6981160e8205319478e4128305c0c48665bc67e7ae6993bc4ebdec1c393a48`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:30:00 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:32:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:32:22 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:32:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:32:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:32:46 GMT
WORKDIR /go
# Mon, 15 Jun 2020 21:20:48 GMT
WORKDIR /src
# Mon, 15 Jun 2020 21:20:57 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 15 Jun 2020 21:21:00 GMT
ENV CADDY_SOURCE_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 21:21:08 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Mon, 15 Jun 2020 21:21:12 GMT
WORKDIR /src/caddy/cmd/caddy
# Mon, 15 Jun 2020 21:23:38 GMT
RUN go get -d ./...
# Mon, 15 Jun 2020 21:23:54 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Mon, 15 Jun 2020 21:23:57 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa9f54e0b14ecd0984863bb950f61bd4bf436b6072e38800e7f963358557067`  
		Last Modified: Tue, 02 Jun 2020 01:48:47 GMT  
		Size: 125.3 MB (125263901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a41edd0480b633d5ed3f00eef305e8a7526c48f1fdde5ef350565830d40609`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca1ca7c0085d0ffb2b0cb1bdabb73af28921fe105ac26bae09acee083eb4c72`  
		Last Modified: Mon, 15 Jun 2020 21:24:51 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55082f384c6dea8e172df520164ab7feeca61be6b9d38ab64bb2265b7f197b1`  
		Last Modified: Mon, 15 Jun 2020 21:24:49 GMT  
		Size: 8.9 MB (8919998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90905665a129e354e226c7575ecc4ddb5a98c47528165cfb837c16c380bad36f`  
		Last Modified: Mon, 15 Jun 2020 21:24:48 GMT  
		Size: 2.9 MB (2945059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f63353d28ed79dfa84ef3dcac82563ae8c8db98241949a4638b82a47fa6db1`  
		Last Modified: Mon, 15 Jun 2020 21:25:16 GMT  
		Size: 184.5 MB (184504835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f67d5f39b0dcc8675a6c48c17733f0cd707c9ef327ea0a7545be543a3b9d9bb`  
		Last Modified: Mon, 15 Jun 2020 21:24:46 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02ff8fd197012f6544aaf40aa94e5ce2555e4960214188f4ea91135d0b0f189`  
		Last Modified: Mon, 15 Jun 2020 21:24:47 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.0-beta.1-builder` - linux; s390x

```console
$ docker pull caddy@sha256:1c464d6b921fd2e335dc840af53517f3de63c78bc6fd55b6b5998dfc73adb746
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.5 MB (330468606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d7794d967c247a7b08ae148ee611ca583fe45e1877076fd4a2b4612cdbaacb9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:53:16 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:54:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:54:38 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:54:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:54:38 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:54:39 GMT
WORKDIR /go
# Mon, 15 Jun 2020 20:43:26 GMT
WORKDIR /src
# Mon, 15 Jun 2020 20:43:28 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 15 Jun 2020 20:43:28 GMT
ENV CADDY_SOURCE_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 20:43:29 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Mon, 15 Jun 2020 20:43:30 GMT
WORKDIR /src/caddy/cmd/caddy
# Mon, 15 Jun 2020 20:43:47 GMT
RUN go get -d ./...
# Mon, 15 Jun 2020 20:43:55 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Mon, 15 Jun 2020 20:43:55 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc125fe27a23a8501491445468375e7ea9db946b45cbd911a05a65cfb7c3334`  
		Last Modified: Tue, 02 Jun 2020 02:01:21 GMT  
		Size: 131.8 MB (131814783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7129c3822665192c1533e7d5ab270717e256b1b9844d6fd116852b00a29058e9`  
		Last Modified: Tue, 02 Jun 2020 02:01:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d8d7ec191535d778fe97d9e282050d4140fab1236212ea77816ba1db178bae`  
		Last Modified: Mon, 15 Jun 2020 20:44:32 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a8d11ad8b6daae49f4e16f31468f03664af47d81d6792e5da6fb1eff11ee52`  
		Last Modified: Mon, 15 Jun 2020 20:44:32 GMT  
		Size: 8.4 MB (8352257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8f498877c102d0e018220d716e0a056bacf2c03dfea62b8ef72a8297b0ac48`  
		Last Modified: Mon, 15 Jun 2020 20:44:30 GMT  
		Size: 2.9 MB (2947505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0203fea6b83df03bd9bfa009875c2a4f936457e55151bc843715ca55ef1b3ca`  
		Last Modified: Mon, 15 Jun 2020 20:44:46 GMT  
		Size: 184.5 MB (184503602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d6a718bb22c4ee74bc153ff60606deb54233407bd1b7cd79b7b2f5cbc7c80b`  
		Last Modified: Mon, 15 Jun 2020 20:44:46 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4612e648f6f05e88a15d1852d2c94d2d615608ea1999f8cb32438f883e7acfbb`  
		Last Modified: Mon, 15 Jun 2020 20:44:46 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.0-beta.1-windowsservercore`

```console
$ docker pull caddy@sha256:adafe9eb7ddc739930719f13022e2fab0ff2ed096afa4c9730282b18b25e70af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64
	-	windows version 10.0.14393.3750; amd64

### `caddy:2.1.0-beta.1-windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:637c6c607ab7ca56a590bb0ae86295010557a84dbdf3dc99fbf4cc591eb1e5bb
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2312521998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20942c19259da51445c3e6c4b6ddc9fedf01b3fb05b07099004d0857bb395936`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Tue, 09 Jun 2020 22:33:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:02:29 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:03:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 15 Jun 2020 21:15:46 GMT
ENV CADDY_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 21:16:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.0-beta.1/caddy_2.1.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8c87f1d5a4f94a5532fdf2b2f63890f4e88e19b8cb409b11cec5a34be263d42ffc17b76eb38bfff7f27b27e9e932f8c15783e96cce98448013fcc516dacf1d0b')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 15 Jun 2020 21:16:22 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 15 Jun 2020 21:16:23 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 15 Jun 2020 21:16:24 GMT
VOLUME [c:/config]
# Mon, 15 Jun 2020 21:16:25 GMT
VOLUME [c:/data]
# Mon, 15 Jun 2020 21:16:26 GMT
LABEL org.opencontainers.image.version=v2.1.0-beta.1
# Mon, 15 Jun 2020 21:16:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 15 Jun 2020 21:16:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 15 Jun 2020 21:16:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 15 Jun 2020 21:16:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 15 Jun 2020 21:16:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 15 Jun 2020 21:16:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 15 Jun 2020 21:16:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 15 Jun 2020 21:16:33 GMT
EXPOSE 80
# Mon, 15 Jun 2020 21:16:34 GMT
EXPOSE 443
# Mon, 15 Jun 2020 21:16:35 GMT
EXPOSE 2019
# Mon, 15 Jun 2020 21:16:52 GMT
RUN caddy version
# Mon, 15 Jun 2020 21:16:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f841c6a0c622cd36b5b2688011a224ac3e8e96273758f4a2804f2f3f099f267d`  
		Last Modified: Tue, 09 Jun 2020 23:17:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e676deb3766189ea2b008f69205017c9ee31a77f9c7001fb5a07fb2e2d4fbb0`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba576338ed5242ba3fb838ce5fa930abb61e22fc422ba46b260dbca773cb9`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 4.8 MB (4772911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e3e4a9deb067045cd0c24b717ffc454d12b87b5f184498f199a4500fcc39ea`  
		Last Modified: Mon, 15 Jun 2020 21:20:18 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed77eefd9fab412b04cfe83746a7d782cf06fb7e26076961fdf01629bf3178b`  
		Last Modified: Mon, 15 Jun 2020 21:20:22 GMT  
		Size: 13.5 MB (13514542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db36924581cd6c03fbc76c1f2536196031f85d7f0632d8ba14ec83dc16e8ca5d`  
		Last Modified: Mon, 15 Jun 2020 21:20:18 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ac6eae76c670d7ba4b0b7c71ec62e7b2985130093837a063cda8cfb6fdb014`  
		Last Modified: Mon, 15 Jun 2020 21:20:17 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ced9b1ae0ee4451dff19cfd6cbc3518ca9fd63b08a3b298846336eec9a92db7`  
		Last Modified: Mon, 15 Jun 2020 21:20:16 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ef23d879b1c5fa266b603fa2ec1ab8f448c51688b2bbbd026a3cdd61e3239`  
		Last Modified: Mon, 15 Jun 2020 21:20:16 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77ba47e8b13bad632b11a83940626505edd75e01c8de4dc24855721e9f48d3f`  
		Last Modified: Mon, 15 Jun 2020 21:20:15 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ed31c38dafc3492acdf4272645ef61c97c18c553777d342c317e70773b9c76`  
		Last Modified: Mon, 15 Jun 2020 21:20:16 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2365dc868a8422756f8ae8f40d061c1b09dc409bc982b25cc8c9c23bce7837d`  
		Last Modified: Mon, 15 Jun 2020 21:20:15 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af8bc08af2758e7f6a18b9a9ec78cec98975121415b3575c33539fc2033d390`  
		Last Modified: Mon, 15 Jun 2020 21:20:14 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fde35a97b738c5b8b6eec76486e86738045f0f6d27863f7d0991c034210bcef`  
		Last Modified: Mon, 15 Jun 2020 21:20:13 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ab21673c985472de4bead86534ff719ac16032d2bb4588b5edd8eb2db504de`  
		Last Modified: Mon, 15 Jun 2020 21:20:13 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e2e941122550083392e2d1271f6c18c3a8dc0872c51727b783a19231bfef33`  
		Last Modified: Mon, 15 Jun 2020 21:20:12 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5f95d02c4e9e331b8eb2f59baa2eab2cb29219fef1b0b235062833c7879ccd`  
		Last Modified: Mon, 15 Jun 2020 21:20:13 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe8f7ad33f8d57d12301a1812d501e197b329152f2d55b99e8863c3ae3a10e9`  
		Last Modified: Mon, 15 Jun 2020 21:20:10 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aea5478316d530d122395a14076ab5093a59eadd6ab6be4c99f9c3185327248`  
		Last Modified: Mon, 15 Jun 2020 21:20:10 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb3d364dd289b26eeda93175144e40522e3447db2f70987a5ca69e9972e0b21`  
		Last Modified: Mon, 15 Jun 2020 21:20:10 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7261589e0957fb07bbb94cd24f9650b976302660138ea35d0b8b47ddf75cef7`  
		Last Modified: Mon, 15 Jun 2020 21:20:10 GMT  
		Size: 298.5 KB (298457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e977c97431a52c4b2c351a5e8cf85767c61a968cec76dbcfbbeca0e4374fa4`  
		Last Modified: Mon, 15 Jun 2020 21:20:10 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.0-beta.1-windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:6201786c3d7a42cac215b169cdfe88681e266ee7d6d390988a8f68fb83bea620
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758217462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a25a49441e73129c3e36057198e872fcf40750007748ea8e2816815dda841ef`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:04:40 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:06:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 15 Jun 2020 21:17:09 GMT
ENV CADDY_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 21:18:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.0-beta.1/caddy_2.1.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8c87f1d5a4f94a5532fdf2b2f63890f4e88e19b8cb409b11cec5a34be263d42ffc17b76eb38bfff7f27b27e9e932f8c15783e96cce98448013fcc516dacf1d0b')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 15 Jun 2020 21:18:35 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 15 Jun 2020 21:18:36 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 15 Jun 2020 21:18:37 GMT
VOLUME [c:/config]
# Mon, 15 Jun 2020 21:18:38 GMT
VOLUME [c:/data]
# Mon, 15 Jun 2020 21:18:39 GMT
LABEL org.opencontainers.image.version=v2.1.0-beta.1
# Mon, 15 Jun 2020 21:18:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 15 Jun 2020 21:18:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 15 Jun 2020 21:18:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 15 Jun 2020 21:18:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 15 Jun 2020 21:18:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 15 Jun 2020 21:18:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 15 Jun 2020 21:18:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 15 Jun 2020 21:18:46 GMT
EXPOSE 80
# Mon, 15 Jun 2020 21:18:47 GMT
EXPOSE 443
# Mon, 15 Jun 2020 21:18:48 GMT
EXPOSE 2019
# Mon, 15 Jun 2020 21:19:29 GMT
RUN caddy version
# Mon, 15 Jun 2020 21:19:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22985925139cd6a6e83b6eb5286a8a6e1053a5c6ddd9762f34deea2aa6bcaacc`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43c028d6768e901bc64b3edb7e2e5f72050d3ed78ea4e7337fe85725d250c15`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 5.4 MB (5404509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c22ecccbfcd030d10a64153d97b05414a12a6e4391fc7727f205d250f82d29b`  
		Last Modified: Mon, 15 Jun 2020 21:20:43 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043abd7aae9c81cfb27da0a6048b753f5d13342428c4351210380b2ef34f1797`  
		Last Modified: Mon, 15 Jun 2020 21:20:47 GMT  
		Size: 18.5 MB (18548536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a94d03da17df89277ff8583569c9cf95187fd10568cb0b9f44bc6dd23b4ab9`  
		Last Modified: Mon, 15 Jun 2020 21:20:42 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054637bf72793f6d35a09b82643d312e8350a19c05a84badcb60eed66e05f9e3`  
		Last Modified: Mon, 15 Jun 2020 21:20:41 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab0ca47076e559a31592d3daac2783f528bce5460203b265a1bf8161d6f1178`  
		Last Modified: Mon, 15 Jun 2020 21:20:40 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b248096abce77da76924f7399bc6942dc8b9e2f025f871c57433971441a246`  
		Last Modified: Mon, 15 Jun 2020 21:20:40 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81455e02f083bd2146af80776e9cc46b0aafaae7593b24b520577b6ab8031ce4`  
		Last Modified: Mon, 15 Jun 2020 21:20:40 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0150fc8e2c153b78027f67e85f6a2bac3bd57be7eae71251c36443cab1eaff40`  
		Last Modified: Mon, 15 Jun 2020 21:20:40 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578d4cdda9428605fe5933f3e16e4c40d18d4f15f486c2bde43f5ad12a84405f`  
		Last Modified: Mon, 15 Jun 2020 21:20:39 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213fe93c05e7b9c8152020cc11bb769e0d0a5670fcec11f5e10054379ade4b91`  
		Last Modified: Mon, 15 Jun 2020 21:20:37 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bef0c8ef4c5321e14235137d7b40bd580a931189d447c53e4902b4b0bfdb4d`  
		Last Modified: Mon, 15 Jun 2020 21:20:37 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d954a308c87819fe2e19d1bf5ef936453ab1e92b386b0cafaac37507e52f4eea`  
		Last Modified: Mon, 15 Jun 2020 21:20:37 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2335b8f54fc31963d6843047a2bdd2a234ca726e9061869551369f6623d7c60a`  
		Last Modified: Mon, 15 Jun 2020 21:20:37 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d17720617ae9cf3b603669655085a68016364f67a23446289006a68f20e13fd`  
		Last Modified: Mon, 15 Jun 2020 21:20:37 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1105a52fd3f7d8ccfab34c3a84c52c70ef4916f12c188775357d544344b495e5`  
		Last Modified: Mon, 15 Jun 2020 21:20:34 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a02dd52c835be30792e049cff4d4bbc6beb11a71718b78f5f20bc8cf474308b`  
		Last Modified: Mon, 15 Jun 2020 21:20:34 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:158c3526d0ace10490df86298bd0fd6a8ee0b0539735e2bf19cb99f93e283bd6`  
		Last Modified: Mon, 15 Jun 2020 21:20:34 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0963f5b2777be491c70973c436712d0c0a0e851be8d75a1a5443bdc07d5b7d9`  
		Last Modified: Mon, 15 Jun 2020 21:20:35 GMT  
		Size: 244.9 KB (244942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d861ed92a97bfd175d80668a81b3da55db1f527c5f453b65182240af0bed640`  
		Last Modified: Mon, 15 Jun 2020 21:20:34 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.0-beta.1-windowsservercore-1809`

```console
$ docker pull caddy@sha256:f68ab50535e7f1889222a043bd534e4a0cbb9c306b576100b8a81d1681e72a8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `caddy:2.1.0-beta.1-windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:637c6c607ab7ca56a590bb0ae86295010557a84dbdf3dc99fbf4cc591eb1e5bb
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2312521998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20942c19259da51445c3e6c4b6ddc9fedf01b3fb05b07099004d0857bb395936`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Tue, 09 Jun 2020 22:33:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:02:29 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:03:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 15 Jun 2020 21:15:46 GMT
ENV CADDY_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 21:16:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.0-beta.1/caddy_2.1.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8c87f1d5a4f94a5532fdf2b2f63890f4e88e19b8cb409b11cec5a34be263d42ffc17b76eb38bfff7f27b27e9e932f8c15783e96cce98448013fcc516dacf1d0b')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 15 Jun 2020 21:16:22 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 15 Jun 2020 21:16:23 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 15 Jun 2020 21:16:24 GMT
VOLUME [c:/config]
# Mon, 15 Jun 2020 21:16:25 GMT
VOLUME [c:/data]
# Mon, 15 Jun 2020 21:16:26 GMT
LABEL org.opencontainers.image.version=v2.1.0-beta.1
# Mon, 15 Jun 2020 21:16:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 15 Jun 2020 21:16:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 15 Jun 2020 21:16:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 15 Jun 2020 21:16:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 15 Jun 2020 21:16:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 15 Jun 2020 21:16:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 15 Jun 2020 21:16:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 15 Jun 2020 21:16:33 GMT
EXPOSE 80
# Mon, 15 Jun 2020 21:16:34 GMT
EXPOSE 443
# Mon, 15 Jun 2020 21:16:35 GMT
EXPOSE 2019
# Mon, 15 Jun 2020 21:16:52 GMT
RUN caddy version
# Mon, 15 Jun 2020 21:16:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f841c6a0c622cd36b5b2688011a224ac3e8e96273758f4a2804f2f3f099f267d`  
		Last Modified: Tue, 09 Jun 2020 23:17:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e676deb3766189ea2b008f69205017c9ee31a77f9c7001fb5a07fb2e2d4fbb0`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba576338ed5242ba3fb838ce5fa930abb61e22fc422ba46b260dbca773cb9`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 4.8 MB (4772911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e3e4a9deb067045cd0c24b717ffc454d12b87b5f184498f199a4500fcc39ea`  
		Last Modified: Mon, 15 Jun 2020 21:20:18 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed77eefd9fab412b04cfe83746a7d782cf06fb7e26076961fdf01629bf3178b`  
		Last Modified: Mon, 15 Jun 2020 21:20:22 GMT  
		Size: 13.5 MB (13514542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db36924581cd6c03fbc76c1f2536196031f85d7f0632d8ba14ec83dc16e8ca5d`  
		Last Modified: Mon, 15 Jun 2020 21:20:18 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ac6eae76c670d7ba4b0b7c71ec62e7b2985130093837a063cda8cfb6fdb014`  
		Last Modified: Mon, 15 Jun 2020 21:20:17 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ced9b1ae0ee4451dff19cfd6cbc3518ca9fd63b08a3b298846336eec9a92db7`  
		Last Modified: Mon, 15 Jun 2020 21:20:16 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ef23d879b1c5fa266b603fa2ec1ab8f448c51688b2bbbd026a3cdd61e3239`  
		Last Modified: Mon, 15 Jun 2020 21:20:16 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77ba47e8b13bad632b11a83940626505edd75e01c8de4dc24855721e9f48d3f`  
		Last Modified: Mon, 15 Jun 2020 21:20:15 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ed31c38dafc3492acdf4272645ef61c97c18c553777d342c317e70773b9c76`  
		Last Modified: Mon, 15 Jun 2020 21:20:16 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2365dc868a8422756f8ae8f40d061c1b09dc409bc982b25cc8c9c23bce7837d`  
		Last Modified: Mon, 15 Jun 2020 21:20:15 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af8bc08af2758e7f6a18b9a9ec78cec98975121415b3575c33539fc2033d390`  
		Last Modified: Mon, 15 Jun 2020 21:20:14 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fde35a97b738c5b8b6eec76486e86738045f0f6d27863f7d0991c034210bcef`  
		Last Modified: Mon, 15 Jun 2020 21:20:13 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ab21673c985472de4bead86534ff719ac16032d2bb4588b5edd8eb2db504de`  
		Last Modified: Mon, 15 Jun 2020 21:20:13 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e2e941122550083392e2d1271f6c18c3a8dc0872c51727b783a19231bfef33`  
		Last Modified: Mon, 15 Jun 2020 21:20:12 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5f95d02c4e9e331b8eb2f59baa2eab2cb29219fef1b0b235062833c7879ccd`  
		Last Modified: Mon, 15 Jun 2020 21:20:13 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe8f7ad33f8d57d12301a1812d501e197b329152f2d55b99e8863c3ae3a10e9`  
		Last Modified: Mon, 15 Jun 2020 21:20:10 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aea5478316d530d122395a14076ab5093a59eadd6ab6be4c99f9c3185327248`  
		Last Modified: Mon, 15 Jun 2020 21:20:10 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb3d364dd289b26eeda93175144e40522e3447db2f70987a5ca69e9972e0b21`  
		Last Modified: Mon, 15 Jun 2020 21:20:10 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7261589e0957fb07bbb94cd24f9650b976302660138ea35d0b8b47ddf75cef7`  
		Last Modified: Mon, 15 Jun 2020 21:20:10 GMT  
		Size: 298.5 KB (298457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e977c97431a52c4b2c351a5e8cf85767c61a968cec76dbcfbbeca0e4374fa4`  
		Last Modified: Mon, 15 Jun 2020 21:20:10 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.0-beta.1-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:d5018165c4a3e00f32633ca090c90cb266acf0b16ca98f5550fecada52ed5964
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `caddy:2.1.0-beta.1-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:6201786c3d7a42cac215b169cdfe88681e266ee7d6d390988a8f68fb83bea620
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758217462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a25a49441e73129c3e36057198e872fcf40750007748ea8e2816815dda841ef`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:04:40 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:06:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 15 Jun 2020 21:17:09 GMT
ENV CADDY_VERSION=v2.1.0-beta.1
# Mon, 15 Jun 2020 21:18:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.0-beta.1/caddy_2.1.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8c87f1d5a4f94a5532fdf2b2f63890f4e88e19b8cb409b11cec5a34be263d42ffc17b76eb38bfff7f27b27e9e932f8c15783e96cce98448013fcc516dacf1d0b')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 15 Jun 2020 21:18:35 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 15 Jun 2020 21:18:36 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 15 Jun 2020 21:18:37 GMT
VOLUME [c:/config]
# Mon, 15 Jun 2020 21:18:38 GMT
VOLUME [c:/data]
# Mon, 15 Jun 2020 21:18:39 GMT
LABEL org.opencontainers.image.version=v2.1.0-beta.1
# Mon, 15 Jun 2020 21:18:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 15 Jun 2020 21:18:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 15 Jun 2020 21:18:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 15 Jun 2020 21:18:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 15 Jun 2020 21:18:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 15 Jun 2020 21:18:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 15 Jun 2020 21:18:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 15 Jun 2020 21:18:46 GMT
EXPOSE 80
# Mon, 15 Jun 2020 21:18:47 GMT
EXPOSE 443
# Mon, 15 Jun 2020 21:18:48 GMT
EXPOSE 2019
# Mon, 15 Jun 2020 21:19:29 GMT
RUN caddy version
# Mon, 15 Jun 2020 21:19:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22985925139cd6a6e83b6eb5286a8a6e1053a5c6ddd9762f34deea2aa6bcaacc`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43c028d6768e901bc64b3edb7e2e5f72050d3ed78ea4e7337fe85725d250c15`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 5.4 MB (5404509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c22ecccbfcd030d10a64153d97b05414a12a6e4391fc7727f205d250f82d29b`  
		Last Modified: Mon, 15 Jun 2020 21:20:43 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043abd7aae9c81cfb27da0a6048b753f5d13342428c4351210380b2ef34f1797`  
		Last Modified: Mon, 15 Jun 2020 21:20:47 GMT  
		Size: 18.5 MB (18548536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a94d03da17df89277ff8583569c9cf95187fd10568cb0b9f44bc6dd23b4ab9`  
		Last Modified: Mon, 15 Jun 2020 21:20:42 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054637bf72793f6d35a09b82643d312e8350a19c05a84badcb60eed66e05f9e3`  
		Last Modified: Mon, 15 Jun 2020 21:20:41 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab0ca47076e559a31592d3daac2783f528bce5460203b265a1bf8161d6f1178`  
		Last Modified: Mon, 15 Jun 2020 21:20:40 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b248096abce77da76924f7399bc6942dc8b9e2f025f871c57433971441a246`  
		Last Modified: Mon, 15 Jun 2020 21:20:40 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81455e02f083bd2146af80776e9cc46b0aafaae7593b24b520577b6ab8031ce4`  
		Last Modified: Mon, 15 Jun 2020 21:20:40 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0150fc8e2c153b78027f67e85f6a2bac3bd57be7eae71251c36443cab1eaff40`  
		Last Modified: Mon, 15 Jun 2020 21:20:40 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578d4cdda9428605fe5933f3e16e4c40d18d4f15f486c2bde43f5ad12a84405f`  
		Last Modified: Mon, 15 Jun 2020 21:20:39 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213fe93c05e7b9c8152020cc11bb769e0d0a5670fcec11f5e10054379ade4b91`  
		Last Modified: Mon, 15 Jun 2020 21:20:37 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bef0c8ef4c5321e14235137d7b40bd580a931189d447c53e4902b4b0bfdb4d`  
		Last Modified: Mon, 15 Jun 2020 21:20:37 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d954a308c87819fe2e19d1bf5ef936453ab1e92b386b0cafaac37507e52f4eea`  
		Last Modified: Mon, 15 Jun 2020 21:20:37 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2335b8f54fc31963d6843047a2bdd2a234ca726e9061869551369f6623d7c60a`  
		Last Modified: Mon, 15 Jun 2020 21:20:37 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d17720617ae9cf3b603669655085a68016364f67a23446289006a68f20e13fd`  
		Last Modified: Mon, 15 Jun 2020 21:20:37 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1105a52fd3f7d8ccfab34c3a84c52c70ef4916f12c188775357d544344b495e5`  
		Last Modified: Mon, 15 Jun 2020 21:20:34 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a02dd52c835be30792e049cff4d4bbc6beb11a71718b78f5f20bc8cf474308b`  
		Last Modified: Mon, 15 Jun 2020 21:20:34 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:158c3526d0ace10490df86298bd0fd6a8ee0b0539735e2bf19cb99f93e283bd6`  
		Last Modified: Mon, 15 Jun 2020 21:20:34 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0963f5b2777be491c70973c436712d0c0a0e851be8d75a1a5443bdc07d5b7d9`  
		Last Modified: Mon, 15 Jun 2020 21:20:35 GMT  
		Size: 244.9 KB (244942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d861ed92a97bfd175d80668a81b3da55db1f527c5f453b65182240af0bed640`  
		Last Modified: Mon, 15 Jun 2020 21:20:34 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:a985dd43871e9cb6c6ab3f9e45dd7bac9732f9f8d7c35f5d1b78a160b57bee4c
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
$ docker pull caddy@sha256:262f58e0836d0be11253e500e3b32e78e6d6149a90ed54e4a4ed5ca736e844fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15145372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:313ad00e425a86a5b5f39170ac018ada5d833fae55ab101712e80f52b4b986de`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 13:39:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 24 Apr 2020 13:39:03 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Fri, 24 Apr 2020 13:39:05 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 19:20:49 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 16:21:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:19:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:19:44 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:19:44 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:19:44 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:19:44 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:19:44 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:19:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:19:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:19:46 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:19:46 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:19:46 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:19:47 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:19:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c92d2df695a8e1549e487fe6691311b8c3ccfdd90383c6ae37c578c4465c76`  
		Last Modified: Fri, 24 Apr 2020 13:39:22 GMT  
		Size: 318.6 KB (318554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d779d752c63b3ccba5c5fbec57ae2361cef2059d83ea0770f389f1d9849ccde`  
		Last Modified: Fri, 24 Apr 2020 13:39:22 GMT  
		Size: 5.8 KB (5765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e321d52b548add190f8f5974453da203fc605ed33865ced7b83cc1e8fddc904e`  
		Last Modified: Wed, 06 May 2020 16:21:33 GMT  
		Size: 12.0 MB (12007584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c780a87c731befe76e920c134aaa9d393de1437f0c3940f40b355bc61de8f7a6`  
		Last Modified: Fri, 26 Jun 2020 01:20:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e304abe5082419b9f5b33d893544fd83a96932dcb7e064f871bee67716222091
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.4 MB (14390760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76f2894818f3ff916764fc8e6f3111c24629f11662bd03135b07492053d9dc86`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:42:29 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 23 Apr 2020 17:42:31 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Thu, 23 Apr 2020 17:42:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 18:49:25 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:49:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 00:50:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 00:50:46 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 00:50:47 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 00:50:47 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 00:50:48 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 00:50:49 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 00:50:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 00:50:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 00:50:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 00:50:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 00:50:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 00:50:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 00:50:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 00:50:55 GMT
EXPOSE 80
# Fri, 26 Jun 2020 00:50:56 GMT
EXPOSE 443
# Fri, 26 Jun 2020 00:50:57 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 00:50:58 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 00:50:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4aecf4b3c455b15219e7ae2914078c1796d34e6b1c2916aab2fa79d0aecc97`  
		Last Modified: Thu, 23 Apr 2020 17:43:07 GMT  
		Size: 318.9 KB (318932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78f3e6c459120cfcfb844a46e1d5fa39f425743ad39e3265fdb6b4c4ea312b6`  
		Last Modified: Thu, 23 Apr 2020 17:43:07 GMT  
		Size: 5.8 KB (5842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6977aa451d29e02cfa0a60ee52aadf3bfa7fad7712ac1687007cbb0bd812f996`  
		Last Modified: Wed, 06 May 2020 15:50:14 GMT  
		Size: 11.4 MB (11445896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2e1a3cae97c62afbdf067d2b1201f2e96a4ae8bb2320a3883f82fd1aec2824`  
		Last Modified: Fri, 26 Jun 2020 00:51:21 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2653b633a6ecc87fdf8ab9941be387a42f25f1c17580878c9cd47055a726d734
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14164711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87f56b16af8dc7e3d49ffb1018e82def382e00da18d024561d9c1fbc0a392938`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 23:22:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 23 Apr 2020 23:22:58 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Thu, 23 Apr 2020 23:23:03 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 18:57:29 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:57:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 00:59:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 00:59:31 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 00:59:31 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 00:59:32 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 00:59:32 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 00:59:33 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 00:59:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 00:59:34 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 00:59:35 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 00:59:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 00:59:36 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 00:59:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 00:59:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 00:59:39 GMT
EXPOSE 80
# Fri, 26 Jun 2020 00:59:39 GMT
EXPOSE 443
# Fri, 26 Jun 2020 00:59:40 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 00:59:41 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 00:59:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf760b044fed05d609c6cc0dbc0163d673af839c2bd8b93be46a9dd9b3235d8d`  
		Last Modified: Thu, 23 Apr 2020 23:23:51 GMT  
		Size: 317.9 KB (317871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702db93291bb8c691008d86b00d866d87fd9904461e56e447408436f67069d12`  
		Last Modified: Thu, 23 Apr 2020 23:23:50 GMT  
		Size: 5.8 KB (5843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a240b5e189e2da028c9e14c55e560dda7eebabe89a0fdc68bd063df8ac5403`  
		Last Modified: Wed, 06 May 2020 15:58:14 GMT  
		Size: 11.4 MB (11418780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febb3ae65834fee908dad31bb9b1fe5dbffd24c31bd7b4d6eb3f7e0cc0be6524`  
		Last Modified: Fri, 26 Jun 2020 01:00:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:d9aef3ac6d0885fa20fd11f612c78377e9b9e12bca0d92e77205e7c90e65d07c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14099502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d385c1b96da99f80af54a8b12302cb050f0b91d661b1d5d3c876b6ae33003cfc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 03:41:26 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 24 Apr 2020 03:41:27 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Fri, 24 Apr 2020 03:41:30 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 18:39:39 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 16:39:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:40:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:40:07 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:40:08 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:40:09 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:40:09 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:40:10 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:40:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:40:11 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:40:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:40:13 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:40:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:40:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:40:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:40:16 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:40:16 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:40:17 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:40:18 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:40:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1dd90474a5634d83eea66237a34342ba1aa7b9660127d7a6168f9dd16a6800`  
		Last Modified: Fri, 24 Apr 2020 03:42:02 GMT  
		Size: 319.1 KB (319109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523ce157ee2040adfd1d897f97c884c8df6de54df4581f3982d4114fea063843`  
		Last Modified: Fri, 24 Apr 2020 03:42:02 GMT  
		Size: 5.8 KB (5843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45586f3cd2c78aa4e4ec308b720449bd298ff8184489fc23ed1b63329d5bfba`  
		Last Modified: Wed, 06 May 2020 16:40:28 GMT  
		Size: 11.0 MB (11049973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f00aaba3fbdd96271be17e7a6a5b181a398f7c2f05bc510c8fb471d69578081`  
		Last Modified: Fri, 26 Jun 2020 01:40:41 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:084bd1339d1118c2e8a50d81da5761d085ebb079eb47faa49957cbcc89168f1a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14000418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c23735b817347971b241008c1dc978437390ce830fce6cf006d678d61b8b21af`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Wed, 06 May 2020 15:29:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 06 May 2020 15:30:01 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Wed, 06 May 2020 15:30:08 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Wed, 06 May 2020 15:30:10 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:30:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:18:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:18:24 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:18:27 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:18:29 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:18:33 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:18:38 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:18:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:18:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:18:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:18:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:18:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:19:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:19:04 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:19:08 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:19:12 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:19:17 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:19:21 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5a8966b60d898cbfd9fb53281860fcb82df54d8f66c9142f4038d0e3d8afb8`  
		Last Modified: Wed, 06 May 2020 15:36:35 GMT  
		Size: 321.6 KB (321641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcdcee6bf7f07bf2e87c36762756faa63a587b445b5112371d799d9983a38d7f`  
		Last Modified: Wed, 06 May 2020 15:36:34 GMT  
		Size: 5.8 KB (5845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912d87d0a8415f3b9ba60c72fc6309c0c67fb08b2834913add34eb8344ce0826`  
		Last Modified: Wed, 06 May 2020 15:36:42 GMT  
		Size: 10.9 MB (10850936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a992aa5354ab6566aa182b0b2122386db6d1143f1bfac22dc492fd1e1c9483`  
		Last Modified: Fri, 26 Jun 2020 01:20:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:16c31b5a11f0b34504a63c04a8b8a84c455e1669a3994f207a0d2d12047f7413
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14740730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d4431f588c0c1832ba15b0e102a300b97eb5374c9434a6c17cfb6ad324eee24`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Wed, 06 May 2020 15:30:02 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 06 May 2020 15:30:03 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Wed, 06 May 2020 15:30:05 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Wed, 06 May 2020 15:30:05 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:30:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:41:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:41:44 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:41:44 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:41:44 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:41:45 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:41:45 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:41:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:41:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:41:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:41:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:41:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:41:47 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:41:47 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:41:48 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:41:48 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:41:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1098bec6a96fa022c5d1e1043cbd10f41d1b5e0788cdeb71e1cbdf3ba0f6b6`  
		Last Modified: Wed, 06 May 2020 15:32:28 GMT  
		Size: 319.2 KB (319200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b06bf33ed224c71042842eaa50af6440423bb48f5cf032ce51277c7d08cb79f`  
		Last Modified: Wed, 06 May 2020 15:32:27 GMT  
		Size: 5.8 KB (5840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b3c02c4f07ca031406ddeefa20f1428b199d11370f5548cffe6bf3c294088c`  
		Last Modified: Wed, 06 May 2020 15:32:29 GMT  
		Size: 11.8 MB (11832677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b274cabb90bbeb4aafa4418e77b128c5caf6aed9aa6b6f1f756a905af241d2cd`  
		Last Modified: Fri, 26 Jun 2020 01:42:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:e7f19375fb2af512955ebfe845d8ea78b32cae8c608d367d393cbc209fc2cf3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:0750762062e92c7e2e8aa0c2c7e80d5762f6771f9c38aee0d4369b562bdad52b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.8 MB (322833946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed310fb9f0cd01f3920b3f64f1697fea83efa462d6fefdd30cc519a005c6910b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:29:00 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 24 Apr 2020 14:29:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:32:50 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:35:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:35:10 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:35:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:35:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:35:11 GMT
WORKDIR /go
# Tue, 02 Jun 2020 02:32:26 GMT
WORKDIR /src
# Tue, 02 Jun 2020 02:32:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 02 Jun 2020 02:32:27 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0
# Tue, 02 Jun 2020 02:32:28 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 02 Jun 2020 02:32:29 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 02 Jun 2020 02:32:42 GMT
RUN go get -d ./...
# Tue, 02 Jun 2020 02:32:42 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 02 Jun 2020 02:32:42 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408f875501273f3af2a9cbff2a23e736585641e73da80dd81712518b28e7843c`  
		Last Modified: Fri, 24 Apr 2020 14:36:50 GMT  
		Size: 301.3 KB (301282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe522b08c9798748151fec9b7a908aca712cd102cfcbb8ed79d57d05b71e6cc4`  
		Last Modified: Fri, 24 Apr 2020 14:36:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1be7d07969680a19c74f96783bb978cfc281d9eb21dd6377a1ba0c60b22161`  
		Last Modified: Tue, 02 Jun 2020 01:45:12 GMT  
		Size: 132.1 MB (132121186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed5455f4aa4c7ceedfadd2f093fffcda763951c5ae506c6d92151ad6e4dae0e`  
		Last Modified: Tue, 02 Jun 2020 01:44:46 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45598100dcda08511c93d19c558a05a901b1a183efefa4cda30b7c7e6f93d03c`  
		Last Modified: Tue, 02 Jun 2020 02:32:53 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89489597245daae1172eaaf4fc1db5044f7684053f7428c9e2b93b567d6d50d`  
		Last Modified: Tue, 02 Jun 2020 02:32:54 GMT  
		Size: 8.2 MB (8177829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc24cd02350289621830e1a9e35520aaa1bc92133dd8b9f775d5d108f93126cc`  
		Last Modified: Tue, 02 Jun 2020 02:32:52 GMT  
		Size: 2.7 MB (2706286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4dbcd3eb953512768ffac90d7561911f8d07b650519e87a8f150417c4210b3`  
		Last Modified: Tue, 02 Jun 2020 02:33:13 GMT  
		Size: 176.7 MB (176713022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461dd6e5ccc455d939c9a53d58c106ce85ec9f7f0c674299b3d974445993dc8c`  
		Last Modified: Tue, 02 Jun 2020 02:32:52 GMT  
		Size: 502.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71023d2750548230f0a4dc5e3687b6c7a8faa42933147a45edaf1d1b0e7155a`  
		Last Modified: Tue, 02 Jun 2020 02:32:52 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f722d703d3a5a30563460536bd3a850b5175ad79c43c8a9397b0b3a5c8f100d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.4 MB (318375279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcb7124899c5889d20b2be36389f5a3f3741f34b9afba1078c43835dea3cd923`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:43:41 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 23 Apr 2020 17:43:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 02:56:25 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 03:51:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 03:51:21 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 03:51:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 03:51:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 03:51:26 GMT
WORKDIR /go
# Tue, 02 Jun 2020 05:40:14 GMT
WORKDIR /src
# Tue, 02 Jun 2020 05:40:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 02 Jun 2020 05:40:17 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0
# Tue, 02 Jun 2020 05:40:19 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 02 Jun 2020 05:40:20 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 02 Jun 2020 05:41:15 GMT
RUN go get -d ./...
# Tue, 02 Jun 2020 05:41:20 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 02 Jun 2020 05:41:21 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ace047eafbdd1d41e753db1fd1004be452f749a7de56a3d24b2614a64577f5`  
		Last Modified: Thu, 23 Apr 2020 18:03:18 GMT  
		Size: 301.6 KB (301629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d0031acb1953f56f2c2592c1c5882b29aa828d45deccabbb9a1b5483090a43`  
		Last Modified: Thu, 23 Apr 2020 18:03:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c18b24b5eeba6322ca5f9b2eedb021ca9618b062bdf48b250ed4b201dc8050`  
		Last Modified: Tue, 02 Jun 2020 05:23:03 GMT  
		Size: 128.2 MB (128229189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de88420151b6ca5c6fc039fda4383cb82cf3566fa1cc6b2858d6fb47afe6ceb`  
		Last Modified: Tue, 02 Jun 2020 05:22:20 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f480e87ad21aa1d6eeb3d546b707aaaef59a9dc5dc0c6e5e14dcbe96c28cd9c`  
		Last Modified: Tue, 02 Jun 2020 05:41:39 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f74f503577c8c19df94e7f595796fd4e4e15166602d5843a4e28a694ef5e28f`  
		Last Modified: Tue, 02 Jun 2020 05:41:40 GMT  
		Size: 7.8 MB (7794708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12265e99f76b1fae972b3d710b32e05095595f8f0a5c088f78a217027939799`  
		Last Modified: Tue, 02 Jun 2020 05:41:38 GMT  
		Size: 2.7 MB (2712506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c581c17f5029909335c44e9a561b604aa98c4db79d38d9e87cae2749bcc658ce`  
		Last Modified: Tue, 02 Jun 2020 05:42:22 GMT  
		Size: 176.7 MB (176716184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57481f1b24f0912bad71decaec966f45bf686c9b218bd73fa4335d867d765ed7`  
		Last Modified: Tue, 02 Jun 2020 05:41:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd612876bd12eb68ab6685845a9b5cc04abca31e2e6292058dee233260487cf`  
		Last Modified: Tue, 02 Jun 2020 05:41:38 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0c21b0ed54253ffdfa14547e326d48beebbf4b92bb8da76b92edb8c3c6abf04c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.0 MB (317037998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4388ab5685329446df0ddd799ba01c8a93d5feb07b8e6347d7c48a4827f0ac0c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:27:40 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 24 Apr 2020 02:27:42 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:35:08 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:59:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:59:49 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:59:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:59:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:59:54 GMT
WORKDIR /go
# Tue, 02 Jun 2020 04:45:11 GMT
WORKDIR /src
# Tue, 02 Jun 2020 04:45:33 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 02 Jun 2020 04:45:42 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0
# Tue, 02 Jun 2020 04:46:08 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 02 Jun 2020 04:46:18 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 02 Jun 2020 04:48:25 GMT
RUN go get -d ./...
# Tue, 02 Jun 2020 04:48:36 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 02 Jun 2020 04:48:46 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a35d9f7887ef683587262c6f5ed88364f59775ff882c71bde03cc59f382ffd`  
		Last Modified: Fri, 24 Apr 2020 03:39:46 GMT  
		Size: 300.6 KB (300593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce21b09ea3d1107df35d9f41a664183faabfc461b8f093ab8e9a34d91e8e71b`  
		Last Modified: Fri, 24 Apr 2020 03:39:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f154a497a43d3932627d4ed19f8a725b92bc6ff032696fd7d02c923aabfdfcd`  
		Last Modified: Tue, 02 Jun 2020 03:53:43 GMT  
		Size: 127.9 MB (127859153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356485fde635696dcdacee878dba8a58e09b58537b064b5f1661e5bbede500c1`  
		Last Modified: Tue, 02 Jun 2020 03:52:31 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955b3271dbcc86df5de81f5274c182306cd2a0e95581acd9a21262668cf2b88a`  
		Last Modified: Tue, 02 Jun 2020 04:49:24 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9e684ca35cc26b7059bb60e83771de2a6b96091a053dd7ecb7b81deeb696fd`  
		Last Modified: Tue, 02 Jun 2020 04:49:20 GMT  
		Size: 7.0 MB (7026779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1d162e820fa1c08e63c96be54a52b452f50218eeeee10b1260cd22d2250215`  
		Last Modified: Tue, 02 Jun 2020 04:49:20 GMT  
		Size: 2.7 MB (2712499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8138743a5c1e38d4db8ff61f24498d97cd9294a19cd9f2c6d88e8be776aa557e`  
		Last Modified: Tue, 02 Jun 2020 04:50:16 GMT  
		Size: 176.7 MB (176715788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e9777f9df18524b4ce10bcb6db5fb00912bde1d57de9ee77e0485b7ca87149`  
		Last Modified: Tue, 02 Jun 2020 04:49:20 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dbf791500a5a018208ecaed66e5d8afc28ca5be7ae31fb54c8b02c6dc02f68`  
		Last Modified: Tue, 02 Jun 2020 04:49:20 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:fa63e1ed3b5857fc2afa0da0e5f87e46c465ca4285b2f4256f033c7d0e075e16
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.3 MB (317306406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa08366dd0271d82e7194ee208f71f532fe0ef0edc70f7f2e9ace0fe35e206c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 24 Apr 2020 09:30:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 02:01:25 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 02:05:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 02:05:51 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 02:06:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 02:07:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 02:07:23 GMT
WORKDIR /go
# Tue, 02 Jun 2020 03:54:39 GMT
WORKDIR /src
# Tue, 02 Jun 2020 03:55:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 02 Jun 2020 03:55:25 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0
# Tue, 02 Jun 2020 03:56:04 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 02 Jun 2020 03:56:07 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 02 Jun 2020 03:57:15 GMT
RUN go get -d ./...
# Tue, 02 Jun 2020 03:57:23 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 02 Jun 2020 03:57:32 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fc45ca0357821724e2824e141e2062d236dedad3d8654e0a390419ec9fe393`  
		Last Modified: Fri, 24 Apr 2020 09:38:53 GMT  
		Size: 301.8 KB (301770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6332e392c90a454bd9f70a303cda942eb0e131e321e82cb70b9346ece4a52a64`  
		Last Modified: Fri, 24 Apr 2020 09:38:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d8f54f55a2670968860ca35a8c2a0e2e526b543894d26874eae63fc6ce1532`  
		Last Modified: Tue, 02 Jun 2020 02:30:54 GMT  
		Size: 126.5 MB (126491009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2603d501b5a4a0cd3f6da1f592af79cba3b33143d7e3c4abd674ddc768193ec`  
		Last Modified: Tue, 02 Jun 2020 02:30:16 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2a6789a8ae4894bb21533776d982f6c268fcdcf9f33941f162b63755960e3b`  
		Last Modified: Tue, 02 Jun 2020 03:57:57 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248984096d3b57adf469c453ec30db708388da2d14aab956f1204e917ca27c4`  
		Last Modified: Tue, 02 Jun 2020 03:57:58 GMT  
		Size: 8.4 MB (8365435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d43f4d0862815e18a79d45498f2fbcfd99029a2863caf46b05618fd0e1cd5fd`  
		Last Modified: Tue, 02 Jun 2020 03:57:54 GMT  
		Size: 2.7 MB (2706372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bafe3a72624764aa34e658d59aff5bb317ff49f7624c43d47d9e5c575902a984`  
		Last Modified: Tue, 02 Jun 2020 03:58:33 GMT  
		Size: 176.7 MB (176716269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905e846552ef4792a1bc0924a7fafdf9fe2e669c5e91a25b222fc69a0ef958d0`  
		Last Modified: Tue, 02 Jun 2020 03:57:53 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ba0a8ecba94bf6fe06e59d7631f3e6ba4f79bbeccac3628b0b9bdb13825406`  
		Last Modified: Tue, 02 Jun 2020 03:57:53 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:6891c6d6490e09d98441446daa3f60dc3c0b1eef350bd60f15da70ce0c66e22d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.6 MB (316596303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d43482e81b370ae7732fbdf178f88ef7b057e0a406359ccbce7ad214d309fbf`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:54:40 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 24 Apr 2020 02:54:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:32:58 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:36:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:36:14 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:36:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:36:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:36:38 GMT
WORKDIR /go
# Tue, 02 Jun 2020 02:07:41 GMT
WORKDIR /src
# Tue, 02 Jun 2020 02:07:52 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 02 Jun 2020 02:07:56 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0
# Tue, 02 Jun 2020 02:08:01 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 02 Jun 2020 02:08:03 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 02 Jun 2020 02:10:04 GMT
RUN go get -d ./...
# Tue, 02 Jun 2020 02:10:07 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 02 Jun 2020 02:10:10 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20efe26326b88a40e960e9cd11fce1b701b2cf370e8328f66fc846d23b5408`  
		Last Modified: Fri, 24 Apr 2020 03:02:11 GMT  
		Size: 304.0 KB (303974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7438e1bdec433812841560459973aca70d85a3b7661615d9c632998dd366f248`  
		Last Modified: Fri, 24 Apr 2020 03:02:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665e10aea526140928afce65b052e28ac4f223162c45360135430121de27c7d7`  
		Last Modified: Tue, 02 Jun 2020 01:49:39 GMT  
		Size: 125.3 MB (125264184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1501bdd7b2a43f71acacc2d8a1122da868e702b75b2b680b69707544a4d2a6`  
		Last Modified: Tue, 02 Jun 2020 01:49:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e91f288ec567edbbf295fad3a3dadb1e59f32db4395eed7839b6ec89b8e2e1b`  
		Last Modified: Tue, 02 Jun 2020 02:10:32 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61996a2194cfe615b8d4f165ab0698f11f77f099cacb4305e2b4a48ecb23d85`  
		Last Modified: Tue, 02 Jun 2020 02:10:32 GMT  
		Size: 8.8 MB (8784628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5252de731606eac2f54796e9249033424cc547c2f7cfda78819e9bad6336d64b`  
		Last Modified: Tue, 02 Jun 2020 02:10:33 GMT  
		Size: 2.7 MB (2706339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3b270c7436a0d3b6f52d2c3ca32e87b1aa6b6cb910d93c8d8c146c281cb098`  
		Last Modified: Tue, 02 Jun 2020 02:10:57 GMT  
		Size: 176.7 MB (176714209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb2be7c1dce157b09712be8befda6ffc7db62d04638eb8de0ffcedc9c72ef9e`  
		Last Modified: Tue, 02 Jun 2020 02:10:29 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1a34918806b67ebe40004ce44428f56acf696819686c01055ec4bba3e40147`  
		Last Modified: Tue, 02 Jun 2020 02:10:30 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:947edd15c7a7b1de99ef6de49bfdba2c2f48b5ac85cdd68429a8d2b308b9fd39
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.3 MB (322334003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:732919a18d2ee22b245cf74dbe9e1e6119e7364d09f35705c4641f8ab310185b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 20:01:10 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 23 Apr 2020 20:01:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:54:47 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:56:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:56:06 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:56:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:56:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:56:07 GMT
WORKDIR /go
# Tue, 02 Jun 2020 02:18:58 GMT
WORKDIR /src
# Tue, 02 Jun 2020 02:18:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 02 Jun 2020 02:19:00 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0
# Tue, 02 Jun 2020 02:19:01 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 02 Jun 2020 02:19:01 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 02 Jun 2020 02:19:20 GMT
RUN go get -d ./...
# Tue, 02 Jun 2020 02:19:28 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 02 Jun 2020 02:19:28 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bb5699ff3d626466b57d4c92bbf8a5410490fcece2b350c368cad50778b96d`  
		Last Modified: Thu, 23 Apr 2020 20:06:33 GMT  
		Size: 301.9 KB (301908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf86b8de56aab63659ca622083cd8174db3525f6baa42836863267efa18de0e2`  
		Last Modified: Thu, 23 Apr 2020 20:06:33 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fc33aefc5654dc9f18f8874ec5df3f0054d95efb6068093b66a806c1a47e54`  
		Last Modified: Tue, 02 Jun 2020 02:02:05 GMT  
		Size: 131.8 MB (131813328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb93b54892812fb36828c107902c548f3819372e46c12a6ecc0a7f79d29bdfd7`  
		Last Modified: Tue, 02 Jun 2020 02:01:43 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b29c909e9fef1d56ec58cb008cf363dead738a814985e79695e537b0d72ea53`  
		Last Modified: Tue, 02 Jun 2020 02:19:40 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1432be465a87de431d75d8d1cf02c7e3a11afc2f17e74071f56a6992f9f79ec`  
		Last Modified: Tue, 02 Jun 2020 02:19:40 GMT  
		Size: 8.2 MB (8212445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4868624099c4b67147b2c3310067ca317b998e011da3445bd20b30e6ea4a1f83`  
		Last Modified: Tue, 02 Jun 2020 02:19:39 GMT  
		Size: 2.7 MB (2706327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7621f436be1cd0adc948c7f4c2b6047e4fdf87b7f63644e5b832ab43cbea5a38`  
		Last Modified: Tue, 02 Jun 2020 02:20:13 GMT  
		Size: 176.7 MB (176716012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7181db5ca0fa079aa4c35d3206d2913d4d544419ff434d64f403c84b766044`  
		Last Modified: Tue, 02 Jun 2020 02:19:39 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eead0c695ec3fd46a6b5f762603d74e1b7757c7fd0f547ecd1ce7f1ab5d3a5`  
		Last Modified: Tue, 02 Jun 2020 02:20:09 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:e4dedf67fc59354c08ec74b75e15f126b2761a88a35522e86d1bb43ec182ab22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64
	-	windows version 10.0.14393.3750; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:4846f66a1cfa0fa858f8ae2a6c348f14be435ca26312f365ed041203bb35f48a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2311249634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94450ec6f1472f8ab0cfd101f7f68644f92c8b2262f9ea2153fdc9a0798b3917`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Tue, 09 Jun 2020 22:33:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:02:29 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:03:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Jun 2020 18:03:16 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 10 Jun 2020 18:03:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('636bb25c9738400b480ca243a605da74988deb1bc856a1cabe7ee36511db0e048ec0a2688b1640d7b157bc239d437944e43500d91881c8acc7f2b8aa138945f9')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Jun 2020 18:03:56 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Jun 2020 18:03:56 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Jun 2020 18:03:57 GMT
VOLUME [c:/config]
# Wed, 10 Jun 2020 18:03:58 GMT
VOLUME [c:/data]
# Wed, 10 Jun 2020 18:03:59 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 10 Jun 2020 18:04:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Jun 2020 18:04:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Jun 2020 18:04:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Jun 2020 18:04:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Jun 2020 18:04:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Jun 2020 18:04:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Jun 2020 18:04:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Jun 2020 18:04:07 GMT
EXPOSE 80
# Wed, 10 Jun 2020 18:04:08 GMT
EXPOSE 443
# Wed, 10 Jun 2020 18:04:08 GMT
EXPOSE 2019
# Wed, 10 Jun 2020 18:04:31 GMT
RUN caddy version
# Wed, 10 Jun 2020 18:04:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f841c6a0c622cd36b5b2688011a224ac3e8e96273758f4a2804f2f3f099f267d`  
		Last Modified: Tue, 09 Jun 2020 23:17:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e676deb3766189ea2b008f69205017c9ee31a77f9c7001fb5a07fb2e2d4fbb0`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba576338ed5242ba3fb838ce5fa930abb61e22fc422ba46b260dbca773cb9`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 4.8 MB (4772911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82aa7b0db5bd44f058750b70c9ca192d7af8986578dd9900fa68f08a53d56d7`  
		Last Modified: Wed, 10 Jun 2020 18:09:46 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6f36d669bbd2a660d47e342775c1705e6b990b004cfb461b66aeb6d978fa60`  
		Last Modified: Wed, 10 Jun 2020 18:09:50 GMT  
		Size: 12.3 MB (12262241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4caa471f3ff12126859610d5fb7a1eee050fdcd24f4c26c840a49072698064`  
		Last Modified: Wed, 10 Jun 2020 18:09:46 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f92da22ed9f6eaba0eb6cb98ff0182e5bf96b672aa9a2a5fc004584af897f91`  
		Last Modified: Wed, 10 Jun 2020 18:09:45 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ca7d66806087b4fb8e9aba7aa8c8d913f6c00b136833ce130ad342601fbcce`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2f91baaa6ad75f37691004649e965eb02f770c8901034ec1d508ac0e198c9f`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490c3bc1055c4210b37fa961535859113aa2a9e83d5373f1edb7664fec3d44a4`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d6ca5a24db2b4dabbd352548aaabc3057e21b5b1d13a3e09ff8d5b4a9f99e4`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6b40d207638f35eb44e6d1c604c7939e68829fe4e04a1ca286eea436d3b3b5`  
		Last Modified: Wed, 10 Jun 2020 18:09:42 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d137f3abb4ef203c2caea5f8b50defc1384938cae41fab9c5f751193dd801e`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ff6d828fdc817dccd02e18fb68f60dfb77e5f91b61e4039622748fdacec123`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce68242ed36c05b1696a9aed8843408c0d3df159bdd08a6f89273aea8cf2a52`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8857e417a7cd480ddc26cd312eb34880b8e76040cd4f2ea589b21fbc5d54e274`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a31891b746d7cffa5744afba11ca2c1e207076488f863fe4cb519147cbc359`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e936bc871ff19fb19ebb325dc0b2a592fd9347488450d772e434000811f5d8c`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500e96dcc8873265379cfdace5e5c75b28080e5042969250c1656de746a3eb17`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7c3e99413b53ef84bebebfb04ec29d95aa84e3f0e040dc9cbf355afca92009`  
		Last Modified: Wed, 10 Jun 2020 18:09:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790f2340b769609f7c8716568b843cd0723c59c8dc64142f1e927d5536bd9f7c`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 278.2 KB (278231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e765bd24f285691b433b20a6296e67d067e6e2918c7e1cd2ad2bef1bbd356dfc`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:64246e00b3c6726a42b20440c70003c72bc6e652f821982345b87928bc79cae5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756998229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb6c0b59ae11bc16763ab0732bf43ae0dead1bbded3284e54191f687f4a670e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:04:40 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:06:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Jun 2020 18:06:15 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 10 Jun 2020 18:07:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('636bb25c9738400b480ca243a605da74988deb1bc856a1cabe7ee36511db0e048ec0a2688b1640d7b157bc239d437944e43500d91881c8acc7f2b8aa138945f9')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Jun 2020 18:08:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Jun 2020 18:08:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Jun 2020 18:08:03 GMT
VOLUME [c:/config]
# Wed, 10 Jun 2020 18:08:04 GMT
VOLUME [c:/data]
# Wed, 10 Jun 2020 18:08:05 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 10 Jun 2020 18:08:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Jun 2020 18:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Jun 2020 18:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Jun 2020 18:08:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Jun 2020 18:08:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Jun 2020 18:08:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Jun 2020 18:08:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Jun 2020 18:08:12 GMT
EXPOSE 80
# Wed, 10 Jun 2020 18:08:13 GMT
EXPOSE 443
# Wed, 10 Jun 2020 18:08:14 GMT
EXPOSE 2019
# Wed, 10 Jun 2020 18:09:10 GMT
RUN caddy version
# Wed, 10 Jun 2020 18:09:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22985925139cd6a6e83b6eb5286a8a6e1053a5c6ddd9762f34deea2aa6bcaacc`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43c028d6768e901bc64b3edb7e2e5f72050d3ed78ea4e7337fe85725d250c15`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 5.4 MB (5404509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab96ccdd2dbffb13487e758409eaae25905b86a83e7b7a51a692c7ff18579b8d`  
		Last Modified: Wed, 10 Jun 2020 18:10:14 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aac2a7ea7e1f98bb6027b5090912006abeb6f367523aac337f6705ba4d7bb6b`  
		Last Modified: Wed, 10 Jun 2020 18:10:19 GMT  
		Size: 17.3 MB (17325836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7acf530d8fe0b1ea1f35f0e20ca267e447936a8edbae3889184d180b44c1a6`  
		Last Modified: Wed, 10 Jun 2020 18:10:13 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7609e5df44616b1f91e5434a43518cf253a69c406c062ef6b99035b20a437`  
		Last Modified: Wed, 10 Jun 2020 18:10:13 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1384cb066181208a5bb3be7023fe3f0b9cedf5483885cf330f7dcd95525302`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f2a49d3e0a25e1871a3dcb23fa333268062b4d027ae041e3bb5c0827dd0c2a`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5ec5b8bc911e1426e8c8dcc06a149b90edee45636d75da5b63e83fe91398a`  
		Last Modified: Wed, 10 Jun 2020 18:10:12 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dab68d41796a58e20ae80dc2528cfe6a2e71a04c8c88bb5595a6e0a5d7f7646`  
		Last Modified: Wed, 10 Jun 2020 18:10:10 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68da8c08840ea413933ac718a42b86738f90a6a5647e151252d4b5193ee40a8d`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946bc1b557fc88846697a1a1308c7af5ef52918f700f7dc8bd4c53e915c4a1a3`  
		Last Modified: Wed, 10 Jun 2020 18:10:09 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7ea127cbc59b2799852a077baa3bc9e46ad415abc4de6305396739a257a25e`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e77ea136bb911d1a64b32d1d139522e0e52ca1bc43b5d12aeeef7be91483d50`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a29c745913025b3a12451ab689a6186ec7756b5d99d0fa379a39ae81d510b0b`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4ae08e24e91168918350e7422b8f47200d09a7313216990ba6a672b5372280`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e219b4ef296fd92d145bf1f1a7b7d79e09c26a996daf350eb5ee70cbfeed02`  
		Last Modified: Wed, 10 Jun 2020 18:10:05 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc81bd4365ed96954980b554e769048c1e4cc97035385e22ee8364bd2856d4af`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec6f99a5c3e003e6dd16b75770a2762bb5de2737ffdd11b1c707f6aefce201a`  
		Last Modified: Wed, 10 Jun 2020 18:10:05 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26ba6de29355852954f97260ed4e96f1d30d7e675356cc21cac59feb841cf3e`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 248.4 KB (248359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef895a3d9501c41dd42a22a3e2a0458c59b35892005f5fb18b8937101a1fb50`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:8104954610b79ec4831237b7893ddd0da8ca6886fb2d4acc184412fcdca0b72c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:4846f66a1cfa0fa858f8ae2a6c348f14be435ca26312f365ed041203bb35f48a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2311249634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94450ec6f1472f8ab0cfd101f7f68644f92c8b2262f9ea2153fdc9a0798b3917`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Tue, 09 Jun 2020 22:33:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:02:29 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:03:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Jun 2020 18:03:16 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 10 Jun 2020 18:03:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('636bb25c9738400b480ca243a605da74988deb1bc856a1cabe7ee36511db0e048ec0a2688b1640d7b157bc239d437944e43500d91881c8acc7f2b8aa138945f9')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Jun 2020 18:03:56 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Jun 2020 18:03:56 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Jun 2020 18:03:57 GMT
VOLUME [c:/config]
# Wed, 10 Jun 2020 18:03:58 GMT
VOLUME [c:/data]
# Wed, 10 Jun 2020 18:03:59 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 10 Jun 2020 18:04:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Jun 2020 18:04:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Jun 2020 18:04:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Jun 2020 18:04:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Jun 2020 18:04:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Jun 2020 18:04:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Jun 2020 18:04:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Jun 2020 18:04:07 GMT
EXPOSE 80
# Wed, 10 Jun 2020 18:04:08 GMT
EXPOSE 443
# Wed, 10 Jun 2020 18:04:08 GMT
EXPOSE 2019
# Wed, 10 Jun 2020 18:04:31 GMT
RUN caddy version
# Wed, 10 Jun 2020 18:04:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f841c6a0c622cd36b5b2688011a224ac3e8e96273758f4a2804f2f3f099f267d`  
		Last Modified: Tue, 09 Jun 2020 23:17:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e676deb3766189ea2b008f69205017c9ee31a77f9c7001fb5a07fb2e2d4fbb0`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba576338ed5242ba3fb838ce5fa930abb61e22fc422ba46b260dbca773cb9`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 4.8 MB (4772911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82aa7b0db5bd44f058750b70c9ca192d7af8986578dd9900fa68f08a53d56d7`  
		Last Modified: Wed, 10 Jun 2020 18:09:46 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6f36d669bbd2a660d47e342775c1705e6b990b004cfb461b66aeb6d978fa60`  
		Last Modified: Wed, 10 Jun 2020 18:09:50 GMT  
		Size: 12.3 MB (12262241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4caa471f3ff12126859610d5fb7a1eee050fdcd24f4c26c840a49072698064`  
		Last Modified: Wed, 10 Jun 2020 18:09:46 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f92da22ed9f6eaba0eb6cb98ff0182e5bf96b672aa9a2a5fc004584af897f91`  
		Last Modified: Wed, 10 Jun 2020 18:09:45 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ca7d66806087b4fb8e9aba7aa8c8d913f6c00b136833ce130ad342601fbcce`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2f91baaa6ad75f37691004649e965eb02f770c8901034ec1d508ac0e198c9f`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490c3bc1055c4210b37fa961535859113aa2a9e83d5373f1edb7664fec3d44a4`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d6ca5a24db2b4dabbd352548aaabc3057e21b5b1d13a3e09ff8d5b4a9f99e4`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6b40d207638f35eb44e6d1c604c7939e68829fe4e04a1ca286eea436d3b3b5`  
		Last Modified: Wed, 10 Jun 2020 18:09:42 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d137f3abb4ef203c2caea5f8b50defc1384938cae41fab9c5f751193dd801e`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ff6d828fdc817dccd02e18fb68f60dfb77e5f91b61e4039622748fdacec123`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce68242ed36c05b1696a9aed8843408c0d3df159bdd08a6f89273aea8cf2a52`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8857e417a7cd480ddc26cd312eb34880b8e76040cd4f2ea589b21fbc5d54e274`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a31891b746d7cffa5744afba11ca2c1e207076488f863fe4cb519147cbc359`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e936bc871ff19fb19ebb325dc0b2a592fd9347488450d772e434000811f5d8c`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500e96dcc8873265379cfdace5e5c75b28080e5042969250c1656de746a3eb17`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7c3e99413b53ef84bebebfb04ec29d95aa84e3f0e040dc9cbf355afca92009`  
		Last Modified: Wed, 10 Jun 2020 18:09:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790f2340b769609f7c8716568b843cd0723c59c8dc64142f1e927d5536bd9f7c`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 278.2 KB (278231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e765bd24f285691b433b20a6296e67d067e6e2918c7e1cd2ad2bef1bbd356dfc`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:c5e137c3575e37688a5ec6f3a628bde1fade7f6c99278fae9f865f24a52accc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:64246e00b3c6726a42b20440c70003c72bc6e652f821982345b87928bc79cae5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756998229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb6c0b59ae11bc16763ab0732bf43ae0dead1bbded3284e54191f687f4a670e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:04:40 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:06:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Jun 2020 18:06:15 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 10 Jun 2020 18:07:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('636bb25c9738400b480ca243a605da74988deb1bc856a1cabe7ee36511db0e048ec0a2688b1640d7b157bc239d437944e43500d91881c8acc7f2b8aa138945f9')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Jun 2020 18:08:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Jun 2020 18:08:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Jun 2020 18:08:03 GMT
VOLUME [c:/config]
# Wed, 10 Jun 2020 18:08:04 GMT
VOLUME [c:/data]
# Wed, 10 Jun 2020 18:08:05 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 10 Jun 2020 18:08:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Jun 2020 18:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Jun 2020 18:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Jun 2020 18:08:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Jun 2020 18:08:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Jun 2020 18:08:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Jun 2020 18:08:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Jun 2020 18:08:12 GMT
EXPOSE 80
# Wed, 10 Jun 2020 18:08:13 GMT
EXPOSE 443
# Wed, 10 Jun 2020 18:08:14 GMT
EXPOSE 2019
# Wed, 10 Jun 2020 18:09:10 GMT
RUN caddy version
# Wed, 10 Jun 2020 18:09:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22985925139cd6a6e83b6eb5286a8a6e1053a5c6ddd9762f34deea2aa6bcaacc`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43c028d6768e901bc64b3edb7e2e5f72050d3ed78ea4e7337fe85725d250c15`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 5.4 MB (5404509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab96ccdd2dbffb13487e758409eaae25905b86a83e7b7a51a692c7ff18579b8d`  
		Last Modified: Wed, 10 Jun 2020 18:10:14 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aac2a7ea7e1f98bb6027b5090912006abeb6f367523aac337f6705ba4d7bb6b`  
		Last Modified: Wed, 10 Jun 2020 18:10:19 GMT  
		Size: 17.3 MB (17325836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7acf530d8fe0b1ea1f35f0e20ca267e447936a8edbae3889184d180b44c1a6`  
		Last Modified: Wed, 10 Jun 2020 18:10:13 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7609e5df44616b1f91e5434a43518cf253a69c406c062ef6b99035b20a437`  
		Last Modified: Wed, 10 Jun 2020 18:10:13 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1384cb066181208a5bb3be7023fe3f0b9cedf5483885cf330f7dcd95525302`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f2a49d3e0a25e1871a3dcb23fa333268062b4d027ae041e3bb5c0827dd0c2a`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5ec5b8bc911e1426e8c8dcc06a149b90edee45636d75da5b63e83fe91398a`  
		Last Modified: Wed, 10 Jun 2020 18:10:12 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dab68d41796a58e20ae80dc2528cfe6a2e71a04c8c88bb5595a6e0a5d7f7646`  
		Last Modified: Wed, 10 Jun 2020 18:10:10 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68da8c08840ea413933ac718a42b86738f90a6a5647e151252d4b5193ee40a8d`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946bc1b557fc88846697a1a1308c7af5ef52918f700f7dc8bd4c53e915c4a1a3`  
		Last Modified: Wed, 10 Jun 2020 18:10:09 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7ea127cbc59b2799852a077baa3bc9e46ad415abc4de6305396739a257a25e`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e77ea136bb911d1a64b32d1d139522e0e52ca1bc43b5d12aeeef7be91483d50`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a29c745913025b3a12451ab689a6186ec7756b5d99d0fa379a39ae81d510b0b`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4ae08e24e91168918350e7422b8f47200d09a7313216990ba6a672b5372280`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e219b4ef296fd92d145bf1f1a7b7d79e09c26a996daf350eb5ee70cbfeed02`  
		Last Modified: Wed, 10 Jun 2020 18:10:05 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc81bd4365ed96954980b554e769048c1e4cc97035385e22ee8364bd2856d4af`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec6f99a5c3e003e6dd16b75770a2762bb5de2737ffdd11b1c707f6aefce201a`  
		Last Modified: Wed, 10 Jun 2020 18:10:05 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26ba6de29355852954f97260ed4e96f1d30d7e675356cc21cac59feb841cf3e`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 248.4 KB (248359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef895a3d9501c41dd42a22a3e2a0458c59b35892005f5fb18b8937101a1fb50`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:a985dd43871e9cb6c6ab3f9e45dd7bac9732f9f8d7c35f5d1b78a160b57bee4c
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
$ docker pull caddy@sha256:262f58e0836d0be11253e500e3b32e78e6d6149a90ed54e4a4ed5ca736e844fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15145372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:313ad00e425a86a5b5f39170ac018ada5d833fae55ab101712e80f52b4b986de`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 13:39:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 24 Apr 2020 13:39:03 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Fri, 24 Apr 2020 13:39:05 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 19:20:49 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 16:21:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:19:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:19:44 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:19:44 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:19:44 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:19:44 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:19:44 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:19:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:19:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:19:46 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:19:46 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:19:46 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:19:47 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:19:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c92d2df695a8e1549e487fe6691311b8c3ccfdd90383c6ae37c578c4465c76`  
		Last Modified: Fri, 24 Apr 2020 13:39:22 GMT  
		Size: 318.6 KB (318554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d779d752c63b3ccba5c5fbec57ae2361cef2059d83ea0770f389f1d9849ccde`  
		Last Modified: Fri, 24 Apr 2020 13:39:22 GMT  
		Size: 5.8 KB (5765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e321d52b548add190f8f5974453da203fc605ed33865ced7b83cc1e8fddc904e`  
		Last Modified: Wed, 06 May 2020 16:21:33 GMT  
		Size: 12.0 MB (12007584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c780a87c731befe76e920c134aaa9d393de1437f0c3940f40b355bc61de8f7a6`  
		Last Modified: Fri, 26 Jun 2020 01:20:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e304abe5082419b9f5b33d893544fd83a96932dcb7e064f871bee67716222091
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.4 MB (14390760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76f2894818f3ff916764fc8e6f3111c24629f11662bd03135b07492053d9dc86`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:42:29 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 23 Apr 2020 17:42:31 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Thu, 23 Apr 2020 17:42:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 18:49:25 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:49:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 00:50:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 00:50:46 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 00:50:47 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 00:50:47 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 00:50:48 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 00:50:49 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 00:50:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 00:50:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 00:50:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 00:50:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 00:50:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 00:50:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 00:50:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 00:50:55 GMT
EXPOSE 80
# Fri, 26 Jun 2020 00:50:56 GMT
EXPOSE 443
# Fri, 26 Jun 2020 00:50:57 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 00:50:58 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 00:50:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4aecf4b3c455b15219e7ae2914078c1796d34e6b1c2916aab2fa79d0aecc97`  
		Last Modified: Thu, 23 Apr 2020 17:43:07 GMT  
		Size: 318.9 KB (318932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78f3e6c459120cfcfb844a46e1d5fa39f425743ad39e3265fdb6b4c4ea312b6`  
		Last Modified: Thu, 23 Apr 2020 17:43:07 GMT  
		Size: 5.8 KB (5842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6977aa451d29e02cfa0a60ee52aadf3bfa7fad7712ac1687007cbb0bd812f996`  
		Last Modified: Wed, 06 May 2020 15:50:14 GMT  
		Size: 11.4 MB (11445896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2e1a3cae97c62afbdf067d2b1201f2e96a4ae8bb2320a3883f82fd1aec2824`  
		Last Modified: Fri, 26 Jun 2020 00:51:21 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2653b633a6ecc87fdf8ab9941be387a42f25f1c17580878c9cd47055a726d734
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14164711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87f56b16af8dc7e3d49ffb1018e82def382e00da18d024561d9c1fbc0a392938`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 23:22:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 23 Apr 2020 23:22:58 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Thu, 23 Apr 2020 23:23:03 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 18:57:29 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:57:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 00:59:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 00:59:31 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 00:59:31 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 00:59:32 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 00:59:32 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 00:59:33 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 00:59:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 00:59:34 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 00:59:35 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 00:59:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 00:59:36 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 00:59:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 00:59:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 00:59:39 GMT
EXPOSE 80
# Fri, 26 Jun 2020 00:59:39 GMT
EXPOSE 443
# Fri, 26 Jun 2020 00:59:40 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 00:59:41 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 00:59:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf760b044fed05d609c6cc0dbc0163d673af839c2bd8b93be46a9dd9b3235d8d`  
		Last Modified: Thu, 23 Apr 2020 23:23:51 GMT  
		Size: 317.9 KB (317871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702db93291bb8c691008d86b00d866d87fd9904461e56e447408436f67069d12`  
		Last Modified: Thu, 23 Apr 2020 23:23:50 GMT  
		Size: 5.8 KB (5843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a240b5e189e2da028c9e14c55e560dda7eebabe89a0fdc68bd063df8ac5403`  
		Last Modified: Wed, 06 May 2020 15:58:14 GMT  
		Size: 11.4 MB (11418780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febb3ae65834fee908dad31bb9b1fe5dbffd24c31bd7b4d6eb3f7e0cc0be6524`  
		Last Modified: Fri, 26 Jun 2020 01:00:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:d9aef3ac6d0885fa20fd11f612c78377e9b9e12bca0d92e77205e7c90e65d07c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14099502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d385c1b96da99f80af54a8b12302cb050f0b91d661b1d5d3c876b6ae33003cfc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 03:41:26 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 24 Apr 2020 03:41:27 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Fri, 24 Apr 2020 03:41:30 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 18:39:39 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 16:39:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:40:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:40:07 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:40:08 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:40:09 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:40:09 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:40:10 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:40:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:40:11 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:40:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:40:13 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:40:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:40:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:40:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:40:16 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:40:16 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:40:17 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:40:18 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:40:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1dd90474a5634d83eea66237a34342ba1aa7b9660127d7a6168f9dd16a6800`  
		Last Modified: Fri, 24 Apr 2020 03:42:02 GMT  
		Size: 319.1 KB (319109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523ce157ee2040adfd1d897f97c884c8df6de54df4581f3982d4114fea063843`  
		Last Modified: Fri, 24 Apr 2020 03:42:02 GMT  
		Size: 5.8 KB (5843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45586f3cd2c78aa4e4ec308b720449bd298ff8184489fc23ed1b63329d5bfba`  
		Last Modified: Wed, 06 May 2020 16:40:28 GMT  
		Size: 11.0 MB (11049973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f00aaba3fbdd96271be17e7a6a5b181a398f7c2f05bc510c8fb471d69578081`  
		Last Modified: Fri, 26 Jun 2020 01:40:41 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:084bd1339d1118c2e8a50d81da5761d085ebb079eb47faa49957cbcc89168f1a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14000418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c23735b817347971b241008c1dc978437390ce830fce6cf006d678d61b8b21af`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Wed, 06 May 2020 15:29:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 06 May 2020 15:30:01 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Wed, 06 May 2020 15:30:08 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Wed, 06 May 2020 15:30:10 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:30:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:18:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:18:24 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:18:27 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:18:29 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:18:33 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:18:38 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:18:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:18:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:18:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:18:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:18:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:19:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:19:04 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:19:08 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:19:12 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:19:17 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:19:21 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5a8966b60d898cbfd9fb53281860fcb82df54d8f66c9142f4038d0e3d8afb8`  
		Last Modified: Wed, 06 May 2020 15:36:35 GMT  
		Size: 321.6 KB (321641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcdcee6bf7f07bf2e87c36762756faa63a587b445b5112371d799d9983a38d7f`  
		Last Modified: Wed, 06 May 2020 15:36:34 GMT  
		Size: 5.8 KB (5845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912d87d0a8415f3b9ba60c72fc6309c0c67fb08b2834913add34eb8344ce0826`  
		Last Modified: Wed, 06 May 2020 15:36:42 GMT  
		Size: 10.9 MB (10850936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a992aa5354ab6566aa182b0b2122386db6d1143f1bfac22dc492fd1e1c9483`  
		Last Modified: Fri, 26 Jun 2020 01:20:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:16c31b5a11f0b34504a63c04a8b8a84c455e1669a3994f207a0d2d12047f7413
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14740730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d4431f588c0c1832ba15b0e102a300b97eb5374c9434a6c17cfb6ad324eee24`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Wed, 06 May 2020 15:30:02 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 06 May 2020 15:30:03 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Wed, 06 May 2020 15:30:05 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Wed, 06 May 2020 15:30:05 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:30:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:41:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:41:44 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:41:44 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:41:44 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:41:45 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:41:45 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:41:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:41:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:41:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:41:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:41:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:41:47 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:41:47 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:41:48 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:41:48 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:41:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1098bec6a96fa022c5d1e1043cbd10f41d1b5e0788cdeb71e1cbdf3ba0f6b6`  
		Last Modified: Wed, 06 May 2020 15:32:28 GMT  
		Size: 319.2 KB (319200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b06bf33ed224c71042842eaa50af6440423bb48f5cf032ce51277c7d08cb79f`  
		Last Modified: Wed, 06 May 2020 15:32:27 GMT  
		Size: 5.8 KB (5840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b3c02c4f07ca031406ddeefa20f1428b199d11370f5548cffe6bf3c294088c`  
		Last Modified: Wed, 06 May 2020 15:32:29 GMT  
		Size: 11.8 MB (11832677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b274cabb90bbeb4aafa4418e77b128c5caf6aed9aa6b6f1f756a905af241d2cd`  
		Last Modified: Fri, 26 Jun 2020 01:42:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:e7f19375fb2af512955ebfe845d8ea78b32cae8c608d367d393cbc209fc2cf3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:0750762062e92c7e2e8aa0c2c7e80d5762f6771f9c38aee0d4369b562bdad52b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.8 MB (322833946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed310fb9f0cd01f3920b3f64f1697fea83efa462d6fefdd30cc519a005c6910b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:29:00 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 24 Apr 2020 14:29:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:32:50 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:35:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:35:10 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:35:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:35:10 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:35:11 GMT
WORKDIR /go
# Tue, 02 Jun 2020 02:32:26 GMT
WORKDIR /src
# Tue, 02 Jun 2020 02:32:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 02 Jun 2020 02:32:27 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0
# Tue, 02 Jun 2020 02:32:28 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 02 Jun 2020 02:32:29 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 02 Jun 2020 02:32:42 GMT
RUN go get -d ./...
# Tue, 02 Jun 2020 02:32:42 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 02 Jun 2020 02:32:42 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408f875501273f3af2a9cbff2a23e736585641e73da80dd81712518b28e7843c`  
		Last Modified: Fri, 24 Apr 2020 14:36:50 GMT  
		Size: 301.3 KB (301282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe522b08c9798748151fec9b7a908aca712cd102cfcbb8ed79d57d05b71e6cc4`  
		Last Modified: Fri, 24 Apr 2020 14:36:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1be7d07969680a19c74f96783bb978cfc281d9eb21dd6377a1ba0c60b22161`  
		Last Modified: Tue, 02 Jun 2020 01:45:12 GMT  
		Size: 132.1 MB (132121186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed5455f4aa4c7ceedfadd2f093fffcda763951c5ae506c6d92151ad6e4dae0e`  
		Last Modified: Tue, 02 Jun 2020 01:44:46 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45598100dcda08511c93d19c558a05a901b1a183efefa4cda30b7c7e6f93d03c`  
		Last Modified: Tue, 02 Jun 2020 02:32:53 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89489597245daae1172eaaf4fc1db5044f7684053f7428c9e2b93b567d6d50d`  
		Last Modified: Tue, 02 Jun 2020 02:32:54 GMT  
		Size: 8.2 MB (8177829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc24cd02350289621830e1a9e35520aaa1bc92133dd8b9f775d5d108f93126cc`  
		Last Modified: Tue, 02 Jun 2020 02:32:52 GMT  
		Size: 2.7 MB (2706286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4dbcd3eb953512768ffac90d7561911f8d07b650519e87a8f150417c4210b3`  
		Last Modified: Tue, 02 Jun 2020 02:33:13 GMT  
		Size: 176.7 MB (176713022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461dd6e5ccc455d939c9a53d58c106ce85ec9f7f0c674299b3d974445993dc8c`  
		Last Modified: Tue, 02 Jun 2020 02:32:52 GMT  
		Size: 502.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71023d2750548230f0a4dc5e3687b6c7a8faa42933147a45edaf1d1b0e7155a`  
		Last Modified: Tue, 02 Jun 2020 02:32:52 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f722d703d3a5a30563460536bd3a850b5175ad79c43c8a9397b0b3a5c8f100d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.4 MB (318375279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcb7124899c5889d20b2be36389f5a3f3741f34b9afba1078c43835dea3cd923`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:43:41 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 23 Apr 2020 17:43:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 02:56:25 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 03:51:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 03:51:21 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 03:51:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 03:51:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 03:51:26 GMT
WORKDIR /go
# Tue, 02 Jun 2020 05:40:14 GMT
WORKDIR /src
# Tue, 02 Jun 2020 05:40:16 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 02 Jun 2020 05:40:17 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0
# Tue, 02 Jun 2020 05:40:19 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 02 Jun 2020 05:40:20 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 02 Jun 2020 05:41:15 GMT
RUN go get -d ./...
# Tue, 02 Jun 2020 05:41:20 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 02 Jun 2020 05:41:21 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ace047eafbdd1d41e753db1fd1004be452f749a7de56a3d24b2614a64577f5`  
		Last Modified: Thu, 23 Apr 2020 18:03:18 GMT  
		Size: 301.6 KB (301629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d0031acb1953f56f2c2592c1c5882b29aa828d45deccabbb9a1b5483090a43`  
		Last Modified: Thu, 23 Apr 2020 18:03:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c18b24b5eeba6322ca5f9b2eedb021ca9618b062bdf48b250ed4b201dc8050`  
		Last Modified: Tue, 02 Jun 2020 05:23:03 GMT  
		Size: 128.2 MB (128229189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de88420151b6ca5c6fc039fda4383cb82cf3566fa1cc6b2858d6fb47afe6ceb`  
		Last Modified: Tue, 02 Jun 2020 05:22:20 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f480e87ad21aa1d6eeb3d546b707aaaef59a9dc5dc0c6e5e14dcbe96c28cd9c`  
		Last Modified: Tue, 02 Jun 2020 05:41:39 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f74f503577c8c19df94e7f595796fd4e4e15166602d5843a4e28a694ef5e28f`  
		Last Modified: Tue, 02 Jun 2020 05:41:40 GMT  
		Size: 7.8 MB (7794708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12265e99f76b1fae972b3d710b32e05095595f8f0a5c088f78a217027939799`  
		Last Modified: Tue, 02 Jun 2020 05:41:38 GMT  
		Size: 2.7 MB (2712506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c581c17f5029909335c44e9a561b604aa98c4db79d38d9e87cae2749bcc658ce`  
		Last Modified: Tue, 02 Jun 2020 05:42:22 GMT  
		Size: 176.7 MB (176716184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57481f1b24f0912bad71decaec966f45bf686c9b218bd73fa4335d867d765ed7`  
		Last Modified: Tue, 02 Jun 2020 05:41:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd612876bd12eb68ab6685845a9b5cc04abca31e2e6292058dee233260487cf`  
		Last Modified: Tue, 02 Jun 2020 05:41:38 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0c21b0ed54253ffdfa14547e326d48beebbf4b92bb8da76b92edb8c3c6abf04c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.0 MB (317037998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4388ab5685329446df0ddd799ba01c8a93d5feb07b8e6347d7c48a4827f0ac0c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:27:40 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 24 Apr 2020 02:27:42 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:35:08 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:59:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:59:49 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:59:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:59:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:59:54 GMT
WORKDIR /go
# Tue, 02 Jun 2020 04:45:11 GMT
WORKDIR /src
# Tue, 02 Jun 2020 04:45:33 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 02 Jun 2020 04:45:42 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0
# Tue, 02 Jun 2020 04:46:08 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 02 Jun 2020 04:46:18 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 02 Jun 2020 04:48:25 GMT
RUN go get -d ./...
# Tue, 02 Jun 2020 04:48:36 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 02 Jun 2020 04:48:46 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a35d9f7887ef683587262c6f5ed88364f59775ff882c71bde03cc59f382ffd`  
		Last Modified: Fri, 24 Apr 2020 03:39:46 GMT  
		Size: 300.6 KB (300593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce21b09ea3d1107df35d9f41a664183faabfc461b8f093ab8e9a34d91e8e71b`  
		Last Modified: Fri, 24 Apr 2020 03:39:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f154a497a43d3932627d4ed19f8a725b92bc6ff032696fd7d02c923aabfdfcd`  
		Last Modified: Tue, 02 Jun 2020 03:53:43 GMT  
		Size: 127.9 MB (127859153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356485fde635696dcdacee878dba8a58e09b58537b064b5f1661e5bbede500c1`  
		Last Modified: Tue, 02 Jun 2020 03:52:31 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955b3271dbcc86df5de81f5274c182306cd2a0e95581acd9a21262668cf2b88a`  
		Last Modified: Tue, 02 Jun 2020 04:49:24 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9e684ca35cc26b7059bb60e83771de2a6b96091a053dd7ecb7b81deeb696fd`  
		Last Modified: Tue, 02 Jun 2020 04:49:20 GMT  
		Size: 7.0 MB (7026779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1d162e820fa1c08e63c96be54a52b452f50218eeeee10b1260cd22d2250215`  
		Last Modified: Tue, 02 Jun 2020 04:49:20 GMT  
		Size: 2.7 MB (2712499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8138743a5c1e38d4db8ff61f24498d97cd9294a19cd9f2c6d88e8be776aa557e`  
		Last Modified: Tue, 02 Jun 2020 04:50:16 GMT  
		Size: 176.7 MB (176715788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e9777f9df18524b4ce10bcb6db5fb00912bde1d57de9ee77e0485b7ca87149`  
		Last Modified: Tue, 02 Jun 2020 04:49:20 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dbf791500a5a018208ecaed66e5d8afc28ca5be7ae31fb54c8b02c6dc02f68`  
		Last Modified: Tue, 02 Jun 2020 04:49:20 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:fa63e1ed3b5857fc2afa0da0e5f87e46c465ca4285b2f4256f033c7d0e075e16
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.3 MB (317306406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa08366dd0271d82e7194ee208f71f532fe0ef0edc70f7f2e9ace0fe35e206c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 24 Apr 2020 09:30:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 02:01:25 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 02:05:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 02:05:51 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 02:06:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 02:07:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 02:07:23 GMT
WORKDIR /go
# Tue, 02 Jun 2020 03:54:39 GMT
WORKDIR /src
# Tue, 02 Jun 2020 03:55:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 02 Jun 2020 03:55:25 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0
# Tue, 02 Jun 2020 03:56:04 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 02 Jun 2020 03:56:07 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 02 Jun 2020 03:57:15 GMT
RUN go get -d ./...
# Tue, 02 Jun 2020 03:57:23 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 02 Jun 2020 03:57:32 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fc45ca0357821724e2824e141e2062d236dedad3d8654e0a390419ec9fe393`  
		Last Modified: Fri, 24 Apr 2020 09:38:53 GMT  
		Size: 301.8 KB (301770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6332e392c90a454bd9f70a303cda942eb0e131e321e82cb70b9346ece4a52a64`  
		Last Modified: Fri, 24 Apr 2020 09:38:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d8f54f55a2670968860ca35a8c2a0e2e526b543894d26874eae63fc6ce1532`  
		Last Modified: Tue, 02 Jun 2020 02:30:54 GMT  
		Size: 126.5 MB (126491009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2603d501b5a4a0cd3f6da1f592af79cba3b33143d7e3c4abd674ddc768193ec`  
		Last Modified: Tue, 02 Jun 2020 02:30:16 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2a6789a8ae4894bb21533776d982f6c268fcdcf9f33941f162b63755960e3b`  
		Last Modified: Tue, 02 Jun 2020 03:57:57 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248984096d3b57adf469c453ec30db708388da2d14aab956f1204e917ca27c4`  
		Last Modified: Tue, 02 Jun 2020 03:57:58 GMT  
		Size: 8.4 MB (8365435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d43f4d0862815e18a79d45498f2fbcfd99029a2863caf46b05618fd0e1cd5fd`  
		Last Modified: Tue, 02 Jun 2020 03:57:54 GMT  
		Size: 2.7 MB (2706372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bafe3a72624764aa34e658d59aff5bb317ff49f7624c43d47d9e5c575902a984`  
		Last Modified: Tue, 02 Jun 2020 03:58:33 GMT  
		Size: 176.7 MB (176716269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905e846552ef4792a1bc0924a7fafdf9fe2e669c5e91a25b222fc69a0ef958d0`  
		Last Modified: Tue, 02 Jun 2020 03:57:53 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ba0a8ecba94bf6fe06e59d7631f3e6ba4f79bbeccac3628b0b9bdb13825406`  
		Last Modified: Tue, 02 Jun 2020 03:57:53 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:6891c6d6490e09d98441446daa3f60dc3c0b1eef350bd60f15da70ce0c66e22d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.6 MB (316596303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d43482e81b370ae7732fbdf178f88ef7b057e0a406359ccbce7ad214d309fbf`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 02:54:40 GMT
RUN apk add --no-cache 		ca-certificates
# Fri, 24 Apr 2020 02:54:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:32:58 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:36:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:36:14 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:36:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:36:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:36:38 GMT
WORKDIR /go
# Tue, 02 Jun 2020 02:07:41 GMT
WORKDIR /src
# Tue, 02 Jun 2020 02:07:52 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 02 Jun 2020 02:07:56 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0
# Tue, 02 Jun 2020 02:08:01 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 02 Jun 2020 02:08:03 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 02 Jun 2020 02:10:04 GMT
RUN go get -d ./...
# Tue, 02 Jun 2020 02:10:07 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 02 Jun 2020 02:10:10 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20efe26326b88a40e960e9cd11fce1b701b2cf370e8328f66fc846d23b5408`  
		Last Modified: Fri, 24 Apr 2020 03:02:11 GMT  
		Size: 304.0 KB (303974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7438e1bdec433812841560459973aca70d85a3b7661615d9c632998dd366f248`  
		Last Modified: Fri, 24 Apr 2020 03:02:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665e10aea526140928afce65b052e28ac4f223162c45360135430121de27c7d7`  
		Last Modified: Tue, 02 Jun 2020 01:49:39 GMT  
		Size: 125.3 MB (125264184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1501bdd7b2a43f71acacc2d8a1122da868e702b75b2b680b69707544a4d2a6`  
		Last Modified: Tue, 02 Jun 2020 01:49:09 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e91f288ec567edbbf295fad3a3dadb1e59f32db4395eed7839b6ec89b8e2e1b`  
		Last Modified: Tue, 02 Jun 2020 02:10:32 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61996a2194cfe615b8d4f165ab0698f11f77f099cacb4305e2b4a48ecb23d85`  
		Last Modified: Tue, 02 Jun 2020 02:10:32 GMT  
		Size: 8.8 MB (8784628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5252de731606eac2f54796e9249033424cc547c2f7cfda78819e9bad6336d64b`  
		Last Modified: Tue, 02 Jun 2020 02:10:33 GMT  
		Size: 2.7 MB (2706339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3b270c7436a0d3b6f52d2c3ca32e87b1aa6b6cb910d93c8d8c146c281cb098`  
		Last Modified: Tue, 02 Jun 2020 02:10:57 GMT  
		Size: 176.7 MB (176714209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb2be7c1dce157b09712be8befda6ffc7db62d04638eb8de0ffcedc9c72ef9e`  
		Last Modified: Tue, 02 Jun 2020 02:10:29 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1a34918806b67ebe40004ce44428f56acf696819686c01055ec4bba3e40147`  
		Last Modified: Tue, 02 Jun 2020 02:10:30 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:947edd15c7a7b1de99ef6de49bfdba2c2f48b5ac85cdd68429a8d2b308b9fd39
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.3 MB (322334003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:732919a18d2ee22b245cf74dbe9e1e6119e7364d09f35705c4641f8ab310185b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 20:01:10 GMT
RUN apk add --no-cache 		ca-certificates
# Thu, 23 Apr 2020 20:01:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:54:47 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:56:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:56:06 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:56:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:56:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:56:07 GMT
WORKDIR /go
# Tue, 02 Jun 2020 02:18:58 GMT
WORKDIR /src
# Tue, 02 Jun 2020 02:18:59 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 02 Jun 2020 02:19:00 GMT
ENV CADDY_SOURCE_VERSION=v2.0.0
# Tue, 02 Jun 2020 02:19:01 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 02 Jun 2020 02:19:01 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 02 Jun 2020 02:19:20 GMT
RUN go get -d ./...
# Tue, 02 Jun 2020 02:19:28 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 02 Jun 2020 02:19:28 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bb5699ff3d626466b57d4c92bbf8a5410490fcece2b350c368cad50778b96d`  
		Last Modified: Thu, 23 Apr 2020 20:06:33 GMT  
		Size: 301.9 KB (301908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf86b8de56aab63659ca622083cd8174db3525f6baa42836863267efa18de0e2`  
		Last Modified: Thu, 23 Apr 2020 20:06:33 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fc33aefc5654dc9f18f8874ec5df3f0054d95efb6068093b66a806c1a47e54`  
		Last Modified: Tue, 02 Jun 2020 02:02:05 GMT  
		Size: 131.8 MB (131813328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb93b54892812fb36828c107902c548f3819372e46c12a6ecc0a7f79d29bdfd7`  
		Last Modified: Tue, 02 Jun 2020 02:01:43 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b29c909e9fef1d56ec58cb008cf363dead738a814985e79695e537b0d72ea53`  
		Last Modified: Tue, 02 Jun 2020 02:19:40 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1432be465a87de431d75d8d1cf02c7e3a11afc2f17e74071f56a6992f9f79ec`  
		Last Modified: Tue, 02 Jun 2020 02:19:40 GMT  
		Size: 8.2 MB (8212445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4868624099c4b67147b2c3310067ca317b998e011da3445bd20b30e6ea4a1f83`  
		Last Modified: Tue, 02 Jun 2020 02:19:39 GMT  
		Size: 2.7 MB (2706327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7621f436be1cd0adc948c7f4c2b6047e4fdf87b7f63644e5b832ab43cbea5a38`  
		Last Modified: Tue, 02 Jun 2020 02:20:13 GMT  
		Size: 176.7 MB (176716012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7181db5ca0fa079aa4c35d3206d2913d4d544419ff434d64f403c84b766044`  
		Last Modified: Tue, 02 Jun 2020 02:19:39 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eead0c695ec3fd46a6b5f762603d74e1b7757c7fd0f547ecd1ce7f1ab5d3a5`  
		Last Modified: Tue, 02 Jun 2020 02:20:09 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:906e32bdd357959838cd20f8a5fdb487afe307542c31b0269d9cb5c3731d0ca5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1282; amd64
	-	windows version 10.0.14393.3750; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:262f58e0836d0be11253e500e3b32e78e6d6149a90ed54e4a4ed5ca736e844fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15145372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:313ad00e425a86a5b5f39170ac018ada5d833fae55ab101712e80f52b4b986de`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 13:39:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 24 Apr 2020 13:39:03 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Fri, 24 Apr 2020 13:39:05 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 19:20:49 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 16:21:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:19:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:19:44 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:19:44 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:19:44 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:19:44 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:19:44 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:19:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:19:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:19:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:19:46 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:19:46 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:19:46 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:19:47 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:19:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c92d2df695a8e1549e487fe6691311b8c3ccfdd90383c6ae37c578c4465c76`  
		Last Modified: Fri, 24 Apr 2020 13:39:22 GMT  
		Size: 318.6 KB (318554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d779d752c63b3ccba5c5fbec57ae2361cef2059d83ea0770f389f1d9849ccde`  
		Last Modified: Fri, 24 Apr 2020 13:39:22 GMT  
		Size: 5.8 KB (5765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e321d52b548add190f8f5974453da203fc605ed33865ced7b83cc1e8fddc904e`  
		Last Modified: Wed, 06 May 2020 16:21:33 GMT  
		Size: 12.0 MB (12007584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c780a87c731befe76e920c134aaa9d393de1437f0c3940f40b355bc61de8f7a6`  
		Last Modified: Fri, 26 Jun 2020 01:20:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e304abe5082419b9f5b33d893544fd83a96932dcb7e064f871bee67716222091
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.4 MB (14390760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76f2894818f3ff916764fc8e6f3111c24629f11662bd03135b07492053d9dc86`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:42:29 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 23 Apr 2020 17:42:31 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Thu, 23 Apr 2020 17:42:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 18:49:25 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:49:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 00:50:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 00:50:46 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 00:50:47 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 00:50:47 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 00:50:48 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 00:50:49 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 00:50:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 00:50:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 00:50:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 00:50:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 00:50:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 00:50:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 00:50:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 00:50:55 GMT
EXPOSE 80
# Fri, 26 Jun 2020 00:50:56 GMT
EXPOSE 443
# Fri, 26 Jun 2020 00:50:57 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 00:50:58 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 00:50:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4aecf4b3c455b15219e7ae2914078c1796d34e6b1c2916aab2fa79d0aecc97`  
		Last Modified: Thu, 23 Apr 2020 17:43:07 GMT  
		Size: 318.9 KB (318932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78f3e6c459120cfcfb844a46e1d5fa39f425743ad39e3265fdb6b4c4ea312b6`  
		Last Modified: Thu, 23 Apr 2020 17:43:07 GMT  
		Size: 5.8 KB (5842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6977aa451d29e02cfa0a60ee52aadf3bfa7fad7712ac1687007cbb0bd812f996`  
		Last Modified: Wed, 06 May 2020 15:50:14 GMT  
		Size: 11.4 MB (11445896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2e1a3cae97c62afbdf067d2b1201f2e96a4ae8bb2320a3883f82fd1aec2824`  
		Last Modified: Fri, 26 Jun 2020 00:51:21 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2653b633a6ecc87fdf8ab9941be387a42f25f1c17580878c9cd47055a726d734
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14164711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87f56b16af8dc7e3d49ffb1018e82def382e00da18d024561d9c1fbc0a392938`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 23:22:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 23 Apr 2020 23:22:58 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Thu, 23 Apr 2020 23:23:03 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 18:57:29 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:57:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 00:59:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 00:59:31 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 00:59:31 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 00:59:32 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 00:59:32 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 00:59:33 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 00:59:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 00:59:34 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 00:59:35 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 00:59:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 00:59:36 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 00:59:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 00:59:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 00:59:39 GMT
EXPOSE 80
# Fri, 26 Jun 2020 00:59:39 GMT
EXPOSE 443
# Fri, 26 Jun 2020 00:59:40 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 00:59:41 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 00:59:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf760b044fed05d609c6cc0dbc0163d673af839c2bd8b93be46a9dd9b3235d8d`  
		Last Modified: Thu, 23 Apr 2020 23:23:51 GMT  
		Size: 317.9 KB (317871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702db93291bb8c691008d86b00d866d87fd9904461e56e447408436f67069d12`  
		Last Modified: Thu, 23 Apr 2020 23:23:50 GMT  
		Size: 5.8 KB (5843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a240b5e189e2da028c9e14c55e560dda7eebabe89a0fdc68bd063df8ac5403`  
		Last Modified: Wed, 06 May 2020 15:58:14 GMT  
		Size: 11.4 MB (11418780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febb3ae65834fee908dad31bb9b1fe5dbffd24c31bd7b4d6eb3f7e0cc0be6524`  
		Last Modified: Fri, 26 Jun 2020 01:00:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:d9aef3ac6d0885fa20fd11f612c78377e9b9e12bca0d92e77205e7c90e65d07c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14099502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d385c1b96da99f80af54a8b12302cb050f0b91d661b1d5d3c876b6ae33003cfc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 03:41:26 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 24 Apr 2020 03:41:27 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Fri, 24 Apr 2020 03:41:30 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 04 May 2020 18:39:39 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 16:39:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:40:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:40:07 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:40:08 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:40:09 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:40:09 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:40:10 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:40:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:40:11 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:40:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:40:13 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:40:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:40:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:40:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:40:16 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:40:16 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:40:17 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:40:18 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:40:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1dd90474a5634d83eea66237a34342ba1aa7b9660127d7a6168f9dd16a6800`  
		Last Modified: Fri, 24 Apr 2020 03:42:02 GMT  
		Size: 319.1 KB (319109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523ce157ee2040adfd1d897f97c884c8df6de54df4581f3982d4114fea063843`  
		Last Modified: Fri, 24 Apr 2020 03:42:02 GMT  
		Size: 5.8 KB (5843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45586f3cd2c78aa4e4ec308b720449bd298ff8184489fc23ed1b63329d5bfba`  
		Last Modified: Wed, 06 May 2020 16:40:28 GMT  
		Size: 11.0 MB (11049973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f00aaba3fbdd96271be17e7a6a5b181a398f7c2f05bc510c8fb471d69578081`  
		Last Modified: Fri, 26 Jun 2020 01:40:41 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:084bd1339d1118c2e8a50d81da5761d085ebb079eb47faa49957cbcc89168f1a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14000418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c23735b817347971b241008c1dc978437390ce830fce6cf006d678d61b8b21af`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Wed, 06 May 2020 15:29:56 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 06 May 2020 15:30:01 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Wed, 06 May 2020 15:30:08 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Wed, 06 May 2020 15:30:10 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:30:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:18:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:18:24 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:18:27 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:18:29 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:18:33 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:18:38 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:18:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:18:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:18:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:18:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:18:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:19:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:19:04 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:19:08 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:19:12 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:19:17 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:19:21 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5a8966b60d898cbfd9fb53281860fcb82df54d8f66c9142f4038d0e3d8afb8`  
		Last Modified: Wed, 06 May 2020 15:36:35 GMT  
		Size: 321.6 KB (321641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcdcee6bf7f07bf2e87c36762756faa63a587b445b5112371d799d9983a38d7f`  
		Last Modified: Wed, 06 May 2020 15:36:34 GMT  
		Size: 5.8 KB (5845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912d87d0a8415f3b9ba60c72fc6309c0c67fb08b2834913add34eb8344ce0826`  
		Last Modified: Wed, 06 May 2020 15:36:42 GMT  
		Size: 10.9 MB (10850936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a992aa5354ab6566aa182b0b2122386db6d1143f1bfac22dc492fd1e1c9483`  
		Last Modified: Fri, 26 Jun 2020 01:20:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:16c31b5a11f0b34504a63c04a8b8a84c455e1669a3994f207a0d2d12047f7413
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14740730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d4431f588c0c1832ba15b0e102a300b97eb5374c9434a6c17cfb6ad324eee24`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Wed, 06 May 2020 15:30:02 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 06 May 2020 15:30:03 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Wed, 06 May 2020 15:30:05 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Wed, 06 May 2020 15:30:05 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 06 May 2020 15:30:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2440fed6d7e240cedc92fd570893ad056195386e369960e1fba3a4de5dbce32871e809841acc926b0cef0afb6ded39073748afe9c39745fb5609472d495d2828' ;; 		s390x)   binArch='s390x'; checksum='b09561e089a0d2deeedfccbd8f0a608068dbc986dc7f1118f0a24e50b5173d90482e1105f9e3249381f2d4815ca316fb7e343fed82b75ea2b070c039bd76324b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 26 Jun 2020 01:41:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Jun 2020 01:41:44 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 26 Jun 2020 01:41:44 GMT
ENV XDG_DATA_HOME=/data
# Fri, 26 Jun 2020 01:41:44 GMT
VOLUME [/config]
# Fri, 26 Jun 2020 01:41:45 GMT
VOLUME [/data]
# Fri, 26 Jun 2020 01:41:45 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Fri, 26 Jun 2020 01:41:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 26 Jun 2020 01:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 26 Jun 2020 01:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 26 Jun 2020 01:41:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 26 Jun 2020 01:41:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 26 Jun 2020 01:41:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 26 Jun 2020 01:41:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 26 Jun 2020 01:41:47 GMT
EXPOSE 80
# Fri, 26 Jun 2020 01:41:47 GMT
EXPOSE 443
# Fri, 26 Jun 2020 01:41:48 GMT
EXPOSE 2019
# Fri, 26 Jun 2020 01:41:48 GMT
WORKDIR /srv
# Fri, 26 Jun 2020 01:41:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1098bec6a96fa022c5d1e1043cbd10f41d1b5e0788cdeb71e1cbdf3ba0f6b6`  
		Last Modified: Wed, 06 May 2020 15:32:28 GMT  
		Size: 319.2 KB (319200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b06bf33ed224c71042842eaa50af6440423bb48f5cf032ce51277c7d08cb79f`  
		Last Modified: Wed, 06 May 2020 15:32:27 GMT  
		Size: 5.8 KB (5840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b3c02c4f07ca031406ddeefa20f1428b199d11370f5548cffe6bf3c294088c`  
		Last Modified: Wed, 06 May 2020 15:32:29 GMT  
		Size: 11.8 MB (11832677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b274cabb90bbeb4aafa4418e77b128c5caf6aed9aa6b6f1f756a905af241d2cd`  
		Last Modified: Fri, 26 Jun 2020 01:42:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:4846f66a1cfa0fa858f8ae2a6c348f14be435ca26312f365ed041203bb35f48a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2311249634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94450ec6f1472f8ab0cfd101f7f68644f92c8b2262f9ea2153fdc9a0798b3917`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Tue, 09 Jun 2020 22:33:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:02:29 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:03:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Jun 2020 18:03:16 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 10 Jun 2020 18:03:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('636bb25c9738400b480ca243a605da74988deb1bc856a1cabe7ee36511db0e048ec0a2688b1640d7b157bc239d437944e43500d91881c8acc7f2b8aa138945f9')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Jun 2020 18:03:56 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Jun 2020 18:03:56 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Jun 2020 18:03:57 GMT
VOLUME [c:/config]
# Wed, 10 Jun 2020 18:03:58 GMT
VOLUME [c:/data]
# Wed, 10 Jun 2020 18:03:59 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 10 Jun 2020 18:04:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Jun 2020 18:04:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Jun 2020 18:04:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Jun 2020 18:04:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Jun 2020 18:04:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Jun 2020 18:04:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Jun 2020 18:04:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Jun 2020 18:04:07 GMT
EXPOSE 80
# Wed, 10 Jun 2020 18:04:08 GMT
EXPOSE 443
# Wed, 10 Jun 2020 18:04:08 GMT
EXPOSE 2019
# Wed, 10 Jun 2020 18:04:31 GMT
RUN caddy version
# Wed, 10 Jun 2020 18:04:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f841c6a0c622cd36b5b2688011a224ac3e8e96273758f4a2804f2f3f099f267d`  
		Last Modified: Tue, 09 Jun 2020 23:17:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e676deb3766189ea2b008f69205017c9ee31a77f9c7001fb5a07fb2e2d4fbb0`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba576338ed5242ba3fb838ce5fa930abb61e22fc422ba46b260dbca773cb9`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 4.8 MB (4772911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82aa7b0db5bd44f058750b70c9ca192d7af8986578dd9900fa68f08a53d56d7`  
		Last Modified: Wed, 10 Jun 2020 18:09:46 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6f36d669bbd2a660d47e342775c1705e6b990b004cfb461b66aeb6d978fa60`  
		Last Modified: Wed, 10 Jun 2020 18:09:50 GMT  
		Size: 12.3 MB (12262241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4caa471f3ff12126859610d5fb7a1eee050fdcd24f4c26c840a49072698064`  
		Last Modified: Wed, 10 Jun 2020 18:09:46 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f92da22ed9f6eaba0eb6cb98ff0182e5bf96b672aa9a2a5fc004584af897f91`  
		Last Modified: Wed, 10 Jun 2020 18:09:45 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ca7d66806087b4fb8e9aba7aa8c8d913f6c00b136833ce130ad342601fbcce`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2f91baaa6ad75f37691004649e965eb02f770c8901034ec1d508ac0e198c9f`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490c3bc1055c4210b37fa961535859113aa2a9e83d5373f1edb7664fec3d44a4`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d6ca5a24db2b4dabbd352548aaabc3057e21b5b1d13a3e09ff8d5b4a9f99e4`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6b40d207638f35eb44e6d1c604c7939e68829fe4e04a1ca286eea436d3b3b5`  
		Last Modified: Wed, 10 Jun 2020 18:09:42 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d137f3abb4ef203c2caea5f8b50defc1384938cae41fab9c5f751193dd801e`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ff6d828fdc817dccd02e18fb68f60dfb77e5f91b61e4039622748fdacec123`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce68242ed36c05b1696a9aed8843408c0d3df159bdd08a6f89273aea8cf2a52`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8857e417a7cd480ddc26cd312eb34880b8e76040cd4f2ea589b21fbc5d54e274`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a31891b746d7cffa5744afba11ca2c1e207076488f863fe4cb519147cbc359`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e936bc871ff19fb19ebb325dc0b2a592fd9347488450d772e434000811f5d8c`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500e96dcc8873265379cfdace5e5c75b28080e5042969250c1656de746a3eb17`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7c3e99413b53ef84bebebfb04ec29d95aa84e3f0e040dc9cbf355afca92009`  
		Last Modified: Wed, 10 Jun 2020 18:09:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790f2340b769609f7c8716568b843cd0723c59c8dc64142f1e927d5536bd9f7c`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 278.2 KB (278231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e765bd24f285691b433b20a6296e67d067e6e2918c7e1cd2ad2bef1bbd356dfc`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:64246e00b3c6726a42b20440c70003c72bc6e652f821982345b87928bc79cae5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756998229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb6c0b59ae11bc16763ab0732bf43ae0dead1bbded3284e54191f687f4a670e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:04:40 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:06:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Jun 2020 18:06:15 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 10 Jun 2020 18:07:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('636bb25c9738400b480ca243a605da74988deb1bc856a1cabe7ee36511db0e048ec0a2688b1640d7b157bc239d437944e43500d91881c8acc7f2b8aa138945f9')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Jun 2020 18:08:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Jun 2020 18:08:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Jun 2020 18:08:03 GMT
VOLUME [c:/config]
# Wed, 10 Jun 2020 18:08:04 GMT
VOLUME [c:/data]
# Wed, 10 Jun 2020 18:08:05 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 10 Jun 2020 18:08:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Jun 2020 18:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Jun 2020 18:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Jun 2020 18:08:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Jun 2020 18:08:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Jun 2020 18:08:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Jun 2020 18:08:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Jun 2020 18:08:12 GMT
EXPOSE 80
# Wed, 10 Jun 2020 18:08:13 GMT
EXPOSE 443
# Wed, 10 Jun 2020 18:08:14 GMT
EXPOSE 2019
# Wed, 10 Jun 2020 18:09:10 GMT
RUN caddy version
# Wed, 10 Jun 2020 18:09:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22985925139cd6a6e83b6eb5286a8a6e1053a5c6ddd9762f34deea2aa6bcaacc`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43c028d6768e901bc64b3edb7e2e5f72050d3ed78ea4e7337fe85725d250c15`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 5.4 MB (5404509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab96ccdd2dbffb13487e758409eaae25905b86a83e7b7a51a692c7ff18579b8d`  
		Last Modified: Wed, 10 Jun 2020 18:10:14 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aac2a7ea7e1f98bb6027b5090912006abeb6f367523aac337f6705ba4d7bb6b`  
		Last Modified: Wed, 10 Jun 2020 18:10:19 GMT  
		Size: 17.3 MB (17325836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7acf530d8fe0b1ea1f35f0e20ca267e447936a8edbae3889184d180b44c1a6`  
		Last Modified: Wed, 10 Jun 2020 18:10:13 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7609e5df44616b1f91e5434a43518cf253a69c406c062ef6b99035b20a437`  
		Last Modified: Wed, 10 Jun 2020 18:10:13 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1384cb066181208a5bb3be7023fe3f0b9cedf5483885cf330f7dcd95525302`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f2a49d3e0a25e1871a3dcb23fa333268062b4d027ae041e3bb5c0827dd0c2a`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5ec5b8bc911e1426e8c8dcc06a149b90edee45636d75da5b63e83fe91398a`  
		Last Modified: Wed, 10 Jun 2020 18:10:12 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dab68d41796a58e20ae80dc2528cfe6a2e71a04c8c88bb5595a6e0a5d7f7646`  
		Last Modified: Wed, 10 Jun 2020 18:10:10 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68da8c08840ea413933ac718a42b86738f90a6a5647e151252d4b5193ee40a8d`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946bc1b557fc88846697a1a1308c7af5ef52918f700f7dc8bd4c53e915c4a1a3`  
		Last Modified: Wed, 10 Jun 2020 18:10:09 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7ea127cbc59b2799852a077baa3bc9e46ad415abc4de6305396739a257a25e`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e77ea136bb911d1a64b32d1d139522e0e52ca1bc43b5d12aeeef7be91483d50`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a29c745913025b3a12451ab689a6186ec7756b5d99d0fa379a39ae81d510b0b`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4ae08e24e91168918350e7422b8f47200d09a7313216990ba6a672b5372280`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e219b4ef296fd92d145bf1f1a7b7d79e09c26a996daf350eb5ee70cbfeed02`  
		Last Modified: Wed, 10 Jun 2020 18:10:05 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc81bd4365ed96954980b554e769048c1e4cc97035385e22ee8364bd2856d4af`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec6f99a5c3e003e6dd16b75770a2762bb5de2737ffdd11b1c707f6aefce201a`  
		Last Modified: Wed, 10 Jun 2020 18:10:05 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26ba6de29355852954f97260ed4e96f1d30d7e675356cc21cac59feb841cf3e`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 248.4 KB (248359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef895a3d9501c41dd42a22a3e2a0458c59b35892005f5fb18b8937101a1fb50`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:e4dedf67fc59354c08ec74b75e15f126b2761a88a35522e86d1bb43ec182ab22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64
	-	windows version 10.0.14393.3750; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:4846f66a1cfa0fa858f8ae2a6c348f14be435ca26312f365ed041203bb35f48a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2311249634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94450ec6f1472f8ab0cfd101f7f68644f92c8b2262f9ea2153fdc9a0798b3917`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Tue, 09 Jun 2020 22:33:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:02:29 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:03:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Jun 2020 18:03:16 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 10 Jun 2020 18:03:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('636bb25c9738400b480ca243a605da74988deb1bc856a1cabe7ee36511db0e048ec0a2688b1640d7b157bc239d437944e43500d91881c8acc7f2b8aa138945f9')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Jun 2020 18:03:56 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Jun 2020 18:03:56 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Jun 2020 18:03:57 GMT
VOLUME [c:/config]
# Wed, 10 Jun 2020 18:03:58 GMT
VOLUME [c:/data]
# Wed, 10 Jun 2020 18:03:59 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 10 Jun 2020 18:04:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Jun 2020 18:04:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Jun 2020 18:04:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Jun 2020 18:04:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Jun 2020 18:04:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Jun 2020 18:04:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Jun 2020 18:04:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Jun 2020 18:04:07 GMT
EXPOSE 80
# Wed, 10 Jun 2020 18:04:08 GMT
EXPOSE 443
# Wed, 10 Jun 2020 18:04:08 GMT
EXPOSE 2019
# Wed, 10 Jun 2020 18:04:31 GMT
RUN caddy version
# Wed, 10 Jun 2020 18:04:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f841c6a0c622cd36b5b2688011a224ac3e8e96273758f4a2804f2f3f099f267d`  
		Last Modified: Tue, 09 Jun 2020 23:17:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e676deb3766189ea2b008f69205017c9ee31a77f9c7001fb5a07fb2e2d4fbb0`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba576338ed5242ba3fb838ce5fa930abb61e22fc422ba46b260dbca773cb9`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 4.8 MB (4772911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82aa7b0db5bd44f058750b70c9ca192d7af8986578dd9900fa68f08a53d56d7`  
		Last Modified: Wed, 10 Jun 2020 18:09:46 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6f36d669bbd2a660d47e342775c1705e6b990b004cfb461b66aeb6d978fa60`  
		Last Modified: Wed, 10 Jun 2020 18:09:50 GMT  
		Size: 12.3 MB (12262241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4caa471f3ff12126859610d5fb7a1eee050fdcd24f4c26c840a49072698064`  
		Last Modified: Wed, 10 Jun 2020 18:09:46 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f92da22ed9f6eaba0eb6cb98ff0182e5bf96b672aa9a2a5fc004584af897f91`  
		Last Modified: Wed, 10 Jun 2020 18:09:45 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ca7d66806087b4fb8e9aba7aa8c8d913f6c00b136833ce130ad342601fbcce`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2f91baaa6ad75f37691004649e965eb02f770c8901034ec1d508ac0e198c9f`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490c3bc1055c4210b37fa961535859113aa2a9e83d5373f1edb7664fec3d44a4`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d6ca5a24db2b4dabbd352548aaabc3057e21b5b1d13a3e09ff8d5b4a9f99e4`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6b40d207638f35eb44e6d1c604c7939e68829fe4e04a1ca286eea436d3b3b5`  
		Last Modified: Wed, 10 Jun 2020 18:09:42 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d137f3abb4ef203c2caea5f8b50defc1384938cae41fab9c5f751193dd801e`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ff6d828fdc817dccd02e18fb68f60dfb77e5f91b61e4039622748fdacec123`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce68242ed36c05b1696a9aed8843408c0d3df159bdd08a6f89273aea8cf2a52`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8857e417a7cd480ddc26cd312eb34880b8e76040cd4f2ea589b21fbc5d54e274`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a31891b746d7cffa5744afba11ca2c1e207076488f863fe4cb519147cbc359`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e936bc871ff19fb19ebb325dc0b2a592fd9347488450d772e434000811f5d8c`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500e96dcc8873265379cfdace5e5c75b28080e5042969250c1656de746a3eb17`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7c3e99413b53ef84bebebfb04ec29d95aa84e3f0e040dc9cbf355afca92009`  
		Last Modified: Wed, 10 Jun 2020 18:09:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790f2340b769609f7c8716568b843cd0723c59c8dc64142f1e927d5536bd9f7c`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 278.2 KB (278231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e765bd24f285691b433b20a6296e67d067e6e2918c7e1cd2ad2bef1bbd356dfc`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:64246e00b3c6726a42b20440c70003c72bc6e652f821982345b87928bc79cae5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756998229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb6c0b59ae11bc16763ab0732bf43ae0dead1bbded3284e54191f687f4a670e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:04:40 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:06:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Jun 2020 18:06:15 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 10 Jun 2020 18:07:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('636bb25c9738400b480ca243a605da74988deb1bc856a1cabe7ee36511db0e048ec0a2688b1640d7b157bc239d437944e43500d91881c8acc7f2b8aa138945f9')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Jun 2020 18:08:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Jun 2020 18:08:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Jun 2020 18:08:03 GMT
VOLUME [c:/config]
# Wed, 10 Jun 2020 18:08:04 GMT
VOLUME [c:/data]
# Wed, 10 Jun 2020 18:08:05 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 10 Jun 2020 18:08:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Jun 2020 18:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Jun 2020 18:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Jun 2020 18:08:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Jun 2020 18:08:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Jun 2020 18:08:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Jun 2020 18:08:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Jun 2020 18:08:12 GMT
EXPOSE 80
# Wed, 10 Jun 2020 18:08:13 GMT
EXPOSE 443
# Wed, 10 Jun 2020 18:08:14 GMT
EXPOSE 2019
# Wed, 10 Jun 2020 18:09:10 GMT
RUN caddy version
# Wed, 10 Jun 2020 18:09:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22985925139cd6a6e83b6eb5286a8a6e1053a5c6ddd9762f34deea2aa6bcaacc`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43c028d6768e901bc64b3edb7e2e5f72050d3ed78ea4e7337fe85725d250c15`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 5.4 MB (5404509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab96ccdd2dbffb13487e758409eaae25905b86a83e7b7a51a692c7ff18579b8d`  
		Last Modified: Wed, 10 Jun 2020 18:10:14 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aac2a7ea7e1f98bb6027b5090912006abeb6f367523aac337f6705ba4d7bb6b`  
		Last Modified: Wed, 10 Jun 2020 18:10:19 GMT  
		Size: 17.3 MB (17325836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7acf530d8fe0b1ea1f35f0e20ca267e447936a8edbae3889184d180b44c1a6`  
		Last Modified: Wed, 10 Jun 2020 18:10:13 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7609e5df44616b1f91e5434a43518cf253a69c406c062ef6b99035b20a437`  
		Last Modified: Wed, 10 Jun 2020 18:10:13 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1384cb066181208a5bb3be7023fe3f0b9cedf5483885cf330f7dcd95525302`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f2a49d3e0a25e1871a3dcb23fa333268062b4d027ae041e3bb5c0827dd0c2a`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5ec5b8bc911e1426e8c8dcc06a149b90edee45636d75da5b63e83fe91398a`  
		Last Modified: Wed, 10 Jun 2020 18:10:12 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dab68d41796a58e20ae80dc2528cfe6a2e71a04c8c88bb5595a6e0a5d7f7646`  
		Last Modified: Wed, 10 Jun 2020 18:10:10 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68da8c08840ea413933ac718a42b86738f90a6a5647e151252d4b5193ee40a8d`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946bc1b557fc88846697a1a1308c7af5ef52918f700f7dc8bd4c53e915c4a1a3`  
		Last Modified: Wed, 10 Jun 2020 18:10:09 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7ea127cbc59b2799852a077baa3bc9e46ad415abc4de6305396739a257a25e`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e77ea136bb911d1a64b32d1d139522e0e52ca1bc43b5d12aeeef7be91483d50`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a29c745913025b3a12451ab689a6186ec7756b5d99d0fa379a39ae81d510b0b`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4ae08e24e91168918350e7422b8f47200d09a7313216990ba6a672b5372280`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e219b4ef296fd92d145bf1f1a7b7d79e09c26a996daf350eb5ee70cbfeed02`  
		Last Modified: Wed, 10 Jun 2020 18:10:05 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc81bd4365ed96954980b554e769048c1e4cc97035385e22ee8364bd2856d4af`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec6f99a5c3e003e6dd16b75770a2762bb5de2737ffdd11b1c707f6aefce201a`  
		Last Modified: Wed, 10 Jun 2020 18:10:05 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26ba6de29355852954f97260ed4e96f1d30d7e675356cc21cac59feb841cf3e`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 248.4 KB (248359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef895a3d9501c41dd42a22a3e2a0458c59b35892005f5fb18b8937101a1fb50`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:8104954610b79ec4831237b7893ddd0da8ca6886fb2d4acc184412fcdca0b72c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:4846f66a1cfa0fa858f8ae2a6c348f14be435ca26312f365ed041203bb35f48a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2311249634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94450ec6f1472f8ab0cfd101f7f68644f92c8b2262f9ea2153fdc9a0798b3917`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Tue, 09 Jun 2020 22:33:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:02:29 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:03:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Jun 2020 18:03:16 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 10 Jun 2020 18:03:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('636bb25c9738400b480ca243a605da74988deb1bc856a1cabe7ee36511db0e048ec0a2688b1640d7b157bc239d437944e43500d91881c8acc7f2b8aa138945f9')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Jun 2020 18:03:56 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Jun 2020 18:03:56 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Jun 2020 18:03:57 GMT
VOLUME [c:/config]
# Wed, 10 Jun 2020 18:03:58 GMT
VOLUME [c:/data]
# Wed, 10 Jun 2020 18:03:59 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 10 Jun 2020 18:04:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Jun 2020 18:04:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Jun 2020 18:04:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Jun 2020 18:04:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Jun 2020 18:04:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Jun 2020 18:04:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Jun 2020 18:04:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Jun 2020 18:04:07 GMT
EXPOSE 80
# Wed, 10 Jun 2020 18:04:08 GMT
EXPOSE 443
# Wed, 10 Jun 2020 18:04:08 GMT
EXPOSE 2019
# Wed, 10 Jun 2020 18:04:31 GMT
RUN caddy version
# Wed, 10 Jun 2020 18:04:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f841c6a0c622cd36b5b2688011a224ac3e8e96273758f4a2804f2f3f099f267d`  
		Last Modified: Tue, 09 Jun 2020 23:17:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e676deb3766189ea2b008f69205017c9ee31a77f9c7001fb5a07fb2e2d4fbb0`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba576338ed5242ba3fb838ce5fa930abb61e22fc422ba46b260dbca773cb9`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 4.8 MB (4772911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82aa7b0db5bd44f058750b70c9ca192d7af8986578dd9900fa68f08a53d56d7`  
		Last Modified: Wed, 10 Jun 2020 18:09:46 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6f36d669bbd2a660d47e342775c1705e6b990b004cfb461b66aeb6d978fa60`  
		Last Modified: Wed, 10 Jun 2020 18:09:50 GMT  
		Size: 12.3 MB (12262241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4caa471f3ff12126859610d5fb7a1eee050fdcd24f4c26c840a49072698064`  
		Last Modified: Wed, 10 Jun 2020 18:09:46 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f92da22ed9f6eaba0eb6cb98ff0182e5bf96b672aa9a2a5fc004584af897f91`  
		Last Modified: Wed, 10 Jun 2020 18:09:45 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ca7d66806087b4fb8e9aba7aa8c8d913f6c00b136833ce130ad342601fbcce`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2f91baaa6ad75f37691004649e965eb02f770c8901034ec1d508ac0e198c9f`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490c3bc1055c4210b37fa961535859113aa2a9e83d5373f1edb7664fec3d44a4`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d6ca5a24db2b4dabbd352548aaabc3057e21b5b1d13a3e09ff8d5b4a9f99e4`  
		Last Modified: Wed, 10 Jun 2020 18:09:43 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6b40d207638f35eb44e6d1c604c7939e68829fe4e04a1ca286eea436d3b3b5`  
		Last Modified: Wed, 10 Jun 2020 18:09:42 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d137f3abb4ef203c2caea5f8b50defc1384938cae41fab9c5f751193dd801e`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ff6d828fdc817dccd02e18fb68f60dfb77e5f91b61e4039622748fdacec123`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce68242ed36c05b1696a9aed8843408c0d3df159bdd08a6f89273aea8cf2a52`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8857e417a7cd480ddc26cd312eb34880b8e76040cd4f2ea589b21fbc5d54e274`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a31891b746d7cffa5744afba11ca2c1e207076488f863fe4cb519147cbc359`  
		Last Modified: Wed, 10 Jun 2020 18:09:40 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e936bc871ff19fb19ebb325dc0b2a592fd9347488450d772e434000811f5d8c`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500e96dcc8873265379cfdace5e5c75b28080e5042969250c1656de746a3eb17`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7c3e99413b53ef84bebebfb04ec29d95aa84e3f0e040dc9cbf355afca92009`  
		Last Modified: Wed, 10 Jun 2020 18:09:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790f2340b769609f7c8716568b843cd0723c59c8dc64142f1e927d5536bd9f7c`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 278.2 KB (278231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e765bd24f285691b433b20a6296e67d067e6e2918c7e1cd2ad2bef1bbd356dfc`  
		Last Modified: Wed, 10 Jun 2020 18:09:37 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:c5e137c3575e37688a5ec6f3a628bde1fade7f6c99278fae9f865f24a52accc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:64246e00b3c6726a42b20440c70003c72bc6e652f821982345b87928bc79cae5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5756998229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb6c0b59ae11bc16763ab0732bf43ae0dead1bbded3284e54191f687f4a670e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:04:40 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:06:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Jun 2020 18:06:15 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 10 Jun 2020 18:07:58 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('636bb25c9738400b480ca243a605da74988deb1bc856a1cabe7ee36511db0e048ec0a2688b1640d7b157bc239d437944e43500d91881c8acc7f2b8aa138945f9')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Jun 2020 18:08:00 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Jun 2020 18:08:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Jun 2020 18:08:03 GMT
VOLUME [c:/config]
# Wed, 10 Jun 2020 18:08:04 GMT
VOLUME [c:/data]
# Wed, 10 Jun 2020 18:08:05 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 10 Jun 2020 18:08:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Jun 2020 18:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Jun 2020 18:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Jun 2020 18:08:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Jun 2020 18:08:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Jun 2020 18:08:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Jun 2020 18:08:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Jun 2020 18:08:12 GMT
EXPOSE 80
# Wed, 10 Jun 2020 18:08:13 GMT
EXPOSE 443
# Wed, 10 Jun 2020 18:08:14 GMT
EXPOSE 2019
# Wed, 10 Jun 2020 18:09:10 GMT
RUN caddy version
# Wed, 10 Jun 2020 18:09:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22985925139cd6a6e83b6eb5286a8a6e1053a5c6ddd9762f34deea2aa6bcaacc`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43c028d6768e901bc64b3edb7e2e5f72050d3ed78ea4e7337fe85725d250c15`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 5.4 MB (5404509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab96ccdd2dbffb13487e758409eaae25905b86a83e7b7a51a692c7ff18579b8d`  
		Last Modified: Wed, 10 Jun 2020 18:10:14 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aac2a7ea7e1f98bb6027b5090912006abeb6f367523aac337f6705ba4d7bb6b`  
		Last Modified: Wed, 10 Jun 2020 18:10:19 GMT  
		Size: 17.3 MB (17325836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7acf530d8fe0b1ea1f35f0e20ca267e447936a8edbae3889184d180b44c1a6`  
		Last Modified: Wed, 10 Jun 2020 18:10:13 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7609e5df44616b1f91e5434a43518cf253a69c406c062ef6b99035b20a437`  
		Last Modified: Wed, 10 Jun 2020 18:10:13 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1384cb066181208a5bb3be7023fe3f0b9cedf5483885cf330f7dcd95525302`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f2a49d3e0a25e1871a3dcb23fa333268062b4d027ae041e3bb5c0827dd0c2a`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5ec5b8bc911e1426e8c8dcc06a149b90edee45636d75da5b63e83fe91398a`  
		Last Modified: Wed, 10 Jun 2020 18:10:12 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dab68d41796a58e20ae80dc2528cfe6a2e71a04c8c88bb5595a6e0a5d7f7646`  
		Last Modified: Wed, 10 Jun 2020 18:10:10 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68da8c08840ea413933ac718a42b86738f90a6a5647e151252d4b5193ee40a8d`  
		Last Modified: Wed, 10 Jun 2020 18:10:11 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946bc1b557fc88846697a1a1308c7af5ef52918f700f7dc8bd4c53e915c4a1a3`  
		Last Modified: Wed, 10 Jun 2020 18:10:09 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7ea127cbc59b2799852a077baa3bc9e46ad415abc4de6305396739a257a25e`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e77ea136bb911d1a64b32d1d139522e0e52ca1bc43b5d12aeeef7be91483d50`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a29c745913025b3a12451ab689a6186ec7756b5d99d0fa379a39ae81d510b0b`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4ae08e24e91168918350e7422b8f47200d09a7313216990ba6a672b5372280`  
		Last Modified: Wed, 10 Jun 2020 18:10:08 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e219b4ef296fd92d145bf1f1a7b7d79e09c26a996daf350eb5ee70cbfeed02`  
		Last Modified: Wed, 10 Jun 2020 18:10:05 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc81bd4365ed96954980b554e769048c1e4cc97035385e22ee8364bd2856d4af`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec6f99a5c3e003e6dd16b75770a2762bb5de2737ffdd11b1c707f6aefce201a`  
		Last Modified: Wed, 10 Jun 2020 18:10:05 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26ba6de29355852954f97260ed4e96f1d30d7e675356cc21cac59feb841cf3e`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 248.4 KB (248359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef895a3d9501c41dd42a22a3e2a0458c59b35892005f5fb18b8937101a1fb50`  
		Last Modified: Wed, 10 Jun 2020 18:10:06 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
