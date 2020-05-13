## `caddy:latest`

```console
$ docker pull caddy@sha256:b362245ce6b083b26a903d374bb03823a8c2ed8f4a855c015788418853ebf581
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1217; amd64
	-	windows version 10.0.14393.3686; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:cbbff068d8d40fd77c5ff5ff23d9e8fb137f7c7bff4ed5be3fc0397b938a0407
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15145224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8015a88eb81de87ca681349b919ed7c8e77ce8002d66f1ea3e134833e2761cdf`
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
# Mon, 04 May 2020 19:20:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='3b00c705caa3162750dfea9cacd3f05ae1dda798e346293ba320ee63682a94e5e26c994fee75677324d841962757b098d2f696e4c5a0044131a0cd9b0e54b9fd' ;; 		armhf)   binArch='armv6'; checksum='c8d054eed16910a3fe84d275b3705f61dab204572d5afac4ca02e735fc5741823413e749dcaa9055f930cf8bbaf7a7c28e3cec94527d44111e3de7ed990d685f' ;; 		armv7)   binArch='armv7'; checksum='786fab05ea32e24d3b36b020087b9e05cac507f5b0677b398730ecbd3559030574c7b0c6ff3950978678ee218afa8b912731a31ce187c28d1c19375c5c742a96' ;; 		aarch64) binArch='arm64'; checksum='8864e9bfa0007f2c8fc0823a729b02e8eb53d41857b4b7ce419102e11a225a975420b36e926c754b2247acc286cbb06fcb705f8cc7258ea1c5f3aea0dc3b44f1' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 04 May 2020 19:20:52 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 04 May 2020 19:20:52 GMT
ENV XDG_DATA_HOME=/data
# Mon, 04 May 2020 19:20:52 GMT
VOLUME [/config]
# Mon, 04 May 2020 19:20:52 GMT
VOLUME [/data]
# Mon, 04 May 2020 19:20:52 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Mon, 04 May 2020 19:20:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 04 May 2020 19:20:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 04 May 2020 19:20:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 04 May 2020 19:20:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 04 May 2020 19:20:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 04 May 2020 19:20:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 04 May 2020 19:20:54 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 04 May 2020 19:20:54 GMT
EXPOSE 80
# Mon, 04 May 2020 19:20:54 GMT
EXPOSE 443
# Mon, 04 May 2020 19:20:54 GMT
EXPOSE 2019
# Mon, 04 May 2020 19:20:54 GMT
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
	-	`sha256:4dee063568bdf18794dbcb4dba623ea3a1f7614ed4069f3ad383b562597ff8c2`  
		Last Modified: Mon, 04 May 2020 19:21:28 GMT  
		Size: 12.0 MB (12007589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:a81d694d3aa6fb71250200e1bd70d07066f22e9ac6a1951b3d6df18d03e12b20
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.4 MB (14390606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b19bc691ae372dac3178e3250246952c0abba5a58c5f48ae92782d9c02660ef6`
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
# Wed, 06 May 2020 15:49:34 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 06 May 2020 15:49:34 GMT
ENV XDG_DATA_HOME=/data
# Wed, 06 May 2020 15:49:35 GMT
VOLUME [/config]
# Wed, 06 May 2020 15:49:36 GMT
VOLUME [/data]
# Wed, 06 May 2020 15:49:36 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 06 May 2020 15:49:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 06 May 2020 15:49:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 06 May 2020 15:49:38 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 06 May 2020 15:49:39 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 06 May 2020 15:49:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 06 May 2020 15:49:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 06 May 2020 15:49:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 06 May 2020 15:49:41 GMT
EXPOSE 80
# Wed, 06 May 2020 15:49:42 GMT
EXPOSE 443
# Wed, 06 May 2020 15:49:42 GMT
EXPOSE 2019
# Wed, 06 May 2020 15:49:43 GMT
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

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fc3097b3cd99187dca11658bd33e93e002c8c5cc7de8bc6a29e9ba97d9d405ad
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14164557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a168a021dfdb6e7170f3f10bb242384bb0946809b89047cc76cd4f0127f74bd`
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
# Wed, 06 May 2020 15:57:34 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 06 May 2020 15:57:34 GMT
ENV XDG_DATA_HOME=/data
# Wed, 06 May 2020 15:57:35 GMT
VOLUME [/config]
# Wed, 06 May 2020 15:57:36 GMT
VOLUME [/data]
# Wed, 06 May 2020 15:57:36 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 06 May 2020 15:57:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 06 May 2020 15:57:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 06 May 2020 15:57:38 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 06 May 2020 15:57:39 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 06 May 2020 15:57:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 06 May 2020 15:57:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 06 May 2020 15:57:41 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 06 May 2020 15:57:41 GMT
EXPOSE 80
# Wed, 06 May 2020 15:57:42 GMT
EXPOSE 443
# Wed, 06 May 2020 15:57:43 GMT
EXPOSE 2019
# Wed, 06 May 2020 15:57:43 GMT
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

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:fda3e6c211e921c164d446eb0db4516b3100092ac6906e34142f02d2a1467ed8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14099349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a6718b41c65682371b1c36f12939c112979db7a4cabdd180ceb046dc80a3653`
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
# Wed, 06 May 2020 16:39:41 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 06 May 2020 16:39:42 GMT
ENV XDG_DATA_HOME=/data
# Wed, 06 May 2020 16:39:44 GMT
VOLUME [/config]
# Wed, 06 May 2020 16:39:45 GMT
VOLUME [/data]
# Wed, 06 May 2020 16:39:47 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 06 May 2020 16:39:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 06 May 2020 16:39:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 06 May 2020 16:39:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 06 May 2020 16:39:54 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 06 May 2020 16:39:56 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 06 May 2020 16:39:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 06 May 2020 16:39:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 06 May 2020 16:40:01 GMT
EXPOSE 80
# Wed, 06 May 2020 16:40:02 GMT
EXPOSE 443
# Wed, 06 May 2020 16:40:04 GMT
EXPOSE 2019
# Wed, 06 May 2020 16:40:06 GMT
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

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:d41420be541ff741166121a337ab2380a37986b80e2c198d33cfa2716b89eebc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14000265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:620e8e504bd843011d47928ba3108b784ab917c2b4e49c91f9b5e7a1ed0488e0`
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
# Wed, 06 May 2020 15:30:22 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 06 May 2020 15:30:25 GMT
ENV XDG_DATA_HOME=/data
# Wed, 06 May 2020 15:30:29 GMT
VOLUME [/config]
# Wed, 06 May 2020 15:30:34 GMT
VOLUME [/data]
# Wed, 06 May 2020 15:30:36 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 06 May 2020 15:30:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 06 May 2020 15:30:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 06 May 2020 15:30:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 06 May 2020 15:30:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 06 May 2020 15:30:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 06 May 2020 15:30:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 06 May 2020 15:31:01 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 06 May 2020 15:31:03 GMT
EXPOSE 80
# Wed, 06 May 2020 15:31:09 GMT
EXPOSE 443
# Wed, 06 May 2020 15:31:13 GMT
EXPOSE 2019
# Wed, 06 May 2020 15:31:15 GMT
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

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:befbf95ceefa9c63c3cb86d06d19549d32b0e79546b943634e906584a01fec1d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14740576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc8b4e73e6c6c10833f75c31436b5903780a5cf76d6d767633538129d7d9cef2`
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
# Wed, 06 May 2020 15:30:13 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 06 May 2020 15:30:13 GMT
ENV XDG_DATA_HOME=/data
# Wed, 06 May 2020 15:30:14 GMT
VOLUME [/config]
# Wed, 06 May 2020 15:30:14 GMT
VOLUME [/data]
# Wed, 06 May 2020 15:30:15 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 06 May 2020 15:30:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 06 May 2020 15:30:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 06 May 2020 15:30:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 06 May 2020 15:30:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 06 May 2020 15:30:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 06 May 2020 15:30:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 06 May 2020 15:30:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 06 May 2020 15:30:19 GMT
EXPOSE 80
# Wed, 06 May 2020 15:30:20 GMT
EXPOSE 443
# Wed, 06 May 2020 15:30:20 GMT
EXPOSE 2019
# Wed, 06 May 2020 15:30:21 GMT
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

### `caddy:latest` - windows version 10.0.17763.1217; amd64

```console
$ docker pull caddy@sha256:72fb2769c5bca3a826c2d20272955543ae0505293b8a21f9d7be902c4024462d
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1731274652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00de5663795f5d4dcdda76bf3051f819c10c1b278328fcf09e429e336ca484f5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 12:41:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 May 2020 18:46:58 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 13 May 2020 18:47:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 May 2020 18:47:22 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 13 May 2020 18:47:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('636bb25c9738400b480ca243a605da74988deb1bc856a1cabe7ee36511db0e048ec0a2688b1640d7b157bc239d437944e43500d91881c8acc7f2b8aa138945f9')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 May 2020 18:47:52 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 May 2020 18:47:53 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 May 2020 18:47:54 GMT
VOLUME [c:/config]
# Wed, 13 May 2020 18:47:55 GMT
VOLUME [c:/data]
# Wed, 13 May 2020 18:47:56 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 13 May 2020 18:47:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 May 2020 18:47:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 May 2020 18:47:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 May 2020 18:47:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 May 2020 18:48:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 May 2020 18:48:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 May 2020 18:48:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 May 2020 18:48:03 GMT
EXPOSE 80
# Wed, 13 May 2020 18:48:04 GMT
EXPOSE 443
# Wed, 13 May 2020 18:48:05 GMT
EXPOSE 2019
# Wed, 13 May 2020 18:48:22 GMT
RUN caddy version
# Wed, 13 May 2020 18:48:23 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:77613e754ba9d62c0acd4ef271c4ee7d3af091b8c8b310afa404560a9d281f82`  
		Last Modified: Wed, 13 May 2020 13:00:20 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:543cc8f1346629803094aa24186a3ffc8662b4a2ee69dc801d795f005d4a0d95`  
		Last Modified: Wed, 13 May 2020 18:53:28 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18106f83313e5d34a070612d3f1c39e8cf8d9848e2b227296adfffd3965ba25d`  
		Last Modified: Wed, 13 May 2020 18:53:28 GMT  
		Size: 355.3 KB (355269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f287fd10774920755d67b6de43826c118ec5fc4e8f9702a55be22da2df6358`  
		Last Modified: Wed, 13 May 2020 18:53:26 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ffcf71efbb212a67332d8465f099b447811876b9e83c74eec3c01de1fcb9d0`  
		Last Modified: Wed, 13 May 2020 18:53:10 GMT  
		Size: 12.3 MB (12275873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0eb7cc61a3acb2499d87ea010471ade578b24271a239602554546a519ffbf9`  
		Last Modified: Wed, 13 May 2020 18:53:04 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbafa5496993eb381a49e7fbbadd58834e3ddc0c0e33a83a2b81965beaa664e0`  
		Last Modified: Wed, 13 May 2020 18:53:02 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8269f4f8903d1aef05afd562fda930223dee66a331d0047620fd05dfc076caa`  
		Last Modified: Wed, 13 May 2020 18:53:00 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b0ba135849e8ad69d2e177204089724847fea899770d08be4f326960779471`  
		Last Modified: Wed, 13 May 2020 18:52:58 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775de502a9e90f88c9d9c68063a1aed6775b8a8eaa4f680ea12b84c7a86997aa`  
		Last Modified: Wed, 13 May 2020 18:52:58 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d8993d7ccb4765510c6cd037e5115c7af0ce11df1c85256085067fdc1fc433`  
		Last Modified: Wed, 13 May 2020 18:52:55 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea3755d5c96e8367ee1c769a90f6e6cfc081fdaf18343af918f815188b334e9`  
		Last Modified: Wed, 13 May 2020 18:52:55 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601866b20fd891e3cb277f3f8f172047a2f71d4ff1d97f310c3b94093dc46a50`  
		Last Modified: Wed, 13 May 2020 18:52:55 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01551299aef213dc22bc7224e912b43e5787201c29b0c31153423f15c5db0a94`  
		Last Modified: Wed, 13 May 2020 18:52:53 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0a51580e4218eb251ae8f64eadc2ec6762034308a4057de80eb7472494393b`  
		Last Modified: Wed, 13 May 2020 18:52:53 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be3a4f0438b1d7c8f2a308cb89fea8bbe8fb3b40f143a62069975f86ba1b059`  
		Last Modified: Wed, 13 May 2020 18:52:53 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118019e0b8aa2d8afae2f438d7ff8005a9e4099624fab2c12ea86fec750c64f2`  
		Last Modified: Wed, 13 May 2020 18:52:52 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72ef0c9522d683451d62dee32a69cde84172241d69c164110f784f78162e2a0`  
		Last Modified: Wed, 13 May 2020 18:52:50 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de8b1c41daa7f57c8fe29b16a91ac4e60b636df159ed486ca9f9dc35bab92154`  
		Last Modified: Wed, 13 May 2020 18:52:50 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c96904d7376e44abc396e46bb450c2da8dcfba33355155f6240e07a878423a5`  
		Last Modified: Wed, 13 May 2020 18:52:50 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d27936f5bc0bfbebee69fb6ffdd7bb368b4894c8388b64ee02ad1c7c467677`  
		Last Modified: Wed, 13 May 2020 18:52:50 GMT  
		Size: 288.9 KB (288908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea2f832bbb7958dfa84ad0d27ee64e1f200e10eb27024304f6f7cac63a1be89`  
		Last Modified: Wed, 13 May 2020 18:52:50 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.14393.3686; amd64

```console
$ docker pull caddy@sha256:934fdbcbab89ce90c31479b6686014c304c2e4025f40ab12a0184d7d7031e77c
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5754870634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a3efc2e9d649455a51c1e525b202723307ac0807d3a66606f8b89e8e1722425`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 12:34:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 May 2020 18:48:38 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 13 May 2020 18:49:57 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 May 2020 18:49:58 GMT
ENV CADDY_VERSION=v2.0.0
# Wed, 13 May 2020 18:51:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.0.0/caddy_2.0.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('636bb25c9738400b480ca243a605da74988deb1bc856a1cabe7ee36511db0e048ec0a2688b1640d7b157bc239d437944e43500d91881c8acc7f2b8aa138945f9')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 May 2020 18:51:23 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 May 2020 18:51:24 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 May 2020 18:51:25 GMT
VOLUME [c:/config]
# Wed, 13 May 2020 18:51:26 GMT
VOLUME [c:/data]
# Wed, 13 May 2020 18:51:28 GMT
LABEL org.opencontainers.image.version=v2.0.0
# Wed, 13 May 2020 18:51:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 May 2020 18:51:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 May 2020 18:51:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 May 2020 18:51:31 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 May 2020 18:51:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 May 2020 18:51:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 May 2020 18:51:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 May 2020 18:51:35 GMT
EXPOSE 80
# Wed, 13 May 2020 18:51:36 GMT
EXPOSE 443
# Wed, 13 May 2020 18:51:37 GMT
EXPOSE 2019
# Wed, 13 May 2020 18:52:21 GMT
RUN caddy version
# Wed, 13 May 2020 18:52:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e3e9730c43354781e87aa51e853bff3b1e8c1ca7004f527139638a8f9d499c49`  
		Last Modified: Wed, 13 May 2020 12:59:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8d9441a5da81d2777cfc76980d60cc19b098fe856021de5a9895613a07a917`  
		Last Modified: Wed, 13 May 2020 18:54:24 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60c45322765cd792196713eabac6cc04ae89c4fa85c29b1ca626b72c62996f6`  
		Last Modified: Wed, 13 May 2020 18:54:27 GMT  
		Size: 5.4 MB (5392506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2b93c4954c5f72c6e382ba1480c3d976f845f42c19bb5e0a085798079bb636`  
		Last Modified: Wed, 13 May 2020 18:54:21 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4516cd556129c57a85ef8c01db6dd2122853c304e58bf1d1594fdd77424509`  
		Last Modified: Wed, 13 May 2020 18:54:26 GMT  
		Size: 17.3 MB (17316249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc90b2c917ea7e1658aee4b4fa5144174055d3138552746c780d9540a188c3d7`  
		Last Modified: Wed, 13 May 2020 18:54:21 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c159ba07aef82e0d25aaef42f0ea5a8f3e9ac5979006bb5cfd717fa2b5979c19`  
		Last Modified: Wed, 13 May 2020 18:54:20 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed119e58b16c0727c096be5f489492947e6c14fa38726d290d671d3eb0b7ddc`  
		Last Modified: Wed, 13 May 2020 18:54:19 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36668ca695daf89b18a9a9f22a1ab73b9caff740b5fe364c83b8752053bd520a`  
		Last Modified: Wed, 13 May 2020 18:54:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda31fec458b3a7161e6b3a2ab63d82bb1ab9291b37081e70941e73a13d4cad6`  
		Last Modified: Wed, 13 May 2020 18:54:18 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f31dc3ae4fe27e8327f459ea65e33ab8c62ffdea360d1b9553ed5cae8d21e7b`  
		Last Modified: Wed, 13 May 2020 18:54:18 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440b0ac6915dd1ededf8d058abfbf5bf18ae61704814448b2017af1b56ac222f`  
		Last Modified: Wed, 13 May 2020 18:54:18 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75e3813123a037b3f32302ec2832c105f64f7e4a171a7c551709919d2a2fe50`  
		Last Modified: Wed, 13 May 2020 18:54:17 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef5c9c51be87e873c5fd688f518a5287153de163472db0a1b8ef5219ebc4667`  
		Last Modified: Wed, 13 May 2020 18:54:16 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741b34839eed5be808ac4292dce3424594ea3cff620ab4c5abbb21d7175165bf`  
		Last Modified: Wed, 13 May 2020 18:54:16 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e296d31b4d6061f26450d68b391b5d96928617c8bc8cbf385721f19db40f13`  
		Last Modified: Wed, 13 May 2020 18:54:16 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094a176c2fcfe281888b44bd6b42edc40ecb1f15fa70e3b46a4057a06a461d97`  
		Last Modified: Wed, 13 May 2020 18:54:16 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e80eb7786a112e5e30e573401f1db37e107bf00f6dd3cb2d5e4a5bfcff5864e`  
		Last Modified: Wed, 13 May 2020 18:54:13 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87fc20b2cbd0d3d3009ab3518b6b3df01534f7bf771ac110e8d1d399a1d4c8e`  
		Last Modified: Wed, 13 May 2020 18:54:13 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a2955b5f7006f6354828c6ed4286cecaf180196b00f8c315c9f6cf796a9cde`  
		Last Modified: Wed, 13 May 2020 18:54:14 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bbc73cc73e699dfa7d295778821ae30a39417fe6ae6d52ad4d0ab252cf71976`  
		Last Modified: Wed, 13 May 2020 18:54:14 GMT  
		Size: 250.3 KB (250292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ebb1402ecee93e19be9f62d2148b518e2d255f5592ab44f8090e373ccd7eeb`  
		Last Modified: Wed, 13 May 2020 18:54:13 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
