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
