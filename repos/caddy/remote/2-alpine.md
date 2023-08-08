## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:e9906c7864e06628e2933acdc2e269509289e14b630c9691344d583fa16a0588
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
$ docker pull caddy@sha256:5eb52d854b03fed68136a58636afb03f641d152abd2749e4ad9839fbad50c3c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18628256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4941d41382c6cdd935f71b9f8ffc093229e051ffd537325b8de7197e2caaf9e7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:09:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 07 Aug 2023 20:09:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"
# Mon, 07 Aug 2023 20:09:19 GMT
ENV CADDY_VERSION=v2.7.2
# Mon, 07 Aug 2023 20:09:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b6690cd345f016b4795195f30e626a54644e66f95dc106fb72b44e009aad87433258cd091dc72d8ae357e1b2081d173da528d3f745fe5eb12286c20aa919a21c' ;; 		armhf)   binArch='armv6'; checksum='7911c1a7129550e8f712d6a9c8ec695e2ec8fa025109b360a94275fe50ae9b5039099464e02e30030e5349fa33106600d05623d60aa3bc1d520697c5b07db120' ;; 		armv7)   binArch='armv7'; checksum='fa8596887d1ea7652caea888511377c7c6ea4492889ec0ab1bf76c366f9e52247d41844bffc2f961cc4d06607d65982d8443651ef53f348c7d60f4fb98efbdb9' ;; 		aarch64) binArch='arm64'; checksum='48db86b764e23b892547741e30bf7c95561e804ec999c42fc1dac237ba8b0797abea76556e45c3b231f7acf303e3511507268c62f88076fd31891fc3a03564a7' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='049f0b0529e3e9334388fd099f03fa48a2f5fa2d17b00f46566117397a5468acbc392782abfe815f15f0ef6d8e3f1055bd1d275a927a42590782b83e01259a79' ;; 		s390x)   binArch='s390x'; checksum='3dadb51b4b1e03b884ba00a96fa7371b80aaf97f820bde7e15d2be745b02b91fa00b66422088bc94725ab86600206c458dc3a393e74f9192ef7e76d6fa54cb1f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 07 Aug 2023 20:09:22 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 07 Aug 2023 20:09:22 GMT
ENV XDG_DATA_HOME=/data
# Mon, 07 Aug 2023 20:09:22 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Mon, 07 Aug 2023 20:09:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 07 Aug 2023 20:09:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 07 Aug 2023 20:09:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 07 Aug 2023 20:09:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 07 Aug 2023 20:09:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 07 Aug 2023 20:09:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 07 Aug 2023 20:09:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 07 Aug 2023 20:09:23 GMT
EXPOSE 80
# Mon, 07 Aug 2023 20:09:23 GMT
EXPOSE 443
# Mon, 07 Aug 2023 20:09:23 GMT
EXPOSE 443/udp
# Mon, 07 Aug 2023 20:09:23 GMT
EXPOSE 2019
# Mon, 07 Aug 2023 20:09:23 GMT
WORKDIR /srv
# Mon, 07 Aug 2023 20:09:23 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0aa7b81ef11c65f43b0b58323a33dd9e07eb785529f0d75b452f87a309db00c`  
		Last Modified: Mon, 07 Aug 2023 20:09:40 GMT  
		Size: 350.8 KB (350844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197b67ff1e7160578f7f407e3c4d635e178326f01d1bea6d4d57862ddf4a130c`  
		Last Modified: Mon, 07 Aug 2023 20:09:40 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31705c986d9b6d409dc53b646b7af85353b4bb29890d5b3ea200e75c17ae68dc`  
		Last Modified: Mon, 07 Aug 2023 20:09:42 GMT  
		Size: 14.9 MB (14868294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:20567e1a6bebe3f25633565d0bff6246c016409c6d8e0165473cbcd28ec7afb4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17685310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:302d5c481e2c3ecbccb8cf06c724f4d4cd20d93aee79688e4d02a01f4e93c32a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:19:50 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 03 Aug 2023 21:49:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"
# Thu, 03 Aug 2023 21:49:13 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 03 Aug 2023 21:49:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b6690cd345f016b4795195f30e626a54644e66f95dc106fb72b44e009aad87433258cd091dc72d8ae357e1b2081d173da528d3f745fe5eb12286c20aa919a21c' ;; 		armhf)   binArch='armv6'; checksum='7911c1a7129550e8f712d6a9c8ec695e2ec8fa025109b360a94275fe50ae9b5039099464e02e30030e5349fa33106600d05623d60aa3bc1d520697c5b07db120' ;; 		armv7)   binArch='armv7'; checksum='fa8596887d1ea7652caea888511377c7c6ea4492889ec0ab1bf76c366f9e52247d41844bffc2f961cc4d06607d65982d8443651ef53f348c7d60f4fb98efbdb9' ;; 		aarch64) binArch='arm64'; checksum='48db86b764e23b892547741e30bf7c95561e804ec999c42fc1dac237ba8b0797abea76556e45c3b231f7acf303e3511507268c62f88076fd31891fc3a03564a7' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='049f0b0529e3e9334388fd099f03fa48a2f5fa2d17b00f46566117397a5468acbc392782abfe815f15f0ef6d8e3f1055bd1d275a927a42590782b83e01259a79' ;; 		s390x)   binArch='s390x'; checksum='3dadb51b4b1e03b884ba00a96fa7371b80aaf97f820bde7e15d2be745b02b91fa00b66422088bc94725ab86600206c458dc3a393e74f9192ef7e76d6fa54cb1f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 03 Aug 2023 21:49:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 03 Aug 2023 21:49:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 03 Aug 2023 21:49:16 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Thu, 03 Aug 2023 21:49:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 03 Aug 2023 21:49:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 03 Aug 2023 21:49:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 03 Aug 2023 21:49:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 03 Aug 2023 21:49:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 03 Aug 2023 21:49:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 03 Aug 2023 21:49:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 03 Aug 2023 21:49:17 GMT
EXPOSE 80
# Thu, 03 Aug 2023 21:49:17 GMT
EXPOSE 443
# Thu, 03 Aug 2023 21:49:17 GMT
EXPOSE 443/udp
# Thu, 03 Aug 2023 21:49:17 GMT
EXPOSE 2019
# Thu, 03 Aug 2023 21:49:17 GMT
WORKDIR /srv
# Thu, 03 Aug 2023 21:49:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1307a8613ad92eee47b12de837dc212d252e41489fd7443b6f7df3af69fe79`  
		Last Modified: Wed, 14 Jun 2023 20:20:54 GMT  
		Size: 347.6 KB (347620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f4df12ce70b3a13e8cfe005d513d8d725cf6657fe7379b3b44e8e2aaea6445`  
		Last Modified: Thu, 03 Aug 2023 21:49:36 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96055b6e3dcd90cd5717e94f85371edd36b9bada09264f4ea5da53045dd8e348`  
		Last Modified: Thu, 03 Aug 2023 21:49:39 GMT  
		Size: 14.2 MB (14186830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:2a7eecce65f3fe7d8ff548aa5a3021037fbedc96588e3a4ee317e40d6fd44fbe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17411852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa15ed114d6c8be3a4b6546fae8e0301b907c1ecfe3a92aed2f0feb0528a00b4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:51:41 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Tue, 08 Aug 2023 01:51:42 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"
# Tue, 08 Aug 2023 01:51:42 GMT
ENV CADDY_VERSION=v2.7.2
# Tue, 08 Aug 2023 01:51:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b6690cd345f016b4795195f30e626a54644e66f95dc106fb72b44e009aad87433258cd091dc72d8ae357e1b2081d173da528d3f745fe5eb12286c20aa919a21c' ;; 		armhf)   binArch='armv6'; checksum='7911c1a7129550e8f712d6a9c8ec695e2ec8fa025109b360a94275fe50ae9b5039099464e02e30030e5349fa33106600d05623d60aa3bc1d520697c5b07db120' ;; 		armv7)   binArch='armv7'; checksum='fa8596887d1ea7652caea888511377c7c6ea4492889ec0ab1bf76c366f9e52247d41844bffc2f961cc4d06607d65982d8443651ef53f348c7d60f4fb98efbdb9' ;; 		aarch64) binArch='arm64'; checksum='48db86b764e23b892547741e30bf7c95561e804ec999c42fc1dac237ba8b0797abea76556e45c3b231f7acf303e3511507268c62f88076fd31891fc3a03564a7' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='049f0b0529e3e9334388fd099f03fa48a2f5fa2d17b00f46566117397a5468acbc392782abfe815f15f0ef6d8e3f1055bd1d275a927a42590782b83e01259a79' ;; 		s390x)   binArch='s390x'; checksum='3dadb51b4b1e03b884ba00a96fa7371b80aaf97f820bde7e15d2be745b02b91fa00b66422088bc94725ab86600206c458dc3a393e74f9192ef7e76d6fa54cb1f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 08 Aug 2023 01:51:45 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 08 Aug 2023 01:51:45 GMT
ENV XDG_DATA_HOME=/data
# Tue, 08 Aug 2023 01:51:45 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Tue, 08 Aug 2023 01:51:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 08 Aug 2023 01:51:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 08 Aug 2023 01:51:45 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 08 Aug 2023 01:51:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 08 Aug 2023 01:51:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 08 Aug 2023 01:51:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 08 Aug 2023 01:51:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 08 Aug 2023 01:51:46 GMT
EXPOSE 80
# Tue, 08 Aug 2023 01:51:46 GMT
EXPOSE 443
# Tue, 08 Aug 2023 01:51:46 GMT
EXPOSE 443/udp
# Tue, 08 Aug 2023 01:51:46 GMT
EXPOSE 2019
# Tue, 08 Aug 2023 01:51:46 GMT
WORKDIR /srv
# Tue, 08 Aug 2023 01:51:46 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a47b73e04459258b08555443754e92e2db20bde113c58ca18e1a6f07878f72`  
		Last Modified: Tue, 08 Aug 2023 01:52:05 GMT  
		Size: 344.5 KB (344462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c3a59ade866837d6b09ad55ed50f718b489d789cbe17975d9afd85f0a23a68`  
		Last Modified: Tue, 08 Aug 2023 01:52:05 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39fe4fdc25f277b9fda61bc5e19dde3f4cc812c2fdd6872fcb0bd954d2dd5f6`  
		Last Modified: Tue, 08 Aug 2023 01:52:08 GMT  
		Size: 14.2 MB (14160407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:de0ae94da2b585c185a53e89fa137b5ed2ff4b773d034000268012fbdc8957f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17323505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b87adb171ac21ada0460ec3c0af47565275d01c1485790416fff456ee27e902`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:09:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 07 Aug 2023 21:09:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"
# Mon, 07 Aug 2023 21:09:13 GMT
ENV CADDY_VERSION=v2.7.2
# Mon, 07 Aug 2023 21:09:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b6690cd345f016b4795195f30e626a54644e66f95dc106fb72b44e009aad87433258cd091dc72d8ae357e1b2081d173da528d3f745fe5eb12286c20aa919a21c' ;; 		armhf)   binArch='armv6'; checksum='7911c1a7129550e8f712d6a9c8ec695e2ec8fa025109b360a94275fe50ae9b5039099464e02e30030e5349fa33106600d05623d60aa3bc1d520697c5b07db120' ;; 		armv7)   binArch='armv7'; checksum='fa8596887d1ea7652caea888511377c7c6ea4492889ec0ab1bf76c366f9e52247d41844bffc2f961cc4d06607d65982d8443651ef53f348c7d60f4fb98efbdb9' ;; 		aarch64) binArch='arm64'; checksum='48db86b764e23b892547741e30bf7c95561e804ec999c42fc1dac237ba8b0797abea76556e45c3b231f7acf303e3511507268c62f88076fd31891fc3a03564a7' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='049f0b0529e3e9334388fd099f03fa48a2f5fa2d17b00f46566117397a5468acbc392782abfe815f15f0ef6d8e3f1055bd1d275a927a42590782b83e01259a79' ;; 		s390x)   binArch='s390x'; checksum='3dadb51b4b1e03b884ba00a96fa7371b80aaf97f820bde7e15d2be745b02b91fa00b66422088bc94725ab86600206c458dc3a393e74f9192ef7e76d6fa54cb1f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 07 Aug 2023 21:09:15 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 07 Aug 2023 21:09:15 GMT
ENV XDG_DATA_HOME=/data
# Mon, 07 Aug 2023 21:09:16 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Mon, 07 Aug 2023 21:09:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 07 Aug 2023 21:09:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 07 Aug 2023 21:09:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 07 Aug 2023 21:09:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 07 Aug 2023 21:09:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 07 Aug 2023 21:09:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 07 Aug 2023 21:09:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 07 Aug 2023 21:09:16 GMT
EXPOSE 80
# Mon, 07 Aug 2023 21:09:16 GMT
EXPOSE 443
# Mon, 07 Aug 2023 21:09:16 GMT
EXPOSE 443/udp
# Mon, 07 Aug 2023 21:09:16 GMT
EXPOSE 2019
# Mon, 07 Aug 2023 21:09:16 GMT
WORKDIR /srv
# Mon, 07 Aug 2023 21:09:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a699f78cfb85f60e17fc7c13495876ea0cb4495bbe39e8c65f3e8559b0d7169`  
		Last Modified: Mon, 07 Aug 2023 21:09:34 GMT  
		Size: 360.6 KB (360642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f072a4f755e0ebd59af322e8a999093a60e17529adefbe24031f1f53aabc8e`  
		Last Modified: Mon, 07 Aug 2023 21:09:34 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006bc887db5cfdaa504f4db9399a06a1f39da402b2a3ac396c194e947892b857`  
		Last Modified: Mon, 07 Aug 2023 21:09:35 GMT  
		Size: 13.6 MB (13624590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:c5fddd12f9f41d529a1fa55a8978a49aa7a07879012ccd064f0ee8964077a90a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17021790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d36860c0e9c840efc947f80690df32c02d43c7c5e837961628968f517371707`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:44:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Tue, 08 Aug 2023 00:44:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"
# Tue, 08 Aug 2023 00:44:18 GMT
ENV CADDY_VERSION=v2.7.2
# Tue, 08 Aug 2023 00:44:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b6690cd345f016b4795195f30e626a54644e66f95dc106fb72b44e009aad87433258cd091dc72d8ae357e1b2081d173da528d3f745fe5eb12286c20aa919a21c' ;; 		armhf)   binArch='armv6'; checksum='7911c1a7129550e8f712d6a9c8ec695e2ec8fa025109b360a94275fe50ae9b5039099464e02e30030e5349fa33106600d05623d60aa3bc1d520697c5b07db120' ;; 		armv7)   binArch='armv7'; checksum='fa8596887d1ea7652caea888511377c7c6ea4492889ec0ab1bf76c366f9e52247d41844bffc2f961cc4d06607d65982d8443651ef53f348c7d60f4fb98efbdb9' ;; 		aarch64) binArch='arm64'; checksum='48db86b764e23b892547741e30bf7c95561e804ec999c42fc1dac237ba8b0797abea76556e45c3b231f7acf303e3511507268c62f88076fd31891fc3a03564a7' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='049f0b0529e3e9334388fd099f03fa48a2f5fa2d17b00f46566117397a5468acbc392782abfe815f15f0ef6d8e3f1055bd1d275a927a42590782b83e01259a79' ;; 		s390x)   binArch='s390x'; checksum='3dadb51b4b1e03b884ba00a96fa7371b80aaf97f820bde7e15d2be745b02b91fa00b66422088bc94725ab86600206c458dc3a393e74f9192ef7e76d6fa54cb1f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 08 Aug 2023 00:44:24 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 08 Aug 2023 00:44:24 GMT
ENV XDG_DATA_HOME=/data
# Tue, 08 Aug 2023 00:44:25 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Tue, 08 Aug 2023 00:44:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 08 Aug 2023 00:44:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 08 Aug 2023 00:44:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 08 Aug 2023 00:44:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 08 Aug 2023 00:44:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 08 Aug 2023 00:44:27 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 08 Aug 2023 00:44:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 08 Aug 2023 00:44:29 GMT
EXPOSE 80
# Tue, 08 Aug 2023 00:44:29 GMT
EXPOSE 443
# Tue, 08 Aug 2023 00:44:30 GMT
EXPOSE 443/udp
# Tue, 08 Aug 2023 00:44:30 GMT
EXPOSE 2019
# Tue, 08 Aug 2023 00:44:31 GMT
WORKDIR /srv
# Tue, 08 Aug 2023 00:44:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f40714f45e39ac41e865ccbf2877db62255ce5a5c36a47eadf00b9d174f042`  
		Last Modified: Tue, 08 Aug 2023 00:45:18 GMT  
		Size: 362.2 KB (362173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01316efd8f636e0e7bbe82eeaf33cac4e0d47a88d4ac3c82afbcf11b0f35d9b`  
		Last Modified: Tue, 08 Aug 2023 00:45:18 GMT  
		Size: 7.5 KB (7509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55004bed12d61b288be42361e2901380000c01b9c3cc55ed77a9730bef3d4f4a`  
		Last Modified: Tue, 08 Aug 2023 00:45:21 GMT  
		Size: 13.3 MB (13305857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:2132e0289e15d2b8c5b55cc7df220828a50e3c1446a562784d410190cb7a3b5f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.0 MB (17980833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c729b4121e38ef4c823e5caca342a3d297a87ff7da64495851444714617cf936`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:14:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 07 Aug 2023 20:14:15 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"
# Mon, 07 Aug 2023 20:14:15 GMT
ENV CADDY_VERSION=v2.7.2
# Mon, 07 Aug 2023 20:14:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b6690cd345f016b4795195f30e626a54644e66f95dc106fb72b44e009aad87433258cd091dc72d8ae357e1b2081d173da528d3f745fe5eb12286c20aa919a21c' ;; 		armhf)   binArch='armv6'; checksum='7911c1a7129550e8f712d6a9c8ec695e2ec8fa025109b360a94275fe50ae9b5039099464e02e30030e5349fa33106600d05623d60aa3bc1d520697c5b07db120' ;; 		armv7)   binArch='armv7'; checksum='fa8596887d1ea7652caea888511377c7c6ea4492889ec0ab1bf76c366f9e52247d41844bffc2f961cc4d06607d65982d8443651ef53f348c7d60f4fb98efbdb9' ;; 		aarch64) binArch='arm64'; checksum='48db86b764e23b892547741e30bf7c95561e804ec999c42fc1dac237ba8b0797abea76556e45c3b231f7acf303e3511507268c62f88076fd31891fc3a03564a7' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='049f0b0529e3e9334388fd099f03fa48a2f5fa2d17b00f46566117397a5468acbc392782abfe815f15f0ef6d8e3f1055bd1d275a927a42590782b83e01259a79' ;; 		s390x)   binArch='s390x'; checksum='3dadb51b4b1e03b884ba00a96fa7371b80aaf97f820bde7e15d2be745b02b91fa00b66422088bc94725ab86600206c458dc3a393e74f9192ef7e76d6fa54cb1f' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 07 Aug 2023 20:14:19 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 07 Aug 2023 20:14:19 GMT
ENV XDG_DATA_HOME=/data
# Mon, 07 Aug 2023 20:14:19 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Mon, 07 Aug 2023 20:14:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 07 Aug 2023 20:14:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 07 Aug 2023 20:14:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 07 Aug 2023 20:14:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 07 Aug 2023 20:14:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 07 Aug 2023 20:14:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 07 Aug 2023 20:14:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 07 Aug 2023 20:14:20 GMT
EXPOSE 80
# Mon, 07 Aug 2023 20:14:20 GMT
EXPOSE 443
# Mon, 07 Aug 2023 20:14:20 GMT
EXPOSE 443/udp
# Mon, 07 Aug 2023 20:14:20 GMT
EXPOSE 2019
# Mon, 07 Aug 2023 20:14:20 GMT
WORKDIR /srv
# Mon, 07 Aug 2023 20:14:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df19abd0ca1d4a821a4174a2c0831a57d6fd584073f056abcae085a51f0b3848`  
		Last Modified: Mon, 07 Aug 2023 20:14:50 GMT  
		Size: 354.9 KB (354950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71634633734fd1efdffc0e3a6d26b9c0c104a10255695227fcdc03706ab6b757`  
		Last Modified: Mon, 07 Aug 2023 20:14:50 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1c0932f734bdbb714c63545616dd4fe2151ef72c05499406756c9f09eb7854`  
		Last Modified: Mon, 07 Aug 2023 20:14:52 GMT  
		Size: 14.4 MB (14404182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
