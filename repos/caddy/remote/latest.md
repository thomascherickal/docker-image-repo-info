## `caddy:latest`

```console
$ docker pull caddy@sha256:89213bb94f8a60ebf0554ffe4a45c1af65321140246d34a689e641dae233b063
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4645; amd64
	-	windows version 10.0.20348.1850; amd64

### `caddy:latest` - linux; amd64

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

### `caddy:latest` - linux; arm variant v6

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

### `caddy:latest` - linux; arm variant v7

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

### `caddy:latest` - linux; arm64 variant v8

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

### `caddy:latest` - linux; ppc64le

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

### `caddy:latest` - linux; s390x

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

### `caddy:latest` - windows version 10.0.17763.4645; amd64

```console
$ docker pull caddy@sha256:244e9ea648e66390681506ed4f38cc4443aa354d1610f9b378bcd02d1fd2cf3a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1955706168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50540779ca9094da63ce195b82e5465f7d70989caa8f2eded984c185762b3663`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Fri, 07 Jul 2023 08:17:39 GMT
RUN Install update 10.0.17763.4645
# Thu, 13 Jul 2023 20:32:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 03 Aug 2023 21:16:24 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 03 Aug 2023 21:16:25 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 03 Aug 2023 21:17:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('69d2d73c2514ab5ce4f6a60489c79ce4da0e1d4302c85ab584d0a7a7fd0d034bfe5a5caab78c96ac3383ddd7d2e12c3c41fb47c4716909d2a78d448b0289ccec')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 03 Aug 2023 21:17:35 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 03 Aug 2023 21:17:35 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 03 Aug 2023 21:17:36 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Thu, 03 Aug 2023 21:17:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 03 Aug 2023 21:17:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 03 Aug 2023 21:17:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 03 Aug 2023 21:17:39 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 03 Aug 2023 21:17:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 03 Aug 2023 21:17:41 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 03 Aug 2023 21:17:42 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 03 Aug 2023 21:17:43 GMT
EXPOSE 80
# Thu, 03 Aug 2023 21:17:43 GMT
EXPOSE 443
# Thu, 03 Aug 2023 21:17:44 GMT
EXPOSE 443/udp
# Thu, 03 Aug 2023 21:17:45 GMT
EXPOSE 2019
# Thu, 03 Aug 2023 21:18:44 GMT
RUN caddy version
# Thu, 03 Aug 2023 21:18:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36dba1ee29cd36713c8785a5de7dd2a487244d734ed4c5e7b0a6890bffb806e`  
		Last Modified: Tue, 11 Jul 2023 18:27:38 GMT  
		Size: 289.1 MB (289068746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e991bb72ebb8bf12a5cb5fcb2075d938e3508db6634bdfe6a5bb73e4c612051`  
		Last Modified: Thu, 13 Jul 2023 21:08:51 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726f37fb0b4083f5193485e0d3eb3b3b22f42142f66c17aca0500f5d9bb746e6`  
		Last Modified: Thu, 03 Aug 2023 21:23:02 GMT  
		Size: 477.3 KB (477339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6eb2f82f2289bf967067e8f54468abfa74d0c560c7ff4ee0f24e17b5c61118`  
		Last Modified: Thu, 03 Aug 2023 21:23:02 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9910ce4e2dbdebf58561c3b79500d00fc0b10a1287e2d6c48a59fd53cd1dafb`  
		Last Modified: Thu, 03 Aug 2023 21:23:05 GMT  
		Size: 15.2 MB (15245835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bf5da4d48ea65ff2f357378115fba0f0820f95ad2e6f0ee28b4915d83a311a`  
		Last Modified: Thu, 03 Aug 2023 21:23:01 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed924e132f53161a3eee91723a9ad59a2131996c4a47ebaeffc7c6e10e5ccdf7`  
		Last Modified: Thu, 03 Aug 2023 21:23:00 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71109424ce24da154412db82bfb418de982d76dfd9f12848b5acfcff7e94c477`  
		Last Modified: Thu, 03 Aug 2023 21:23:00 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d33557b82e542b2f3a8ffae2b0f30e1e99e24d8bd68607565d9ffdde35fb578`  
		Last Modified: Thu, 03 Aug 2023 21:23:00 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d3774f6dbd2be4ba8ac48e3cb6190dcbd59b2a0851cd6f04ba52b006e6d07a`  
		Last Modified: Thu, 03 Aug 2023 21:22:59 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ffbcf8830dfcda713001c480020fef263d6ab48d71f78eff5f0f379bda6671`  
		Last Modified: Thu, 03 Aug 2023 21:22:59 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aca4d6a6c867fbdb7342667fffec74374f3713c0bd5953a435945184a732a96`  
		Last Modified: Thu, 03 Aug 2023 21:22:58 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838d5a52d2c79318e51fa0e8b49d03066411ae79bd7b4c7183209f965ad2b7db`  
		Last Modified: Thu, 03 Aug 2023 21:22:58 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a5ea41d6995173c219170336c2f2508f3c513240c5c9beec697bac8750c4ee`  
		Last Modified: Thu, 03 Aug 2023 21:22:58 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c72b63c2f9d7d5012f78b6da71eed80f74bc25d14c1864697c63c375c76cc41`  
		Last Modified: Thu, 03 Aug 2023 21:22:58 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f98023d7c0698dd995c79b4ab8245804816d123d6bd4f296e0fcc775bd7497`  
		Last Modified: Thu, 03 Aug 2023 21:22:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e132135b4ecd518d7b016af2cd783c553c4805e458ca2ce5eff4a79d30ba20a0`  
		Last Modified: Thu, 03 Aug 2023 21:22:56 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd22701b68006012181ebe5b8b726bf4e18afae02e2811719add8702bae39d4`  
		Last Modified: Thu, 03 Aug 2023 21:22:56 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabd852e11407bf1fef45700213ba9857caaef051c7d5e55a0c3632b0186a4b0`  
		Last Modified: Thu, 03 Aug 2023 21:22:56 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647b0fad50d9473598d50c3a2ac34267923778f155f20a4be40087605e8ee28d`  
		Last Modified: Thu, 03 Aug 2023 21:22:56 GMT  
		Size: 270.0 KB (269978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7826c418b559608173421f5ace0ca76d18eb4e81f42dd8ba13a0d38ee05211`  
		Last Modified: Thu, 03 Aug 2023 21:22:56 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.20348.1850; amd64

```console
$ docker pull caddy@sha256:61759f5a3d1ce10d853a4094cf6408335d1433fdc548bbb5df47112f7f42b37c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1753439348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77fcc9fb8974b4428fbaf1925336b5f32b2042050f4668ab2477eeb473ce44ac`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 07 Jul 2023 21:29:32 GMT
RUN Install update 10.0.20348.1850
# Thu, 13 Jul 2023 20:29:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 03 Aug 2023 21:19:26 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 03 Aug 2023 21:19:27 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 03 Aug 2023 21:19:52 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('69d2d73c2514ab5ce4f6a60489c79ce4da0e1d4302c85ab584d0a7a7fd0d034bfe5a5caab78c96ac3383ddd7d2e12c3c41fb47c4716909d2a78d448b0289ccec')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 03 Aug 2023 21:19:53 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 03 Aug 2023 21:19:54 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 03 Aug 2023 21:19:54 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Thu, 03 Aug 2023 21:19:55 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 03 Aug 2023 21:19:56 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 03 Aug 2023 21:19:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 03 Aug 2023 21:19:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 03 Aug 2023 21:19:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 03 Aug 2023 21:19:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 03 Aug 2023 21:20:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 03 Aug 2023 21:20:01 GMT
EXPOSE 80
# Thu, 03 Aug 2023 21:20:01 GMT
EXPOSE 443
# Thu, 03 Aug 2023 21:20:02 GMT
EXPOSE 443/udp
# Thu, 03 Aug 2023 21:20:03 GMT
EXPOSE 2019
# Thu, 03 Aug 2023 21:20:18 GMT
RUN caddy version
# Thu, 03 Aug 2023 21:20:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84a7416e1317a892f4786a89c62493b21df55e0e06b82a4bb007cc79df0f949`  
		Last Modified: Tue, 11 Jul 2023 18:03:32 GMT  
		Size: 348.8 MB (348766456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3e3828ab9c4326158b6161915d8bad87619b3107529ab32863eb31b684d127`  
		Last Modified: Thu, 13 Jul 2023 21:07:36 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e9b6bcbb67de5b41933b793abd6c9589609ac3a81f57c9a9769774bc7d2f0b`  
		Last Modified: Thu, 03 Aug 2023 21:23:28 GMT  
		Size: 492.7 KB (492678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0360f78127e07566726f205a72b71f42ef1e3da4913f6a887e32f2e0ba4d366`  
		Last Modified: Thu, 03 Aug 2023 21:23:28 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af128dc74644b16188a4cb9b4fb19435d69d3d10b097722c5712897fa181dce7`  
		Last Modified: Thu, 03 Aug 2023 21:23:31 GMT  
		Size: 15.3 MB (15252961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89696f04e1e31855a60e95e326f06ed1916b2eb8b24016fb305d5b3cb24d9787`  
		Last Modified: Thu, 03 Aug 2023 21:23:28 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609c23c5b8a90c440aae7423d54ec85e7e461c6877760b74873c27e9031c3f17`  
		Last Modified: Thu, 03 Aug 2023 21:23:26 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e57861cb9b72f7b636fb59a66e8da9be9aad09c3a064555f832560b91a908ef`  
		Last Modified: Thu, 03 Aug 2023 21:23:26 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a8802e26c708c1db71aee23e5ff8f662081a32c6ffb23887861289d3fa76c4`  
		Last Modified: Thu, 03 Aug 2023 21:23:26 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c621782c599e094a65087cbde3d0ccdaac54a9fdbca938411769a0dbfad9fd33`  
		Last Modified: Thu, 03 Aug 2023 21:23:26 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4cc33619413c8259d35279c8f94f76b2f474920a1ece27c4941f511824d90fd`  
		Last Modified: Thu, 03 Aug 2023 21:23:26 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf2fce68a0a9aa50c6d7e2bb20cc8edda4d7138775c234c97773758330be771`  
		Last Modified: Thu, 03 Aug 2023 21:23:24 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d64f2b86ca83abd07dbf404641950ae47023547eb2be1738a4505fca9704a7`  
		Last Modified: Thu, 03 Aug 2023 21:23:24 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28dbbc7aabf9f4e53a0434c7f7929e43b33d6e867cda77eeaa9a6a022bd5ba1c`  
		Last Modified: Thu, 03 Aug 2023 21:23:24 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7469da2db14b8c19ce07788ab3b97af9ddeb68a23da4d42798bffdc185cc7ebf`  
		Last Modified: Thu, 03 Aug 2023 21:23:24 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5e78924954f90ddeb5c34801adcf26789cd0522921ef88796a7c28dbf931c6`  
		Last Modified: Thu, 03 Aug 2023 21:23:24 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f245fed41d1a5742e9eae5db6128bdf5c83e6887f4ec020e452b5343b9a992`  
		Last Modified: Thu, 03 Aug 2023 21:23:22 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92f20efc54b02c58faef830e554c2bdab85b22b0176f17fdd2c39a5e9ae700d`  
		Last Modified: Thu, 03 Aug 2023 21:23:22 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245d53fc9e8da0df2da9a6755505aaefa0d96f527339c282fc9efe0229912dc6`  
		Last Modified: Thu, 03 Aug 2023 21:23:22 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e397d6aa6ede289022b24d854c6b0598776f1e69bacdfc960065b4fe37ea39`  
		Last Modified: Thu, 03 Aug 2023 21:23:22 GMT  
		Size: 306.3 KB (306273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa04fefc0f732dd54239c7498fb47296762fe74c6ea8ada17d09683a9a59fb5f`  
		Last Modified: Thu, 03 Aug 2023 21:23:22 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
