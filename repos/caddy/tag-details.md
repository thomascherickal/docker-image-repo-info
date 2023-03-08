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
-	[`caddy:2.6.4`](#caddy264)
-	[`caddy:2.6.4-alpine`](#caddy264-alpine)
-	[`caddy:2.6.4-builder`](#caddy264-builder)
-	[`caddy:2.6.4-builder-alpine`](#caddy264-builder-alpine)
-	[`caddy:2.6.4-builder-windowsservercore-1809`](#caddy264-builder-windowsservercore-1809)
-	[`caddy:2.6.4-builder-windowsservercore-ltsc2022`](#caddy264-builder-windowsservercore-ltsc2022)
-	[`caddy:2.6.4-windowsservercore`](#caddy264-windowsservercore)
-	[`caddy:2.6.4-windowsservercore-1809`](#caddy264-windowsservercore-1809)
-	[`caddy:2.6.4-windowsservercore-ltsc2022`](#caddy264-windowsservercore-ltsc2022)
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
$ docker pull caddy@sha256:304185ec40295c7b7c33f98981c241d23d959fa0534eb34cd18c732fde51cd5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4010; amd64
	-	windows version 10.0.20348.1547; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:36ba71b44afa613ecf0aadce8e4b9e3f56e0c4b0a78c8edf4e8c2485f21b35ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17449113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8464e23f16f9a82426bbdc3ac8c94270a84453ddc86b9147505a2378a7c2fd0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:38:34 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 11 Feb 2023 07:38:36 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:19:21 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:19:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:19:23 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:19:24 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:19:25 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e3e797818bc929d95bae8220b7b6034b559c217ef5bf622dc7fedc8d270a48`  
		Last Modified: Sat, 11 Feb 2023 07:39:01 GMT  
		Size: 351.2 KB (351178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cebb4c80b3906a9b751ee9a512c1581331b1fd691c84f575c01a29e28403dde`  
		Last Modified: Sat, 11 Feb 2023 07:39:00 GMT  
		Size: 7.6 KB (7552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90648ba22c191b969d8db393bf6138e7d6ecc1b70b3865d1717ec4d663192d89`  
		Last Modified: Wed, 15 Feb 2023 19:19:52 GMT  
		Size: 14.3 MB (14282621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:db317e683b30c11665349301255c3c59f3f5b085d4e075553e445129981ad5e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16582515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4628532cad0308b1d01506925ca941dffeb3bdd058cd79ccd7f055dce243e3b6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:32 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Fri, 10 Feb 2023 20:49:32 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 00:17:32 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 08 Mar 2023 00:17:34 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 08 Mar 2023 00:17:34 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:17:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 08 Mar 2023 00:17:38 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 08 Mar 2023 00:17:39 GMT
ENV XDG_DATA_HOME=/data
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 08 Mar 2023 00:17:41 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 80
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 443
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 443/udp
# Wed, 08 Mar 2023 00:17:42 GMT
EXPOSE 2019
# Wed, 08 Mar 2023 00:17:42 GMT
WORKDIR /srv
# Wed, 08 Mar 2023 00:17:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e676ebf894f684676e3a3c92294bbc14ba7061c7d24285909e673075903c39a9`  
		Last Modified: Wed, 08 Mar 2023 00:18:32 GMT  
		Size: 345.9 KB (345903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b146a16f288a28f362ad572b56958616fb5f4e0572bbe406ce18868be0d5c3`  
		Last Modified: Wed, 08 Mar 2023 00:18:31 GMT  
		Size: 7.6 KB (7559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e662de32a44a67eae886e653355902b11fec7407264122f1e72b5c460cb4334`  
		Last Modified: Wed, 08 Mar 2023 00:18:34 GMT  
		Size: 13.6 MB (13612275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:03b5f2d631567d2783e8977e4988bdc75f13acb5c5b7bb18f3984045fb557b11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16365710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bed848976d2f2ce06398c52bf359363302bd512c4c51f08acb50cdd7ec0db5a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 10:40:15 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 02 Mar 2023 10:40:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 02 Mar 2023 10:40:16 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 02 Mar 2023 10:40:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 02 Mar 2023 10:40:19 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 02 Mar 2023 10:40:19 GMT
ENV XDG_DATA_HOME=/data
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 02 Mar 2023 10:40:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 02 Mar 2023 10:40:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 80
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 443
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 443/udp
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 2019
# Thu, 02 Mar 2023 10:40:20 GMT
WORKDIR /srv
# Thu, 02 Mar 2023 10:40:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769efc94ebb1351d7f88e191e0e5c768fc2462e89d73fa4b373005e8a912f367`  
		Last Modified: Thu, 02 Mar 2023 10:41:04 GMT  
		Size: 342.7 KB (342688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fb7d44b5e1d66fb60d8593e306cfef844841aca960cacb7258951888fcf79e`  
		Last Modified: Thu, 02 Mar 2023 10:41:04 GMT  
		Size: 7.6 KB (7560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818d68e9d461fbb298a8bb8f5467049d89e77e6324f72842c3d45e5af3d0767b`  
		Last Modified: Thu, 02 Mar 2023 10:41:06 GMT  
		Size: 13.6 MB (13594968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6c2623f6bf30798be5c37fc7484e45ecc288d493fb657883f59ddb27ed714ad8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16130997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a38afdc517ef4cff6b6b51a1c6a633c2826599b07feb1e88380d0f783e35cf1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:00:35 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:00:37 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 18:39:20 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 18:39:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 18:39:22 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 18:39:22 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 80
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 443
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 18:39:23 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 18:39:23 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70730e8e2fb933ec157ec87f2a4fb4ad45e8e578b8f7c76cc4846631d773554`  
		Last Modified: Fri, 10 Feb 2023 22:01:02 GMT  
		Size: 350.2 KB (350153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a4b7390d269477c225f1d03e825d2d8bdf6b4d87b5f7bb8811b341e56b7d36`  
		Last Modified: Fri, 10 Feb 2023 22:01:02 GMT  
		Size: 7.6 KB (7555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2743d2ef53ee6edb0e39c89bf16957e3a00990410b2d1a126dca1b2d196182`  
		Last Modified: Wed, 15 Feb 2023 18:39:53 GMT  
		Size: 13.1 MB (13063787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:8861ab3ae3d0c180e38142c2f7482f9ce1773419eb29ed9d6d18308246858093
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5819f0ab4928a30c29293a27299a3b44371cd3bd97df91432ef7b3f43b692d8c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:13:21 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:13:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:16:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:16:41 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:16:42 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:16:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:16:47 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:16:47 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:16:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bd0321e6539bb7dac8574fd36bad22059ef06bb63dc842165f69d0a821572`  
		Last Modified: Fri, 10 Feb 2023 22:14:16 GMT  
		Size: 363.1 KB (363088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb806b2600b0209a73fc7175ab778d0224661034b2f722bd1a0aec1eb9eabe3d`  
		Last Modified: Fri, 10 Feb 2023 22:14:15 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd7c8ae860931dd79dea76d33bc21bb11d89cd4d133cdb41078b040afc6633e`  
		Last Modified: Wed, 15 Feb 2023 19:17:41 GMT  
		Size: 12.8 MB (12779898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:4e1ed99f133abf02d6a7c77849978bb621f748e18c9cb9f7a1dbf88480ddb8d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45cd164da734310b788dcbd4f6c94bccff6e48705fe4d42ecca07a54e9459a9c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:31 GMT
ADD file:17af250b49631cf2acf655c85df90977eddab4c9afd67bda3c577db5200364f1 in / 
# Fri, 10 Feb 2023 21:41:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:14:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:14:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 18:41:48 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 18:41:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 18:41:59 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 18:41:59 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 18:42:00 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 18:42:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 18:42:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 18:42:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 18:42:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 18:42:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 18:42:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 18:42:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 18:42:05 GMT
EXPOSE 80
# Wed, 15 Feb 2023 18:42:06 GMT
EXPOSE 443
# Wed, 15 Feb 2023 18:42:07 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 18:42:07 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 18:42:08 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 18:42:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:667d93a24f321610e24486f3148545191f113ab9ab2444804087dd65ebbda9ed`  
		Last Modified: Fri, 10 Feb 2023 21:42:26 GMT  
		Size: 2.6 MB (2593581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e6ec82400496ce74e37120e1655955b79303daaa5b8ca7e956e3cd96ddd6e9`  
		Last Modified: Fri, 10 Feb 2023 22:15:05 GMT  
		Size: 352.8 KB (352801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5b992687f93ced3715ad97bd95ab37daef5685b784e195209caefbc48f14e9`  
		Last Modified: Fri, 10 Feb 2023 22:15:05 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ccc40924ce2df3343fa5465a92ccaa4ed80e0883190a99d3f468c60f9ddbcf8`  
		Last Modified: Wed, 15 Feb 2023 18:43:19 GMT  
		Size: 13.8 MB (13838817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.4010; amd64

```console
$ docker pull caddy@sha256:f78e6d4fc1641b322d4e44adcada628f9acb5106b2e166cbcba796764a4db257
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1978492183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:198e4772b4788d7810819799af107998abe8e241416654ca5406331afefc2908`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:43:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:44:00 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:45:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:45:08 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:45:09 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:45:10 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:45:11 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:45:12 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:45:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:45:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:45:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:45:17 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:45:19 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:46:11 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:46:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f19b532038d3c84c40068e825815f2b252b82869809b11745d9893f12a99ac1`  
		Last Modified: Thu, 16 Feb 2023 02:51:03 GMT  
		Size: 526.3 KB (526332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15f6c8f1e7f194b2b408bf6c4330db67cf7cd4783d39acba2d8384b2f3c31d4`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab346a52e8e98a31f0970c85a32f1653b5179dd5ad781a8764b08de792a4d99`  
		Last Modified: Thu, 16 Feb 2023 02:51:05 GMT  
		Size: 14.7 MB (14677251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4451f67396ee792e3ace473ca4a69e5e49639ab8b620e489635a7b2eeb775523`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9291ccd53cd67f009cd59c77d90d2623192e5e134fc2ad5a03f1c1860ab66b80`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3096247c037e7418f5efc50ce5c7e6bc272ccac5c014f5cb085d77c4c28a3a`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f902038f4ba892bc3e1e4d5fdcef6b7759891c41c067b744fa3d5b008776c90`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82e400c4f2072b1e2b2ff49169de3108075208b544f454b3cdf016be6356321`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0944799324319439cbaf2f01dd147e8cc496ea80243ddc22e59e301237acb293`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce6c226ffeaa8146cae1b818b43a4776a06f6ce0be460b7d9b42fcc503b39db`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0b36e09fd7994e37dd27ccdcfa4610fc1219c4044a95695c6de9f9eecda63b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f284721a924468c7a0ff80b2809a222ae20cae99d35aa761b5296272783263b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bec609c0b4d99a9726ad86662d32a57664d18dde9d9087c0695ec7e9c4a47c`  
		Last Modified: Thu, 16 Feb 2023 02:50:59 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ad796550cc1ac21dd77352cf12cc78cacbd0a9f8a1e728e7e4f6a02a0cb9fb`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1955699b7dbbfef476622c70f983565943bafe8909c80ec278dff19509fad86`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4096827c6eb36146321a048a5041be746e60afe4c8e90717d681f2d271e0143`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc99e795e3855739a0c170e77263147dec07ac66a9ae51c306705be5af6574b`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8683be90a75d0e97aa8b7002c075e040e7299bd1fde397a541df3e7e4168d97`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 308.1 KB (308099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156392510131bc65057e3573b9aa9838fccd38cc8ed89734e5255bcd4a315274`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.20348.1547; amd64

```console
$ docker pull caddy@sha256:87b9acadc87fc1f78b7ee864f06462a0f45aa263af20fa1744e2f2a0d0870b02
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1695421581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaff43d5343d972f345ff5561ee131879eaafd463e389a1c2607715ac3f6e793`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:46:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:46:57 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:47:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:47:26 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:47:27 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:47:28 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:47:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:47:31 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:47:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:47:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:47:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:47:36 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:47:37 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:47:56 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:47:57 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1961fba6606566986ddd1960cf8309d19fa9deaa486f5a162a60114f3d4c3c82`  
		Last Modified: Thu, 16 Feb 2023 02:51:29 GMT  
		Size: 778.8 KB (778807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af5d76bf41697a16b3336a1857d1e530a3137f28d997c6f5eca0121d42ea88d`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d935f5b810851a2833b69e65d9dcff828f1c6686dab6fa117e9bd08eb95f5990`  
		Last Modified: Thu, 16 Feb 2023 02:51:31 GMT  
		Size: 14.9 MB (14914232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54e2a419181dd9257efde40f9ab80121dd6cc1a478f6ff42d160ddbf5e17cd4`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c07f1bbb0931b3148683baae55ab0d85f8576b2a1d8c2a59bb28544572b5a9d`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06073fd741cf5968f24574903b70213f9743b648ebec9c53ccb8fe114ce01ae`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a17243f1184726e21bf0821ee5984a84575b55befba72594fbf0b3a32a47f1`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c403099e0a283f6f2b25b4235c61c8b564a832643f33280253dc040d2a2ab07`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cc4608f06891b205fbec74e83a221161a2f9d9b50a0b548c3c716d176ee1a4`  
		Last Modified: Thu, 16 Feb 2023 02:51:25 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfe2ac143052b1fa8973567134244ce4ecd1693f16205dd53f0d4cf1b5caa5a`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e217159efeb187bf7ae9a12f6f70764141dd97837f24a517851bc15a36b552`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc05a7da758918922e168d1b07b29f4a81d398dc805724dd6b23b4cb28c7b43`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832768cea319f33011657944b08b51ea41229fdd7a37f21162dd8aedceb31a6b`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443fc82ac63aefa17f6de497731a007fbc972b175040388a8fda7112834af9fa`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39ff50a2c37b226c6e79e3789d1706fc47cb355b14372a147024fc11b2dfb2b`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c6037df6cbd4b9e046dded7157e841a1c40659c4dd082ff9d397c95be6e411`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a470cfe53e2d01e3ca43a7211eb050493a97f430e3c5a52e2364f54a0a4e4834`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d12a1c4350235354af8011d0b2eccb56884eea72a0475197fb007c4fa6c111`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 359.9 KB (359894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea80c894fe52045adaa4c44b9f66422259571c7aec153753d27a56aa3ccbd930`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:3f4414616d9141c4fbd9f66641d9b91a3b67833dd4145738c536dee584db5314
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
$ docker pull caddy@sha256:36ba71b44afa613ecf0aadce8e4b9e3f56e0c4b0a78c8edf4e8c2485f21b35ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17449113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8464e23f16f9a82426bbdc3ac8c94270a84453ddc86b9147505a2378a7c2fd0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:38:34 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 11 Feb 2023 07:38:36 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:19:21 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:19:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:19:23 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:19:24 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:19:25 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e3e797818bc929d95bae8220b7b6034b559c217ef5bf622dc7fedc8d270a48`  
		Last Modified: Sat, 11 Feb 2023 07:39:01 GMT  
		Size: 351.2 KB (351178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cebb4c80b3906a9b751ee9a512c1581331b1fd691c84f575c01a29e28403dde`  
		Last Modified: Sat, 11 Feb 2023 07:39:00 GMT  
		Size: 7.6 KB (7552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90648ba22c191b969d8db393bf6138e7d6ecc1b70b3865d1717ec4d663192d89`  
		Last Modified: Wed, 15 Feb 2023 19:19:52 GMT  
		Size: 14.3 MB (14282621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:db317e683b30c11665349301255c3c59f3f5b085d4e075553e445129981ad5e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16582515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4628532cad0308b1d01506925ca941dffeb3bdd058cd79ccd7f055dce243e3b6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:32 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Fri, 10 Feb 2023 20:49:32 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 00:17:32 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 08 Mar 2023 00:17:34 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 08 Mar 2023 00:17:34 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:17:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 08 Mar 2023 00:17:38 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 08 Mar 2023 00:17:39 GMT
ENV XDG_DATA_HOME=/data
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 08 Mar 2023 00:17:41 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 80
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 443
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 443/udp
# Wed, 08 Mar 2023 00:17:42 GMT
EXPOSE 2019
# Wed, 08 Mar 2023 00:17:42 GMT
WORKDIR /srv
# Wed, 08 Mar 2023 00:17:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e676ebf894f684676e3a3c92294bbc14ba7061c7d24285909e673075903c39a9`  
		Last Modified: Wed, 08 Mar 2023 00:18:32 GMT  
		Size: 345.9 KB (345903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b146a16f288a28f362ad572b56958616fb5f4e0572bbe406ce18868be0d5c3`  
		Last Modified: Wed, 08 Mar 2023 00:18:31 GMT  
		Size: 7.6 KB (7559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e662de32a44a67eae886e653355902b11fec7407264122f1e72b5c460cb4334`  
		Last Modified: Wed, 08 Mar 2023 00:18:34 GMT  
		Size: 13.6 MB (13612275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:03b5f2d631567d2783e8977e4988bdc75f13acb5c5b7bb18f3984045fb557b11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16365710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bed848976d2f2ce06398c52bf359363302bd512c4c51f08acb50cdd7ec0db5a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 10:40:15 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 02 Mar 2023 10:40:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 02 Mar 2023 10:40:16 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 02 Mar 2023 10:40:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 02 Mar 2023 10:40:19 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 02 Mar 2023 10:40:19 GMT
ENV XDG_DATA_HOME=/data
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 02 Mar 2023 10:40:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 02 Mar 2023 10:40:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 80
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 443
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 443/udp
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 2019
# Thu, 02 Mar 2023 10:40:20 GMT
WORKDIR /srv
# Thu, 02 Mar 2023 10:40:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769efc94ebb1351d7f88e191e0e5c768fc2462e89d73fa4b373005e8a912f367`  
		Last Modified: Thu, 02 Mar 2023 10:41:04 GMT  
		Size: 342.7 KB (342688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fb7d44b5e1d66fb60d8593e306cfef844841aca960cacb7258951888fcf79e`  
		Last Modified: Thu, 02 Mar 2023 10:41:04 GMT  
		Size: 7.6 KB (7560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818d68e9d461fbb298a8bb8f5467049d89e77e6324f72842c3d45e5af3d0767b`  
		Last Modified: Thu, 02 Mar 2023 10:41:06 GMT  
		Size: 13.6 MB (13594968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6c2623f6bf30798be5c37fc7484e45ecc288d493fb657883f59ddb27ed714ad8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16130997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a38afdc517ef4cff6b6b51a1c6a633c2826599b07feb1e88380d0f783e35cf1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:00:35 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:00:37 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 18:39:20 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 18:39:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 18:39:22 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 18:39:22 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 80
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 443
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 18:39:23 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 18:39:23 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70730e8e2fb933ec157ec87f2a4fb4ad45e8e578b8f7c76cc4846631d773554`  
		Last Modified: Fri, 10 Feb 2023 22:01:02 GMT  
		Size: 350.2 KB (350153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a4b7390d269477c225f1d03e825d2d8bdf6b4d87b5f7bb8811b341e56b7d36`  
		Last Modified: Fri, 10 Feb 2023 22:01:02 GMT  
		Size: 7.6 KB (7555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2743d2ef53ee6edb0e39c89bf16957e3a00990410b2d1a126dca1b2d196182`  
		Last Modified: Wed, 15 Feb 2023 18:39:53 GMT  
		Size: 13.1 MB (13063787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:8861ab3ae3d0c180e38142c2f7482f9ce1773419eb29ed9d6d18308246858093
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5819f0ab4928a30c29293a27299a3b44371cd3bd97df91432ef7b3f43b692d8c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:13:21 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:13:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:16:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:16:41 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:16:42 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:16:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:16:47 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:16:47 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:16:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bd0321e6539bb7dac8574fd36bad22059ef06bb63dc842165f69d0a821572`  
		Last Modified: Fri, 10 Feb 2023 22:14:16 GMT  
		Size: 363.1 KB (363088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb806b2600b0209a73fc7175ab778d0224661034b2f722bd1a0aec1eb9eabe3d`  
		Last Modified: Fri, 10 Feb 2023 22:14:15 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd7c8ae860931dd79dea76d33bc21bb11d89cd4d133cdb41078b040afc6633e`  
		Last Modified: Wed, 15 Feb 2023 19:17:41 GMT  
		Size: 12.8 MB (12779898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:4e1ed99f133abf02d6a7c77849978bb621f748e18c9cb9f7a1dbf88480ddb8d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45cd164da734310b788dcbd4f6c94bccff6e48705fe4d42ecca07a54e9459a9c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:31 GMT
ADD file:17af250b49631cf2acf655c85df90977eddab4c9afd67bda3c577db5200364f1 in / 
# Fri, 10 Feb 2023 21:41:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:14:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:14:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 18:41:48 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 18:41:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 18:41:59 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 18:41:59 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 18:42:00 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 18:42:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 18:42:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 18:42:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 18:42:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 18:42:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 18:42:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 18:42:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 18:42:05 GMT
EXPOSE 80
# Wed, 15 Feb 2023 18:42:06 GMT
EXPOSE 443
# Wed, 15 Feb 2023 18:42:07 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 18:42:07 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 18:42:08 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 18:42:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:667d93a24f321610e24486f3148545191f113ab9ab2444804087dd65ebbda9ed`  
		Last Modified: Fri, 10 Feb 2023 21:42:26 GMT  
		Size: 2.6 MB (2593581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e6ec82400496ce74e37120e1655955b79303daaa5b8ca7e956e3cd96ddd6e9`  
		Last Modified: Fri, 10 Feb 2023 22:15:05 GMT  
		Size: 352.8 KB (352801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5b992687f93ced3715ad97bd95ab37daef5685b784e195209caefbc48f14e9`  
		Last Modified: Fri, 10 Feb 2023 22:15:05 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ccc40924ce2df3343fa5465a92ccaa4ed80e0883190a99d3f468c60f9ddbcf8`  
		Last Modified: Wed, 15 Feb 2023 18:43:19 GMT  
		Size: 13.8 MB (13838817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:8fe3549f0a6c0db646ec94d25f0c2a87ea055f50cb73477405df8f6fd2349784
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4010; amd64
	-	windows version 10.0.20348.1547; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:47722ffc694507be1e2f34ca172e292fb5e226ea68d87871300b9d65f543fcce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131421587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4674ac67a52f4d29bc8349e9dcca7db8393d778c97c79d9e2f6e997603a99cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 08:21:54 GMT
RUN apk add --no-cache ca-certificates
# Sat, 11 Feb 2023 08:21:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:24:10 GMT
ENV GOLANG_VERSION=1.19.6
# Tue, 14 Feb 2023 19:25:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 14 Feb 2023 19:25:43 GMT
ENV GOPATH=/go
# Tue, 14 Feb 2023 19:25:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:25:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Feb 2023 19:25:44 GMT
WORKDIR /go
# Tue, 14 Feb 2023 19:47:10 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 14 Feb 2023 19:47:10 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 15 Feb 2023 19:19:27 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:19:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 15 Feb 2023 19:19:28 GMT
ENV XCADDY_SETCAP=1
# Wed, 15 Feb 2023 19:19:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 15 Feb 2023 19:19:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 15 Feb 2023 19:19:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d21d5440ebff5aaaaeb115a003f7a4a3897f1866a87de95bc4a21436fc563c`  
		Last Modified: Sat, 11 Feb 2023 08:29:10 GMT  
		Size: 284.8 KB (284816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f790f4c5274f100158d4c23bc5eddf659c1fe93ef4025488f9493d88f1490d88`  
		Last Modified: Tue, 14 Feb 2023 19:31:12 GMT  
		Size: 122.4 MB (122355677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bf170fd9e6726c86c0d4b478d9ec522e82c527a8e708668f48233a4d03f618`  
		Last Modified: Tue, 14 Feb 2023 19:30:55 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a5d1c1b6ed103f8c7f97c73ed546ff7e767b10473b55c15c0d4e1a13a69481`  
		Last Modified: Tue, 14 Feb 2023 19:47:34 GMT  
		Size: 4.2 MB (4188243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0130eaa2f0b1f7646719d82927743bd84c83ed450eb8be4db5327d280d5e4d0`  
		Last Modified: Wed, 15 Feb 2023 19:20:05 GMT  
		Size: 1.2 MB (1217841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab1f57409241476a86d26944527bc2c6c3903eadb21221b8d96da52120b3109`  
		Last Modified: Wed, 15 Feb 2023 19:20:05 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e2b8479c011649b6d47ead7051ebf36d10e2c764f2bc3bc507eab00a1812b6a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127455561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7351cc9a113eeb1deb8afa4c19e381df6b5e03cfef4e63e47bfe99f0b43d95ab`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:28 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Fri, 10 Feb 2023 20:49:28 GMT
CMD ["/bin/sh"]
# Tue, 07 Mar 2023 23:49:29 GMT
RUN apk add --no-cache ca-certificates
# Tue, 07 Mar 2023 23:49:29 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:53:43 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:55:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:55:31 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:55:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:55:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:55:32 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:17:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:17:50 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:17:50 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:17:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:17:51 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:17:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:17:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:17:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06dc45fa3a2f6e0270fe56d6b9f8efada3c9b5854707b52fe42dd55844fb1d5`  
		Last Modified: Tue, 07 Mar 2023 23:58:16 GMT  
		Size: 286.2 KB (286214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9c435c140baf308bcd21b10be4fe27e2cec5ec2acccb0cba35e7ec207d54ae`  
		Last Modified: Tue, 07 Mar 2023 23:59:54 GMT  
		Size: 118.7 MB (118731518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f756f642eb6722bcddfd36a868987c31f5583a7bac2ccf573f8c4fc55198ad49`  
		Last Modified: Tue, 07 Mar 2023 23:59:33 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c49be1b95c6f947e8aaed6708b2c0b38ea78e63b117ac389af00cca5f95334f`  
		Last Modified: Wed, 08 Mar 2023 00:18:51 GMT  
		Size: 4.2 MB (4160310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1cd39813132ad141affe91c6d7f78654e7dbe1e8454baf43e2ee60f2480ecd`  
		Last Modified: Wed, 08 Mar 2023 00:18:51 GMT  
		Size: 1.2 MB (1166071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6624093c59eca00c1b574cd2672bb86cf72a602c484c89dd864ab09d28d875b`  
		Last Modified: Wed, 08 Mar 2023 00:18:50 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:35dc985cc319ba4cd38b0f28d82ec4af14971a9336ce7870444c023c1415fa7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126524974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:822857d40d7e456ebf6b4405bd126f6499dd89ce092e55728fa8deaea4601da8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 02:15:04 GMT
RUN apk add --no-cache ca-certificates
# Thu, 02 Mar 2023 02:15:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 02:19:52 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 02 Mar 2023 02:21:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 02 Mar 2023 02:21:35 GMT
ENV GOPATH=/go
# Thu, 02 Mar 2023 02:21:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 02:21:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 02 Mar 2023 02:21:35 GMT
WORKDIR /go
# Thu, 02 Mar 2023 10:40:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 02 Mar 2023 10:40:26 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_SETCAP=1
# Thu, 02 Mar 2023 10:40:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 02 Mar 2023 10:40:28 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 02 Mar 2023 10:40:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4962ca8504034f69427a90f2b07cfde1e4c20297e4507d5620bb7ea27e646919`  
		Last Modified: Thu, 02 Mar 2023 02:26:02 GMT  
		Size: 285.4 KB (285445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20059bad54d9966d7995685d0c72ce1566c6370b4105df472360f5d2c8ecd21`  
		Last Modified: Thu, 02 Mar 2023 02:28:31 GMT  
		Size: 118.5 MB (118477876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4d49a4d60a68cc1326493b7f8b4cf548d4cec1694b7ccb266f06e4028b501d`  
		Last Modified: Thu, 02 Mar 2023 02:28:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0098f26d1429a39f7d8f6dd18417972d79d6706e530dbfbc4cf9991ff98f3c6`  
		Last Modified: Thu, 02 Mar 2023 10:41:22 GMT  
		Size: 3.7 MB (3729269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0aafe51cc793a860e8c2f2c4799c11f9bebe521643a6f6578f348ce06ae80d`  
		Last Modified: Thu, 02 Mar 2023 10:41:22 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24f3750a2b57fead59e3d812fa66ae7c79703a8a84d41670403b9dc7c23eb90`  
		Last Modified: Thu, 02 Mar 2023 10:41:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6e43472efedad7b414f4cce21a50e04578ea8527ad05ee901ba9eabc88d7718e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125849779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62beb7ef29ce475cb1f571275d3c9ac33185ec48844366ef16a99e8540239b2b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:38:33 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:38:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:43:17 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:44:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:44:26 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:44:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:44:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:44:27 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:06:06 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:06:06 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:06:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:06:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:06:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55522c79112429742fe76c795b9509c5cd1e8198e0caa2a1e355c0e60a719576`  
		Last Modified: Fri, 10 Feb 2023 22:44:19 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1815dcbf43e87e122cc76a24663b7c0d6e01ad03c3be30a7dc13c1bf941c595`  
		Last Modified: Tue, 07 Mar 2023 23:49:19 GMT  
		Size: 116.9 MB (116933985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5aad4e0c6f77e535fe5a51a211a4691a5002a111c52fa17708cf1bc7c01879`  
		Last Modified: Tue, 07 Mar 2023 23:49:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557acb83c53566587727172247e84b25f860b606c200b1fc863eafc75d6b0cf4`  
		Last Modified: Wed, 08 Mar 2023 00:06:29 GMT  
		Size: 4.2 MB (4243285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb71700cd911a18f7eb1f75d651639bc79bda4000e2f4e6a8afe570b03816eb`  
		Last Modified: Wed, 08 Mar 2023 00:06:29 GMT  
		Size: 1.1 MB (1123733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358517d9544ce3184d74860b7f2054339481407b928bb11ccbf7d35163006788`  
		Last Modified: Wed, 08 Mar 2023 00:06:28 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:8126a0d2b7cc9613f70b6b5375c14cc61dfca5dc1b83adc5be33efab8eacc69f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126579575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2da1cd24f35f4106a8a7176a2f2b5656a22982a1787b9204d3eaab9ec535ef58`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:40:13 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:40:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:46:09 GMT
ENV GOLANG_VERSION=1.19.6
# Tue, 14 Feb 2023 19:48:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 14 Feb 2023 19:48:44 GMT
ENV GOPATH=/go
# Tue, 14 Feb 2023 19:48:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:48:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Feb 2023 19:48:46 GMT
WORKDIR /go
# Tue, 14 Feb 2023 20:12:48 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 14 Feb 2023 20:12:48 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 15 Feb 2023 19:16:53 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 15 Feb 2023 19:16:54 GMT
ENV XCADDY_SETCAP=1
# Wed, 15 Feb 2023 19:16:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 15 Feb 2023 19:16:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 15 Feb 2023 19:16:57 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788962e1689dbb14c760601cbf633ae350e98e3a045f8010924cd585de6b6a3e`  
		Last Modified: Fri, 10 Feb 2023 22:53:32 GMT  
		Size: 286.6 KB (286645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ae39b9ad00c218f9156f0958fa48f3062eb5830b791b8592e5f25fd576c7c5`  
		Last Modified: Tue, 14 Feb 2023 19:56:18 GMT  
		Size: 117.3 MB (117316160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f3bf55d586b31bb5c97f2cbf5167fd359b61336f93bed839c2f4de055ced88`  
		Last Modified: Tue, 14 Feb 2023 19:55:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e012d53123423a5fe128ab31d41596d83d8e48699ad608e9eb58dd0b2322fe0`  
		Last Modified: Tue, 14 Feb 2023 20:13:35 GMT  
		Size: 4.5 MB (4479556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90177e6cf58218f094608b8401f41d0da78a0cf57d95718e48e8c6e2f77c6fae`  
		Last Modified: Wed, 15 Feb 2023 19:18:00 GMT  
		Size: 1.1 MB (1105899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e897949e5a46b09b4606d86b20ecb5684cb43f7e1bed1f208ee9b7e93d208c`  
		Last Modified: Wed, 15 Feb 2023 19:17:59 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:8c80a3ba9211715e4a4892ab129d736ec6405a52630b14b828837b7307115c02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129610728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e05d79b3ea15e4e9b6f3f1a89c9e9b9580f66c78fcef17624a8c7bb9f3f51cb5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:27:44 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:27:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:47:03 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:48:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:48:53 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:48:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:48:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:48:53 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:10:01 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:10:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:10:01 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:10:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:10:02 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:10:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:10:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:10:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affa53ed2f1b70a83e3a15cae881ca47cd40f6ac11060717cdbbd4e405f9d586`  
		Last Modified: Fri, 10 Feb 2023 22:37:18 GMT  
		Size: 285.0 KB (285032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d83de48b90cbc8ae74a05d0af343e28f82727b9797b0b45ed9a70fa837a9a5`  
		Last Modified: Tue, 07 Mar 2023 23:53:54 GMT  
		Size: 120.8 MB (120808046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d22668a5d7432e1f8abda37a563ffa67f01cd8658b3247b89a7770eb41fe2a0`  
		Last Modified: Tue, 07 Mar 2023 23:53:38 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3beeef51570794945ced834a4af09db492ac50aadef9f4120ccc6b1dcb4f1251`  
		Last Modified: Wed, 08 Mar 2023 00:10:47 GMT  
		Size: 4.2 MB (4171573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57140a7518a2548d3fd2cef1ecb24c3b4ffb6aee2cc51f3921cb5497bf0863ce`  
		Last Modified: Wed, 08 Mar 2023 00:10:38 GMT  
		Size: 1.2 MB (1170402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe35434ab4b6dfcd2742bd2454af4cb9fe85cc900cacf2e2ef375861498fa09e`  
		Last Modified: Wed, 08 Mar 2023 00:10:38 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.4010; amd64

```console
$ docker pull caddy@sha256:698c8dda106fb34e783e5030fd3ea5166df618f08c2a01204a7a82aabf6b20c9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2148348831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cee813843af987f6985470a05839367529db056040844b778343ebd71743f6a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 23:47:41 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Feb 2023 23:47:42 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Feb 2023 23:47:43 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Feb 2023 23:47:44 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Feb 2023 23:50:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Feb 2023 23:50:19 GMT
ENV GOPATH=C:\go
# Wed, 15 Feb 2023 23:51:42 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Feb 2023 00:11:44 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 16 Feb 2023 00:17:12 GMT
RUN $url = 'https://dl.google.com/go/go1.19.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '8d84af29e46c38b1eec77f9310310517c9e394ac7489e1c7329a94b443b0388d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Feb 2023 00:17:13 GMT
WORKDIR C:\go
# Thu, 16 Feb 2023 02:48:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:48:16 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Feb 2023 02:48:17 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:48:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Feb 2023 02:49:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Feb 2023 02:49:37 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03ac75ee62e05ad7b8b8f97fb78a769177c49d210eedcf0a93035e9a07d0ff2`  
		Last Modified: Thu, 16 Feb 2023 00:28:24 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4beb360c9024340aa5072ce67eab6b3cb005293938525c4f3b77c3bb03f9f501`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5051ce7a895da09ac63e7ca01ef4e30434d833dbd271107d6f96375f291752ad`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea419e1594fbbef3584b4731c356499c7b8a5616af16968e6fd693eccd92012b`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb97c6a047d2cfcb6f0ef6846e78c4d5f60212639a9d1892e2af05033c217df`  
		Last Modified: Thu, 16 Feb 2023 00:28:30 GMT  
		Size: 25.6 MB (25606151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941d25224d4bab25ba0b2304a5811b0fc2970ba6385afdbefbfec898720c3beb`  
		Last Modified: Thu, 16 Feb 2023 00:28:17 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa161895f771062e6d8e8aa2e0e44c15c5affdacc8d409f6e70f1fa743a9bb1`  
		Last Modified: Thu, 16 Feb 2023 00:28:17 GMT  
		Size: 335.6 KB (335550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd14ed3be87ab223f1391d40c3cdcfcee876586e89fbeed2aeccb318734a22`  
		Last Modified: Thu, 16 Feb 2023 00:32:40 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddec1d087c619cf7156e3dba04dd6a73e704d66c60e3fbc4b32c73b4401471b`  
		Last Modified: Thu, 16 Feb 2023 00:33:24 GMT  
		Size: 157.8 MB (157798436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50612066f9b2d86b5cecd95ce6897d89929be6a819c3de13dd9ecc32948832cb`  
		Last Modified: Thu, 16 Feb 2023 00:32:40 GMT  
		Size: 1.5 KB (1544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3bbcb2df900a9ead208e08eefd6faa32bbd6c5a189212d97b94eec1e5807a24`  
		Last Modified: Thu, 16 Feb 2023 02:51:49 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b5e7db448c55e5e60ab1aefceb414700fb99de06cc1c047404e32031064e0c`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7af0982eb604918cfaece327a35d278b59d5f2ca440882b5e7d402e7cce80f6`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad49ef8883b47edaa38ca21b422551a4da50f675370fc1596432938cd7de4d2`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce066417e925c257e21d7126cbbdcf5316022725a7ef7a89575b86fd534d133f`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.6 MB (1632671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbe58e4b6c6b7d8f16c2682325b6df5f61050915e6af7829adab49c1914e5c9`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.20348.1547; amd64

```console
$ docker pull caddy@sha256:21d50bd59eead7016b606e72f6dede55b7f2c718f306c823f3a34ef794622aa7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1865665598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f3a334b2d908beba62aa4ea43b950f4be8fa2261a29819fecc52e58eaadf2df`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 23:42:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Feb 2023 23:42:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Feb 2023 23:42:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Feb 2023 23:42:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Feb 2023 23:43:27 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Feb 2023 23:43:28 GMT
ENV GOPATH=C:\go
# Wed, 15 Feb 2023 23:44:03 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Feb 2023 00:07:02 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 16 Feb 2023 00:11:25 GMT
RUN $url = 'https://dl.google.com/go/go1.19.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '8d84af29e46c38b1eec77f9310310517c9e394ac7489e1c7329a94b443b0388d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Feb 2023 00:11:27 GMT
WORKDIR C:\go
# Thu, 16 Feb 2023 02:49:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:49:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Feb 2023 02:49:47 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:49:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Feb 2023 02:50:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Feb 2023 02:50:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4048a86b3278e59b840ad06b4cf5f5888ce1068d503522a95eb470d5126ed69a`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b07973952171f91c05aade363f3e6c9a2e84548f33eaa3c8e48632460e61f8`  
		Last Modified: Thu, 16 Feb 2023 00:26:45 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a95dff10905572b5f9177959a5a9f60a9364e1dd627ed52e34ec4bee3fb3069`  
		Last Modified: Thu, 16 Feb 2023 00:26:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4267caf437f5a3d92235ab7b8d55b2c812744f166725151ba701aef9d682c6e9`  
		Last Modified: Thu, 16 Feb 2023 00:26:41 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982a959ece2e33bce3f35c5c0adb01a3426c92111b309c15f8cc31200ebcf899`  
		Last Modified: Thu, 16 Feb 2023 00:26:54 GMT  
		Size: 25.9 MB (25852811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065416c07c5d80f7a085e0e84237051d7050a71103cc9d7fb6d5ef57725dc4c6`  
		Last Modified: Thu, 16 Feb 2023 00:26:39 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07015cae66c7ebb6b0adce2dfe424313b228bb703ac3e900deebe74ae961bb49`  
		Last Modified: Thu, 16 Feb 2023 00:26:40 GMT  
		Size: 571.7 KB (571672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285847798b3738c8863954b395d2e44410be1004e9f8513dd1546a0713f153d3`  
		Last Modified: Thu, 16 Feb 2023 00:31:40 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4f6797c9312e8b2093037565c19561d6152cca51a84614b32c0813526f219f`  
		Last Modified: Thu, 16 Feb 2023 00:32:31 GMT  
		Size: 158.0 MB (158008192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2bd8446758388c6c8ddb5d51dd63d25a0dbf5c8e1385928c5e64c83948d966`  
		Last Modified: Thu, 16 Feb 2023 00:31:40 GMT  
		Size: 1.6 KB (1561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd741098e5131c0452f3451d13ce2b131c36cbfcf24df5fbd2fb9e5751e85627`  
		Last Modified: Thu, 16 Feb 2023 02:52:08 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcd5d2a85aea028cd55d32ae579beb21aa5efc8eb3875d901dfcb623092327a`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f63b7e14eef097ca8f36e589d8d609a276d3196875467da71a714db6c8e583`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2e98e1ab65293643e4b2173a01d386c2129bf22ffaee5d1b730f19a26759a7`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15030494f30adf45739bdc5e411e1ae7ea0395ebcb4c2a4f74eedbc5f71d3acd`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.9 MB (1868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba874cf328299688fd26dd5261c439698422f93ce708e583e0e248444622caff`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:68f552074b7668f5c49a7545bad89568f46b134851ee4bb7f558fe6b2e7b7749
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
$ docker pull caddy@sha256:47722ffc694507be1e2f34ca172e292fb5e226ea68d87871300b9d65f543fcce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131421587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4674ac67a52f4d29bc8349e9dcca7db8393d778c97c79d9e2f6e997603a99cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 08:21:54 GMT
RUN apk add --no-cache ca-certificates
# Sat, 11 Feb 2023 08:21:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:24:10 GMT
ENV GOLANG_VERSION=1.19.6
# Tue, 14 Feb 2023 19:25:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 14 Feb 2023 19:25:43 GMT
ENV GOPATH=/go
# Tue, 14 Feb 2023 19:25:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:25:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Feb 2023 19:25:44 GMT
WORKDIR /go
# Tue, 14 Feb 2023 19:47:10 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 14 Feb 2023 19:47:10 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 15 Feb 2023 19:19:27 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:19:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 15 Feb 2023 19:19:28 GMT
ENV XCADDY_SETCAP=1
# Wed, 15 Feb 2023 19:19:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 15 Feb 2023 19:19:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 15 Feb 2023 19:19:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d21d5440ebff5aaaaeb115a003f7a4a3897f1866a87de95bc4a21436fc563c`  
		Last Modified: Sat, 11 Feb 2023 08:29:10 GMT  
		Size: 284.8 KB (284816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f790f4c5274f100158d4c23bc5eddf659c1fe93ef4025488f9493d88f1490d88`  
		Last Modified: Tue, 14 Feb 2023 19:31:12 GMT  
		Size: 122.4 MB (122355677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bf170fd9e6726c86c0d4b478d9ec522e82c527a8e708668f48233a4d03f618`  
		Last Modified: Tue, 14 Feb 2023 19:30:55 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a5d1c1b6ed103f8c7f97c73ed546ff7e767b10473b55c15c0d4e1a13a69481`  
		Last Modified: Tue, 14 Feb 2023 19:47:34 GMT  
		Size: 4.2 MB (4188243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0130eaa2f0b1f7646719d82927743bd84c83ed450eb8be4db5327d280d5e4d0`  
		Last Modified: Wed, 15 Feb 2023 19:20:05 GMT  
		Size: 1.2 MB (1217841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab1f57409241476a86d26944527bc2c6c3903eadb21221b8d96da52120b3109`  
		Last Modified: Wed, 15 Feb 2023 19:20:05 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e2b8479c011649b6d47ead7051ebf36d10e2c764f2bc3bc507eab00a1812b6a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127455561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7351cc9a113eeb1deb8afa4c19e381df6b5e03cfef4e63e47bfe99f0b43d95ab`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:28 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Fri, 10 Feb 2023 20:49:28 GMT
CMD ["/bin/sh"]
# Tue, 07 Mar 2023 23:49:29 GMT
RUN apk add --no-cache ca-certificates
# Tue, 07 Mar 2023 23:49:29 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:53:43 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:55:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:55:31 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:55:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:55:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:55:32 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:17:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:17:50 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:17:50 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:17:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:17:51 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:17:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:17:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:17:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06dc45fa3a2f6e0270fe56d6b9f8efada3c9b5854707b52fe42dd55844fb1d5`  
		Last Modified: Tue, 07 Mar 2023 23:58:16 GMT  
		Size: 286.2 KB (286214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9c435c140baf308bcd21b10be4fe27e2cec5ec2acccb0cba35e7ec207d54ae`  
		Last Modified: Tue, 07 Mar 2023 23:59:54 GMT  
		Size: 118.7 MB (118731518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f756f642eb6722bcddfd36a868987c31f5583a7bac2ccf573f8c4fc55198ad49`  
		Last Modified: Tue, 07 Mar 2023 23:59:33 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c49be1b95c6f947e8aaed6708b2c0b38ea78e63b117ac389af00cca5f95334f`  
		Last Modified: Wed, 08 Mar 2023 00:18:51 GMT  
		Size: 4.2 MB (4160310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1cd39813132ad141affe91c6d7f78654e7dbe1e8454baf43e2ee60f2480ecd`  
		Last Modified: Wed, 08 Mar 2023 00:18:51 GMT  
		Size: 1.2 MB (1166071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6624093c59eca00c1b574cd2672bb86cf72a602c484c89dd864ab09d28d875b`  
		Last Modified: Wed, 08 Mar 2023 00:18:50 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:35dc985cc319ba4cd38b0f28d82ec4af14971a9336ce7870444c023c1415fa7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126524974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:822857d40d7e456ebf6b4405bd126f6499dd89ce092e55728fa8deaea4601da8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 02:15:04 GMT
RUN apk add --no-cache ca-certificates
# Thu, 02 Mar 2023 02:15:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 02:19:52 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 02 Mar 2023 02:21:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 02 Mar 2023 02:21:35 GMT
ENV GOPATH=/go
# Thu, 02 Mar 2023 02:21:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 02:21:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 02 Mar 2023 02:21:35 GMT
WORKDIR /go
# Thu, 02 Mar 2023 10:40:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 02 Mar 2023 10:40:26 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_SETCAP=1
# Thu, 02 Mar 2023 10:40:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 02 Mar 2023 10:40:28 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 02 Mar 2023 10:40:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4962ca8504034f69427a90f2b07cfde1e4c20297e4507d5620bb7ea27e646919`  
		Last Modified: Thu, 02 Mar 2023 02:26:02 GMT  
		Size: 285.4 KB (285445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20059bad54d9966d7995685d0c72ce1566c6370b4105df472360f5d2c8ecd21`  
		Last Modified: Thu, 02 Mar 2023 02:28:31 GMT  
		Size: 118.5 MB (118477876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4d49a4d60a68cc1326493b7f8b4cf548d4cec1694b7ccb266f06e4028b501d`  
		Last Modified: Thu, 02 Mar 2023 02:28:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0098f26d1429a39f7d8f6dd18417972d79d6706e530dbfbc4cf9991ff98f3c6`  
		Last Modified: Thu, 02 Mar 2023 10:41:22 GMT  
		Size: 3.7 MB (3729269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0aafe51cc793a860e8c2f2c4799c11f9bebe521643a6f6578f348ce06ae80d`  
		Last Modified: Thu, 02 Mar 2023 10:41:22 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24f3750a2b57fead59e3d812fa66ae7c79703a8a84d41670403b9dc7c23eb90`  
		Last Modified: Thu, 02 Mar 2023 10:41:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6e43472efedad7b414f4cce21a50e04578ea8527ad05ee901ba9eabc88d7718e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125849779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62beb7ef29ce475cb1f571275d3c9ac33185ec48844366ef16a99e8540239b2b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:38:33 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:38:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:43:17 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:44:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:44:26 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:44:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:44:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:44:27 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:06:06 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:06:06 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:06:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:06:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:06:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55522c79112429742fe76c795b9509c5cd1e8198e0caa2a1e355c0e60a719576`  
		Last Modified: Fri, 10 Feb 2023 22:44:19 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1815dcbf43e87e122cc76a24663b7c0d6e01ad03c3be30a7dc13c1bf941c595`  
		Last Modified: Tue, 07 Mar 2023 23:49:19 GMT  
		Size: 116.9 MB (116933985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5aad4e0c6f77e535fe5a51a211a4691a5002a111c52fa17708cf1bc7c01879`  
		Last Modified: Tue, 07 Mar 2023 23:49:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557acb83c53566587727172247e84b25f860b606c200b1fc863eafc75d6b0cf4`  
		Last Modified: Wed, 08 Mar 2023 00:06:29 GMT  
		Size: 4.2 MB (4243285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb71700cd911a18f7eb1f75d651639bc79bda4000e2f4e6a8afe570b03816eb`  
		Last Modified: Wed, 08 Mar 2023 00:06:29 GMT  
		Size: 1.1 MB (1123733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358517d9544ce3184d74860b7f2054339481407b928bb11ccbf7d35163006788`  
		Last Modified: Wed, 08 Mar 2023 00:06:28 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:8126a0d2b7cc9613f70b6b5375c14cc61dfca5dc1b83adc5be33efab8eacc69f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126579575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2da1cd24f35f4106a8a7176a2f2b5656a22982a1787b9204d3eaab9ec535ef58`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:40:13 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:40:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:46:09 GMT
ENV GOLANG_VERSION=1.19.6
# Tue, 14 Feb 2023 19:48:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 14 Feb 2023 19:48:44 GMT
ENV GOPATH=/go
# Tue, 14 Feb 2023 19:48:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:48:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Feb 2023 19:48:46 GMT
WORKDIR /go
# Tue, 14 Feb 2023 20:12:48 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 14 Feb 2023 20:12:48 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 15 Feb 2023 19:16:53 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 15 Feb 2023 19:16:54 GMT
ENV XCADDY_SETCAP=1
# Wed, 15 Feb 2023 19:16:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 15 Feb 2023 19:16:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 15 Feb 2023 19:16:57 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788962e1689dbb14c760601cbf633ae350e98e3a045f8010924cd585de6b6a3e`  
		Last Modified: Fri, 10 Feb 2023 22:53:32 GMT  
		Size: 286.6 KB (286645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ae39b9ad00c218f9156f0958fa48f3062eb5830b791b8592e5f25fd576c7c5`  
		Last Modified: Tue, 14 Feb 2023 19:56:18 GMT  
		Size: 117.3 MB (117316160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f3bf55d586b31bb5c97f2cbf5167fd359b61336f93bed839c2f4de055ced88`  
		Last Modified: Tue, 14 Feb 2023 19:55:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e012d53123423a5fe128ab31d41596d83d8e48699ad608e9eb58dd0b2322fe0`  
		Last Modified: Tue, 14 Feb 2023 20:13:35 GMT  
		Size: 4.5 MB (4479556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90177e6cf58218f094608b8401f41d0da78a0cf57d95718e48e8c6e2f77c6fae`  
		Last Modified: Wed, 15 Feb 2023 19:18:00 GMT  
		Size: 1.1 MB (1105899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e897949e5a46b09b4606d86b20ecb5684cb43f7e1bed1f208ee9b7e93d208c`  
		Last Modified: Wed, 15 Feb 2023 19:17:59 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:8c80a3ba9211715e4a4892ab129d736ec6405a52630b14b828837b7307115c02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129610728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e05d79b3ea15e4e9b6f3f1a89c9e9b9580f66c78fcef17624a8c7bb9f3f51cb5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:27:44 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:27:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:47:03 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:48:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:48:53 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:48:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:48:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:48:53 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:10:01 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:10:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:10:01 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:10:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:10:02 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:10:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:10:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:10:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affa53ed2f1b70a83e3a15cae881ca47cd40f6ac11060717cdbbd4e405f9d586`  
		Last Modified: Fri, 10 Feb 2023 22:37:18 GMT  
		Size: 285.0 KB (285032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d83de48b90cbc8ae74a05d0af343e28f82727b9797b0b45ed9a70fa837a9a5`  
		Last Modified: Tue, 07 Mar 2023 23:53:54 GMT  
		Size: 120.8 MB (120808046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d22668a5d7432e1f8abda37a563ffa67f01cd8658b3247b89a7770eb41fe2a0`  
		Last Modified: Tue, 07 Mar 2023 23:53:38 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3beeef51570794945ced834a4af09db492ac50aadef9f4120ccc6b1dcb4f1251`  
		Last Modified: Wed, 08 Mar 2023 00:10:47 GMT  
		Size: 4.2 MB (4171573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57140a7518a2548d3fd2cef1ecb24c3b4ffb6aee2cc51f3921cb5497bf0863ce`  
		Last Modified: Wed, 08 Mar 2023 00:10:38 GMT  
		Size: 1.2 MB (1170402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe35434ab4b6dfcd2742bd2454af4cb9fe85cc900cacf2e2ef375861498fa09e`  
		Last Modified: Wed, 08 Mar 2023 00:10:38 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:687ff9a9e85091470e7d84be08a4e96d119290226bfcd464502138db4b9f1542
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4010; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.4010; amd64

```console
$ docker pull caddy@sha256:698c8dda106fb34e783e5030fd3ea5166df618f08c2a01204a7a82aabf6b20c9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2148348831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cee813843af987f6985470a05839367529db056040844b778343ebd71743f6a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 23:47:41 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Feb 2023 23:47:42 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Feb 2023 23:47:43 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Feb 2023 23:47:44 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Feb 2023 23:50:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Feb 2023 23:50:19 GMT
ENV GOPATH=C:\go
# Wed, 15 Feb 2023 23:51:42 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Feb 2023 00:11:44 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 16 Feb 2023 00:17:12 GMT
RUN $url = 'https://dl.google.com/go/go1.19.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '8d84af29e46c38b1eec77f9310310517c9e394ac7489e1c7329a94b443b0388d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Feb 2023 00:17:13 GMT
WORKDIR C:\go
# Thu, 16 Feb 2023 02:48:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:48:16 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Feb 2023 02:48:17 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:48:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Feb 2023 02:49:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Feb 2023 02:49:37 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03ac75ee62e05ad7b8b8f97fb78a769177c49d210eedcf0a93035e9a07d0ff2`  
		Last Modified: Thu, 16 Feb 2023 00:28:24 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4beb360c9024340aa5072ce67eab6b3cb005293938525c4f3b77c3bb03f9f501`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5051ce7a895da09ac63e7ca01ef4e30434d833dbd271107d6f96375f291752ad`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea419e1594fbbef3584b4731c356499c7b8a5616af16968e6fd693eccd92012b`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb97c6a047d2cfcb6f0ef6846e78c4d5f60212639a9d1892e2af05033c217df`  
		Last Modified: Thu, 16 Feb 2023 00:28:30 GMT  
		Size: 25.6 MB (25606151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941d25224d4bab25ba0b2304a5811b0fc2970ba6385afdbefbfec898720c3beb`  
		Last Modified: Thu, 16 Feb 2023 00:28:17 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa161895f771062e6d8e8aa2e0e44c15c5affdacc8d409f6e70f1fa743a9bb1`  
		Last Modified: Thu, 16 Feb 2023 00:28:17 GMT  
		Size: 335.6 KB (335550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd14ed3be87ab223f1391d40c3cdcfcee876586e89fbeed2aeccb318734a22`  
		Last Modified: Thu, 16 Feb 2023 00:32:40 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddec1d087c619cf7156e3dba04dd6a73e704d66c60e3fbc4b32c73b4401471b`  
		Last Modified: Thu, 16 Feb 2023 00:33:24 GMT  
		Size: 157.8 MB (157798436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50612066f9b2d86b5cecd95ce6897d89929be6a819c3de13dd9ecc32948832cb`  
		Last Modified: Thu, 16 Feb 2023 00:32:40 GMT  
		Size: 1.5 KB (1544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3bbcb2df900a9ead208e08eefd6faa32bbd6c5a189212d97b94eec1e5807a24`  
		Last Modified: Thu, 16 Feb 2023 02:51:49 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b5e7db448c55e5e60ab1aefceb414700fb99de06cc1c047404e32031064e0c`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7af0982eb604918cfaece327a35d278b59d5f2ca440882b5e7d402e7cce80f6`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad49ef8883b47edaa38ca21b422551a4da50f675370fc1596432938cd7de4d2`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce066417e925c257e21d7126cbbdcf5316022725a7ef7a89575b86fd534d133f`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.6 MB (1632671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbe58e4b6c6b7d8f16c2682325b6df5f61050915e6af7829adab49c1914e5c9`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:573ab227ac93b402974ef9c7f039983bc070f5e08c73d21e62345c13f8ccbaab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `caddy:2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1547; amd64

```console
$ docker pull caddy@sha256:21d50bd59eead7016b606e72f6dede55b7f2c718f306c823f3a34ef794622aa7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1865665598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f3a334b2d908beba62aa4ea43b950f4be8fa2261a29819fecc52e58eaadf2df`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 23:42:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Feb 2023 23:42:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Feb 2023 23:42:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Feb 2023 23:42:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Feb 2023 23:43:27 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Feb 2023 23:43:28 GMT
ENV GOPATH=C:\go
# Wed, 15 Feb 2023 23:44:03 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Feb 2023 00:07:02 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 16 Feb 2023 00:11:25 GMT
RUN $url = 'https://dl.google.com/go/go1.19.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '8d84af29e46c38b1eec77f9310310517c9e394ac7489e1c7329a94b443b0388d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Feb 2023 00:11:27 GMT
WORKDIR C:\go
# Thu, 16 Feb 2023 02:49:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:49:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Feb 2023 02:49:47 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:49:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Feb 2023 02:50:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Feb 2023 02:50:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4048a86b3278e59b840ad06b4cf5f5888ce1068d503522a95eb470d5126ed69a`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b07973952171f91c05aade363f3e6c9a2e84548f33eaa3c8e48632460e61f8`  
		Last Modified: Thu, 16 Feb 2023 00:26:45 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a95dff10905572b5f9177959a5a9f60a9364e1dd627ed52e34ec4bee3fb3069`  
		Last Modified: Thu, 16 Feb 2023 00:26:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4267caf437f5a3d92235ab7b8d55b2c812744f166725151ba701aef9d682c6e9`  
		Last Modified: Thu, 16 Feb 2023 00:26:41 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982a959ece2e33bce3f35c5c0adb01a3426c92111b309c15f8cc31200ebcf899`  
		Last Modified: Thu, 16 Feb 2023 00:26:54 GMT  
		Size: 25.9 MB (25852811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065416c07c5d80f7a085e0e84237051d7050a71103cc9d7fb6d5ef57725dc4c6`  
		Last Modified: Thu, 16 Feb 2023 00:26:39 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07015cae66c7ebb6b0adce2dfe424313b228bb703ac3e900deebe74ae961bb49`  
		Last Modified: Thu, 16 Feb 2023 00:26:40 GMT  
		Size: 571.7 KB (571672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285847798b3738c8863954b395d2e44410be1004e9f8513dd1546a0713f153d3`  
		Last Modified: Thu, 16 Feb 2023 00:31:40 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4f6797c9312e8b2093037565c19561d6152cca51a84614b32c0813526f219f`  
		Last Modified: Thu, 16 Feb 2023 00:32:31 GMT  
		Size: 158.0 MB (158008192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2bd8446758388c6c8ddb5d51dd63d25a0dbf5c8e1385928c5e64c83948d966`  
		Last Modified: Thu, 16 Feb 2023 00:31:40 GMT  
		Size: 1.6 KB (1561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd741098e5131c0452f3451d13ce2b131c36cbfcf24df5fbd2fb9e5751e85627`  
		Last Modified: Thu, 16 Feb 2023 02:52:08 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcd5d2a85aea028cd55d32ae579beb21aa5efc8eb3875d901dfcb623092327a`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f63b7e14eef097ca8f36e589d8d609a276d3196875467da71a714db6c8e583`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2e98e1ab65293643e4b2173a01d386c2129bf22ffaee5d1b730f19a26759a7`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15030494f30adf45739bdc5e411e1ae7ea0395ebcb4c2a4f74eedbc5f71d3acd`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.9 MB (1868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba874cf328299688fd26dd5261c439698422f93ce708e583e0e248444622caff`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:07fbc5a89186611e042f7ab23685ae8afbcce5678ff9b1315e742e6935052c9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4010; amd64
	-	windows version 10.0.20348.1547; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.4010; amd64

```console
$ docker pull caddy@sha256:f78e6d4fc1641b322d4e44adcada628f9acb5106b2e166cbcba796764a4db257
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1978492183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:198e4772b4788d7810819799af107998abe8e241416654ca5406331afefc2908`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:43:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:44:00 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:45:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:45:08 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:45:09 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:45:10 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:45:11 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:45:12 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:45:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:45:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:45:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:45:17 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:45:19 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:46:11 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:46:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f19b532038d3c84c40068e825815f2b252b82869809b11745d9893f12a99ac1`  
		Last Modified: Thu, 16 Feb 2023 02:51:03 GMT  
		Size: 526.3 KB (526332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15f6c8f1e7f194b2b408bf6c4330db67cf7cd4783d39acba2d8384b2f3c31d4`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab346a52e8e98a31f0970c85a32f1653b5179dd5ad781a8764b08de792a4d99`  
		Last Modified: Thu, 16 Feb 2023 02:51:05 GMT  
		Size: 14.7 MB (14677251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4451f67396ee792e3ace473ca4a69e5e49639ab8b620e489635a7b2eeb775523`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9291ccd53cd67f009cd59c77d90d2623192e5e134fc2ad5a03f1c1860ab66b80`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3096247c037e7418f5efc50ce5c7e6bc272ccac5c014f5cb085d77c4c28a3a`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f902038f4ba892bc3e1e4d5fdcef6b7759891c41c067b744fa3d5b008776c90`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82e400c4f2072b1e2b2ff49169de3108075208b544f454b3cdf016be6356321`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0944799324319439cbaf2f01dd147e8cc496ea80243ddc22e59e301237acb293`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce6c226ffeaa8146cae1b818b43a4776a06f6ce0be460b7d9b42fcc503b39db`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0b36e09fd7994e37dd27ccdcfa4610fc1219c4044a95695c6de9f9eecda63b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f284721a924468c7a0ff80b2809a222ae20cae99d35aa761b5296272783263b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bec609c0b4d99a9726ad86662d32a57664d18dde9d9087c0695ec7e9c4a47c`  
		Last Modified: Thu, 16 Feb 2023 02:50:59 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ad796550cc1ac21dd77352cf12cc78cacbd0a9f8a1e728e7e4f6a02a0cb9fb`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1955699b7dbbfef476622c70f983565943bafe8909c80ec278dff19509fad86`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4096827c6eb36146321a048a5041be746e60afe4c8e90717d681f2d271e0143`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc99e795e3855739a0c170e77263147dec07ac66a9ae51c306705be5af6574b`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8683be90a75d0e97aa8b7002c075e040e7299bd1fde397a541df3e7e4168d97`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 308.1 KB (308099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156392510131bc65057e3573b9aa9838fccd38cc8ed89734e5255bcd4a315274`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.20348.1547; amd64

```console
$ docker pull caddy@sha256:87b9acadc87fc1f78b7ee864f06462a0f45aa263af20fa1744e2f2a0d0870b02
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1695421581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaff43d5343d972f345ff5561ee131879eaafd463e389a1c2607715ac3f6e793`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:46:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:46:57 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:47:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:47:26 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:47:27 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:47:28 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:47:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:47:31 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:47:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:47:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:47:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:47:36 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:47:37 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:47:56 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:47:57 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1961fba6606566986ddd1960cf8309d19fa9deaa486f5a162a60114f3d4c3c82`  
		Last Modified: Thu, 16 Feb 2023 02:51:29 GMT  
		Size: 778.8 KB (778807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af5d76bf41697a16b3336a1857d1e530a3137f28d997c6f5eca0121d42ea88d`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d935f5b810851a2833b69e65d9dcff828f1c6686dab6fa117e9bd08eb95f5990`  
		Last Modified: Thu, 16 Feb 2023 02:51:31 GMT  
		Size: 14.9 MB (14914232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54e2a419181dd9257efde40f9ab80121dd6cc1a478f6ff42d160ddbf5e17cd4`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c07f1bbb0931b3148683baae55ab0d85f8576b2a1d8c2a59bb28544572b5a9d`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06073fd741cf5968f24574903b70213f9743b648ebec9c53ccb8fe114ce01ae`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a17243f1184726e21bf0821ee5984a84575b55befba72594fbf0b3a32a47f1`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c403099e0a283f6f2b25b4235c61c8b564a832643f33280253dc040d2a2ab07`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cc4608f06891b205fbec74e83a221161a2f9d9b50a0b548c3c716d176ee1a4`  
		Last Modified: Thu, 16 Feb 2023 02:51:25 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfe2ac143052b1fa8973567134244ce4ecd1693f16205dd53f0d4cf1b5caa5a`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e217159efeb187bf7ae9a12f6f70764141dd97837f24a517851bc15a36b552`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc05a7da758918922e168d1b07b29f4a81d398dc805724dd6b23b4cb28c7b43`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832768cea319f33011657944b08b51ea41229fdd7a37f21162dd8aedceb31a6b`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443fc82ac63aefa17f6de497731a007fbc972b175040388a8fda7112834af9fa`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39ff50a2c37b226c6e79e3789d1706fc47cb355b14372a147024fc11b2dfb2b`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c6037df6cbd4b9e046dded7157e841a1c40659c4dd082ff9d397c95be6e411`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a470cfe53e2d01e3ca43a7211eb050493a97f430e3c5a52e2364f54a0a4e4834`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d12a1c4350235354af8011d0b2eccb56884eea72a0475197fb007c4fa6c111`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 359.9 KB (359894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea80c894fe52045adaa4c44b9f66422259571c7aec153753d27a56aa3ccbd930`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:1bd6dc9cf41fc94696e73caafb13f1e2aa4080c4961ffe195303c2a51811ff9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4010; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.4010; amd64

```console
$ docker pull caddy@sha256:f78e6d4fc1641b322d4e44adcada628f9acb5106b2e166cbcba796764a4db257
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1978492183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:198e4772b4788d7810819799af107998abe8e241416654ca5406331afefc2908`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:43:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:44:00 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:45:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:45:08 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:45:09 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:45:10 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:45:11 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:45:12 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:45:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:45:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:45:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:45:17 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:45:19 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:46:11 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:46:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f19b532038d3c84c40068e825815f2b252b82869809b11745d9893f12a99ac1`  
		Last Modified: Thu, 16 Feb 2023 02:51:03 GMT  
		Size: 526.3 KB (526332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15f6c8f1e7f194b2b408bf6c4330db67cf7cd4783d39acba2d8384b2f3c31d4`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab346a52e8e98a31f0970c85a32f1653b5179dd5ad781a8764b08de792a4d99`  
		Last Modified: Thu, 16 Feb 2023 02:51:05 GMT  
		Size: 14.7 MB (14677251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4451f67396ee792e3ace473ca4a69e5e49639ab8b620e489635a7b2eeb775523`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9291ccd53cd67f009cd59c77d90d2623192e5e134fc2ad5a03f1c1860ab66b80`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3096247c037e7418f5efc50ce5c7e6bc272ccac5c014f5cb085d77c4c28a3a`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f902038f4ba892bc3e1e4d5fdcef6b7759891c41c067b744fa3d5b008776c90`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82e400c4f2072b1e2b2ff49169de3108075208b544f454b3cdf016be6356321`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0944799324319439cbaf2f01dd147e8cc496ea80243ddc22e59e301237acb293`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce6c226ffeaa8146cae1b818b43a4776a06f6ce0be460b7d9b42fcc503b39db`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0b36e09fd7994e37dd27ccdcfa4610fc1219c4044a95695c6de9f9eecda63b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f284721a924468c7a0ff80b2809a222ae20cae99d35aa761b5296272783263b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bec609c0b4d99a9726ad86662d32a57664d18dde9d9087c0695ec7e9c4a47c`  
		Last Modified: Thu, 16 Feb 2023 02:50:59 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ad796550cc1ac21dd77352cf12cc78cacbd0a9f8a1e728e7e4f6a02a0cb9fb`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1955699b7dbbfef476622c70f983565943bafe8909c80ec278dff19509fad86`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4096827c6eb36146321a048a5041be746e60afe4c8e90717d681f2d271e0143`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc99e795e3855739a0c170e77263147dec07ac66a9ae51c306705be5af6574b`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8683be90a75d0e97aa8b7002c075e040e7299bd1fde397a541df3e7e4168d97`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 308.1 KB (308099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156392510131bc65057e3573b9aa9838fccd38cc8ed89734e5255bcd4a315274`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:bdada4aecbae3dbf7c909817361c5c5e025530a60f1017107cf4cbe628e5a12b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `caddy:2-windowsservercore-ltsc2022` - windows version 10.0.20348.1547; amd64

```console
$ docker pull caddy@sha256:87b9acadc87fc1f78b7ee864f06462a0f45aa263af20fa1744e2f2a0d0870b02
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1695421581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaff43d5343d972f345ff5561ee131879eaafd463e389a1c2607715ac3f6e793`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:46:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:46:57 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:47:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:47:26 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:47:27 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:47:28 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:47:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:47:31 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:47:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:47:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:47:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:47:36 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:47:37 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:47:56 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:47:57 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1961fba6606566986ddd1960cf8309d19fa9deaa486f5a162a60114f3d4c3c82`  
		Last Modified: Thu, 16 Feb 2023 02:51:29 GMT  
		Size: 778.8 KB (778807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af5d76bf41697a16b3336a1857d1e530a3137f28d997c6f5eca0121d42ea88d`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d935f5b810851a2833b69e65d9dcff828f1c6686dab6fa117e9bd08eb95f5990`  
		Last Modified: Thu, 16 Feb 2023 02:51:31 GMT  
		Size: 14.9 MB (14914232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54e2a419181dd9257efde40f9ab80121dd6cc1a478f6ff42d160ddbf5e17cd4`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c07f1bbb0931b3148683baae55ab0d85f8576b2a1d8c2a59bb28544572b5a9d`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06073fd741cf5968f24574903b70213f9743b648ebec9c53ccb8fe114ce01ae`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a17243f1184726e21bf0821ee5984a84575b55befba72594fbf0b3a32a47f1`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c403099e0a283f6f2b25b4235c61c8b564a832643f33280253dc040d2a2ab07`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cc4608f06891b205fbec74e83a221161a2f9d9b50a0b548c3c716d176ee1a4`  
		Last Modified: Thu, 16 Feb 2023 02:51:25 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfe2ac143052b1fa8973567134244ce4ecd1693f16205dd53f0d4cf1b5caa5a`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e217159efeb187bf7ae9a12f6f70764141dd97837f24a517851bc15a36b552`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc05a7da758918922e168d1b07b29f4a81d398dc805724dd6b23b4cb28c7b43`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832768cea319f33011657944b08b51ea41229fdd7a37f21162dd8aedceb31a6b`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443fc82ac63aefa17f6de497731a007fbc972b175040388a8fda7112834af9fa`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39ff50a2c37b226c6e79e3789d1706fc47cb355b14372a147024fc11b2dfb2b`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c6037df6cbd4b9e046dded7157e841a1c40659c4dd082ff9d397c95be6e411`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a470cfe53e2d01e3ca43a7211eb050493a97f430e3c5a52e2364f54a0a4e4834`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d12a1c4350235354af8011d0b2eccb56884eea72a0475197fb007c4fa6c111`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 359.9 KB (359894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea80c894fe52045adaa4c44b9f66422259571c7aec153753d27a56aa3ccbd930`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6`

```console
$ docker pull caddy@sha256:304185ec40295c7b7c33f98981c241d23d959fa0534eb34cd18c732fde51cd5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4010; amd64
	-	windows version 10.0.20348.1547; amd64

### `caddy:2.6` - linux; amd64

```console
$ docker pull caddy@sha256:36ba71b44afa613ecf0aadce8e4b9e3f56e0c4b0a78c8edf4e8c2485f21b35ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17449113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8464e23f16f9a82426bbdc3ac8c94270a84453ddc86b9147505a2378a7c2fd0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:38:34 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 11 Feb 2023 07:38:36 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:19:21 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:19:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:19:23 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:19:24 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:19:25 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e3e797818bc929d95bae8220b7b6034b559c217ef5bf622dc7fedc8d270a48`  
		Last Modified: Sat, 11 Feb 2023 07:39:01 GMT  
		Size: 351.2 KB (351178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cebb4c80b3906a9b751ee9a512c1581331b1fd691c84f575c01a29e28403dde`  
		Last Modified: Sat, 11 Feb 2023 07:39:00 GMT  
		Size: 7.6 KB (7552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90648ba22c191b969d8db393bf6138e7d6ecc1b70b3865d1717ec4d663192d89`  
		Last Modified: Wed, 15 Feb 2023 19:19:52 GMT  
		Size: 14.3 MB (14282621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - linux; arm variant v6

```console
$ docker pull caddy@sha256:db317e683b30c11665349301255c3c59f3f5b085d4e075553e445129981ad5e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16582515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4628532cad0308b1d01506925ca941dffeb3bdd058cd79ccd7f055dce243e3b6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:32 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Fri, 10 Feb 2023 20:49:32 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 00:17:32 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 08 Mar 2023 00:17:34 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 08 Mar 2023 00:17:34 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:17:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 08 Mar 2023 00:17:38 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 08 Mar 2023 00:17:39 GMT
ENV XDG_DATA_HOME=/data
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 08 Mar 2023 00:17:41 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 80
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 443
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 443/udp
# Wed, 08 Mar 2023 00:17:42 GMT
EXPOSE 2019
# Wed, 08 Mar 2023 00:17:42 GMT
WORKDIR /srv
# Wed, 08 Mar 2023 00:17:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e676ebf894f684676e3a3c92294bbc14ba7061c7d24285909e673075903c39a9`  
		Last Modified: Wed, 08 Mar 2023 00:18:32 GMT  
		Size: 345.9 KB (345903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b146a16f288a28f362ad572b56958616fb5f4e0572bbe406ce18868be0d5c3`  
		Last Modified: Wed, 08 Mar 2023 00:18:31 GMT  
		Size: 7.6 KB (7559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e662de32a44a67eae886e653355902b11fec7407264122f1e72b5c460cb4334`  
		Last Modified: Wed, 08 Mar 2023 00:18:34 GMT  
		Size: 13.6 MB (13612275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - linux; arm variant v7

```console
$ docker pull caddy@sha256:03b5f2d631567d2783e8977e4988bdc75f13acb5c5b7bb18f3984045fb557b11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16365710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bed848976d2f2ce06398c52bf359363302bd512c4c51f08acb50cdd7ec0db5a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 10:40:15 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 02 Mar 2023 10:40:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 02 Mar 2023 10:40:16 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 02 Mar 2023 10:40:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 02 Mar 2023 10:40:19 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 02 Mar 2023 10:40:19 GMT
ENV XDG_DATA_HOME=/data
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 02 Mar 2023 10:40:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 02 Mar 2023 10:40:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 80
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 443
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 443/udp
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 2019
# Thu, 02 Mar 2023 10:40:20 GMT
WORKDIR /srv
# Thu, 02 Mar 2023 10:40:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769efc94ebb1351d7f88e191e0e5c768fc2462e89d73fa4b373005e8a912f367`  
		Last Modified: Thu, 02 Mar 2023 10:41:04 GMT  
		Size: 342.7 KB (342688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fb7d44b5e1d66fb60d8593e306cfef844841aca960cacb7258951888fcf79e`  
		Last Modified: Thu, 02 Mar 2023 10:41:04 GMT  
		Size: 7.6 KB (7560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818d68e9d461fbb298a8bb8f5467049d89e77e6324f72842c3d45e5af3d0767b`  
		Last Modified: Thu, 02 Mar 2023 10:41:06 GMT  
		Size: 13.6 MB (13594968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6c2623f6bf30798be5c37fc7484e45ecc288d493fb657883f59ddb27ed714ad8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16130997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a38afdc517ef4cff6b6b51a1c6a633c2826599b07feb1e88380d0f783e35cf1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:00:35 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:00:37 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 18:39:20 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 18:39:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 18:39:22 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 18:39:22 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 80
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 443
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 18:39:23 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 18:39:23 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70730e8e2fb933ec157ec87f2a4fb4ad45e8e578b8f7c76cc4846631d773554`  
		Last Modified: Fri, 10 Feb 2023 22:01:02 GMT  
		Size: 350.2 KB (350153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a4b7390d269477c225f1d03e825d2d8bdf6b4d87b5f7bb8811b341e56b7d36`  
		Last Modified: Fri, 10 Feb 2023 22:01:02 GMT  
		Size: 7.6 KB (7555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2743d2ef53ee6edb0e39c89bf16957e3a00990410b2d1a126dca1b2d196182`  
		Last Modified: Wed, 15 Feb 2023 18:39:53 GMT  
		Size: 13.1 MB (13063787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - linux; ppc64le

```console
$ docker pull caddy@sha256:8861ab3ae3d0c180e38142c2f7482f9ce1773419eb29ed9d6d18308246858093
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5819f0ab4928a30c29293a27299a3b44371cd3bd97df91432ef7b3f43b692d8c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:13:21 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:13:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:16:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:16:41 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:16:42 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:16:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:16:47 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:16:47 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:16:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bd0321e6539bb7dac8574fd36bad22059ef06bb63dc842165f69d0a821572`  
		Last Modified: Fri, 10 Feb 2023 22:14:16 GMT  
		Size: 363.1 KB (363088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb806b2600b0209a73fc7175ab778d0224661034b2f722bd1a0aec1eb9eabe3d`  
		Last Modified: Fri, 10 Feb 2023 22:14:15 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd7c8ae860931dd79dea76d33bc21bb11d89cd4d133cdb41078b040afc6633e`  
		Last Modified: Wed, 15 Feb 2023 19:17:41 GMT  
		Size: 12.8 MB (12779898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - linux; s390x

```console
$ docker pull caddy@sha256:4e1ed99f133abf02d6a7c77849978bb621f748e18c9cb9f7a1dbf88480ddb8d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45cd164da734310b788dcbd4f6c94bccff6e48705fe4d42ecca07a54e9459a9c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:31 GMT
ADD file:17af250b49631cf2acf655c85df90977eddab4c9afd67bda3c577db5200364f1 in / 
# Fri, 10 Feb 2023 21:41:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:14:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:14:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 18:41:48 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 18:41:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 18:41:59 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 18:41:59 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 18:42:00 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 18:42:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 18:42:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 18:42:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 18:42:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 18:42:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 18:42:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 18:42:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 18:42:05 GMT
EXPOSE 80
# Wed, 15 Feb 2023 18:42:06 GMT
EXPOSE 443
# Wed, 15 Feb 2023 18:42:07 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 18:42:07 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 18:42:08 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 18:42:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:667d93a24f321610e24486f3148545191f113ab9ab2444804087dd65ebbda9ed`  
		Last Modified: Fri, 10 Feb 2023 21:42:26 GMT  
		Size: 2.6 MB (2593581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e6ec82400496ce74e37120e1655955b79303daaa5b8ca7e956e3cd96ddd6e9`  
		Last Modified: Fri, 10 Feb 2023 22:15:05 GMT  
		Size: 352.8 KB (352801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5b992687f93ced3715ad97bd95ab37daef5685b784e195209caefbc48f14e9`  
		Last Modified: Fri, 10 Feb 2023 22:15:05 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ccc40924ce2df3343fa5465a92ccaa4ed80e0883190a99d3f468c60f9ddbcf8`  
		Last Modified: Wed, 15 Feb 2023 18:43:19 GMT  
		Size: 13.8 MB (13838817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - windows version 10.0.17763.4010; amd64

```console
$ docker pull caddy@sha256:f78e6d4fc1641b322d4e44adcada628f9acb5106b2e166cbcba796764a4db257
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1978492183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:198e4772b4788d7810819799af107998abe8e241416654ca5406331afefc2908`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:43:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:44:00 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:45:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:45:08 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:45:09 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:45:10 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:45:11 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:45:12 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:45:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:45:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:45:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:45:17 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:45:19 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:46:11 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:46:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f19b532038d3c84c40068e825815f2b252b82869809b11745d9893f12a99ac1`  
		Last Modified: Thu, 16 Feb 2023 02:51:03 GMT  
		Size: 526.3 KB (526332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15f6c8f1e7f194b2b408bf6c4330db67cf7cd4783d39acba2d8384b2f3c31d4`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab346a52e8e98a31f0970c85a32f1653b5179dd5ad781a8764b08de792a4d99`  
		Last Modified: Thu, 16 Feb 2023 02:51:05 GMT  
		Size: 14.7 MB (14677251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4451f67396ee792e3ace473ca4a69e5e49639ab8b620e489635a7b2eeb775523`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9291ccd53cd67f009cd59c77d90d2623192e5e134fc2ad5a03f1c1860ab66b80`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3096247c037e7418f5efc50ce5c7e6bc272ccac5c014f5cb085d77c4c28a3a`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f902038f4ba892bc3e1e4d5fdcef6b7759891c41c067b744fa3d5b008776c90`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82e400c4f2072b1e2b2ff49169de3108075208b544f454b3cdf016be6356321`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0944799324319439cbaf2f01dd147e8cc496ea80243ddc22e59e301237acb293`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce6c226ffeaa8146cae1b818b43a4776a06f6ce0be460b7d9b42fcc503b39db`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0b36e09fd7994e37dd27ccdcfa4610fc1219c4044a95695c6de9f9eecda63b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f284721a924468c7a0ff80b2809a222ae20cae99d35aa761b5296272783263b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bec609c0b4d99a9726ad86662d32a57664d18dde9d9087c0695ec7e9c4a47c`  
		Last Modified: Thu, 16 Feb 2023 02:50:59 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ad796550cc1ac21dd77352cf12cc78cacbd0a9f8a1e728e7e4f6a02a0cb9fb`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1955699b7dbbfef476622c70f983565943bafe8909c80ec278dff19509fad86`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4096827c6eb36146321a048a5041be746e60afe4c8e90717d681f2d271e0143`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc99e795e3855739a0c170e77263147dec07ac66a9ae51c306705be5af6574b`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8683be90a75d0e97aa8b7002c075e040e7299bd1fde397a541df3e7e4168d97`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 308.1 KB (308099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156392510131bc65057e3573b9aa9838fccd38cc8ed89734e5255bcd4a315274`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - windows version 10.0.20348.1547; amd64

```console
$ docker pull caddy@sha256:87b9acadc87fc1f78b7ee864f06462a0f45aa263af20fa1744e2f2a0d0870b02
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1695421581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaff43d5343d972f345ff5561ee131879eaafd463e389a1c2607715ac3f6e793`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:46:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:46:57 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:47:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:47:26 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:47:27 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:47:28 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:47:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:47:31 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:47:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:47:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:47:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:47:36 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:47:37 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:47:56 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:47:57 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1961fba6606566986ddd1960cf8309d19fa9deaa486f5a162a60114f3d4c3c82`  
		Last Modified: Thu, 16 Feb 2023 02:51:29 GMT  
		Size: 778.8 KB (778807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af5d76bf41697a16b3336a1857d1e530a3137f28d997c6f5eca0121d42ea88d`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d935f5b810851a2833b69e65d9dcff828f1c6686dab6fa117e9bd08eb95f5990`  
		Last Modified: Thu, 16 Feb 2023 02:51:31 GMT  
		Size: 14.9 MB (14914232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54e2a419181dd9257efde40f9ab80121dd6cc1a478f6ff42d160ddbf5e17cd4`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c07f1bbb0931b3148683baae55ab0d85f8576b2a1d8c2a59bb28544572b5a9d`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06073fd741cf5968f24574903b70213f9743b648ebec9c53ccb8fe114ce01ae`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a17243f1184726e21bf0821ee5984a84575b55befba72594fbf0b3a32a47f1`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c403099e0a283f6f2b25b4235c61c8b564a832643f33280253dc040d2a2ab07`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cc4608f06891b205fbec74e83a221161a2f9d9b50a0b548c3c716d176ee1a4`  
		Last Modified: Thu, 16 Feb 2023 02:51:25 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfe2ac143052b1fa8973567134244ce4ecd1693f16205dd53f0d4cf1b5caa5a`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e217159efeb187bf7ae9a12f6f70764141dd97837f24a517851bc15a36b552`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc05a7da758918922e168d1b07b29f4a81d398dc805724dd6b23b4cb28c7b43`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832768cea319f33011657944b08b51ea41229fdd7a37f21162dd8aedceb31a6b`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443fc82ac63aefa17f6de497731a007fbc972b175040388a8fda7112834af9fa`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39ff50a2c37b226c6e79e3789d1706fc47cb355b14372a147024fc11b2dfb2b`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c6037df6cbd4b9e046dded7157e841a1c40659c4dd082ff9d397c95be6e411`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a470cfe53e2d01e3ca43a7211eb050493a97f430e3c5a52e2364f54a0a4e4834`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d12a1c4350235354af8011d0b2eccb56884eea72a0475197fb007c4fa6c111`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 359.9 KB (359894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea80c894fe52045adaa4c44b9f66422259571c7aec153753d27a56aa3ccbd930`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-alpine`

```console
$ docker pull caddy@sha256:3f4414616d9141c4fbd9f66641d9b91a3b67833dd4145738c536dee584db5314
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
$ docker pull caddy@sha256:36ba71b44afa613ecf0aadce8e4b9e3f56e0c4b0a78c8edf4e8c2485f21b35ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17449113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8464e23f16f9a82426bbdc3ac8c94270a84453ddc86b9147505a2378a7c2fd0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:38:34 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 11 Feb 2023 07:38:36 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:19:21 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:19:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:19:23 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:19:24 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:19:25 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e3e797818bc929d95bae8220b7b6034b559c217ef5bf622dc7fedc8d270a48`  
		Last Modified: Sat, 11 Feb 2023 07:39:01 GMT  
		Size: 351.2 KB (351178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cebb4c80b3906a9b751ee9a512c1581331b1fd691c84f575c01a29e28403dde`  
		Last Modified: Sat, 11 Feb 2023 07:39:00 GMT  
		Size: 7.6 KB (7552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90648ba22c191b969d8db393bf6138e7d6ecc1b70b3865d1717ec4d663192d89`  
		Last Modified: Wed, 15 Feb 2023 19:19:52 GMT  
		Size: 14.3 MB (14282621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:db317e683b30c11665349301255c3c59f3f5b085d4e075553e445129981ad5e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16582515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4628532cad0308b1d01506925ca941dffeb3bdd058cd79ccd7f055dce243e3b6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:32 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Fri, 10 Feb 2023 20:49:32 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 00:17:32 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 08 Mar 2023 00:17:34 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 08 Mar 2023 00:17:34 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:17:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 08 Mar 2023 00:17:38 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 08 Mar 2023 00:17:39 GMT
ENV XDG_DATA_HOME=/data
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 08 Mar 2023 00:17:41 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 80
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 443
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 443/udp
# Wed, 08 Mar 2023 00:17:42 GMT
EXPOSE 2019
# Wed, 08 Mar 2023 00:17:42 GMT
WORKDIR /srv
# Wed, 08 Mar 2023 00:17:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e676ebf894f684676e3a3c92294bbc14ba7061c7d24285909e673075903c39a9`  
		Last Modified: Wed, 08 Mar 2023 00:18:32 GMT  
		Size: 345.9 KB (345903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b146a16f288a28f362ad572b56958616fb5f4e0572bbe406ce18868be0d5c3`  
		Last Modified: Wed, 08 Mar 2023 00:18:31 GMT  
		Size: 7.6 KB (7559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e662de32a44a67eae886e653355902b11fec7407264122f1e72b5c460cb4334`  
		Last Modified: Wed, 08 Mar 2023 00:18:34 GMT  
		Size: 13.6 MB (13612275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:03b5f2d631567d2783e8977e4988bdc75f13acb5c5b7bb18f3984045fb557b11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16365710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bed848976d2f2ce06398c52bf359363302bd512c4c51f08acb50cdd7ec0db5a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 10:40:15 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 02 Mar 2023 10:40:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 02 Mar 2023 10:40:16 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 02 Mar 2023 10:40:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 02 Mar 2023 10:40:19 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 02 Mar 2023 10:40:19 GMT
ENV XDG_DATA_HOME=/data
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 02 Mar 2023 10:40:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 02 Mar 2023 10:40:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 80
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 443
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 443/udp
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 2019
# Thu, 02 Mar 2023 10:40:20 GMT
WORKDIR /srv
# Thu, 02 Mar 2023 10:40:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769efc94ebb1351d7f88e191e0e5c768fc2462e89d73fa4b373005e8a912f367`  
		Last Modified: Thu, 02 Mar 2023 10:41:04 GMT  
		Size: 342.7 KB (342688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fb7d44b5e1d66fb60d8593e306cfef844841aca960cacb7258951888fcf79e`  
		Last Modified: Thu, 02 Mar 2023 10:41:04 GMT  
		Size: 7.6 KB (7560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818d68e9d461fbb298a8bb8f5467049d89e77e6324f72842c3d45e5af3d0767b`  
		Last Modified: Thu, 02 Mar 2023 10:41:06 GMT  
		Size: 13.6 MB (13594968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6c2623f6bf30798be5c37fc7484e45ecc288d493fb657883f59ddb27ed714ad8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16130997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a38afdc517ef4cff6b6b51a1c6a633c2826599b07feb1e88380d0f783e35cf1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:00:35 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:00:37 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 18:39:20 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 18:39:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 18:39:22 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 18:39:22 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 80
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 443
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 18:39:23 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 18:39:23 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70730e8e2fb933ec157ec87f2a4fb4ad45e8e578b8f7c76cc4846631d773554`  
		Last Modified: Fri, 10 Feb 2023 22:01:02 GMT  
		Size: 350.2 KB (350153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a4b7390d269477c225f1d03e825d2d8bdf6b4d87b5f7bb8811b341e56b7d36`  
		Last Modified: Fri, 10 Feb 2023 22:01:02 GMT  
		Size: 7.6 KB (7555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2743d2ef53ee6edb0e39c89bf16957e3a00990410b2d1a126dca1b2d196182`  
		Last Modified: Wed, 15 Feb 2023 18:39:53 GMT  
		Size: 13.1 MB (13063787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:8861ab3ae3d0c180e38142c2f7482f9ce1773419eb29ed9d6d18308246858093
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5819f0ab4928a30c29293a27299a3b44371cd3bd97df91432ef7b3f43b692d8c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:13:21 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:13:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:16:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:16:41 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:16:42 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:16:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:16:47 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:16:47 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:16:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bd0321e6539bb7dac8574fd36bad22059ef06bb63dc842165f69d0a821572`  
		Last Modified: Fri, 10 Feb 2023 22:14:16 GMT  
		Size: 363.1 KB (363088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb806b2600b0209a73fc7175ab778d0224661034b2f722bd1a0aec1eb9eabe3d`  
		Last Modified: Fri, 10 Feb 2023 22:14:15 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd7c8ae860931dd79dea76d33bc21bb11d89cd4d133cdb41078b040afc6633e`  
		Last Modified: Wed, 15 Feb 2023 19:17:41 GMT  
		Size: 12.8 MB (12779898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:4e1ed99f133abf02d6a7c77849978bb621f748e18c9cb9f7a1dbf88480ddb8d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45cd164da734310b788dcbd4f6c94bccff6e48705fe4d42ecca07a54e9459a9c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:31 GMT
ADD file:17af250b49631cf2acf655c85df90977eddab4c9afd67bda3c577db5200364f1 in / 
# Fri, 10 Feb 2023 21:41:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:14:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:14:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 18:41:48 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 18:41:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 18:41:59 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 18:41:59 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 18:42:00 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 18:42:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 18:42:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 18:42:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 18:42:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 18:42:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 18:42:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 18:42:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 18:42:05 GMT
EXPOSE 80
# Wed, 15 Feb 2023 18:42:06 GMT
EXPOSE 443
# Wed, 15 Feb 2023 18:42:07 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 18:42:07 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 18:42:08 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 18:42:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:667d93a24f321610e24486f3148545191f113ab9ab2444804087dd65ebbda9ed`  
		Last Modified: Fri, 10 Feb 2023 21:42:26 GMT  
		Size: 2.6 MB (2593581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e6ec82400496ce74e37120e1655955b79303daaa5b8ca7e956e3cd96ddd6e9`  
		Last Modified: Fri, 10 Feb 2023 22:15:05 GMT  
		Size: 352.8 KB (352801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5b992687f93ced3715ad97bd95ab37daef5685b784e195209caefbc48f14e9`  
		Last Modified: Fri, 10 Feb 2023 22:15:05 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ccc40924ce2df3343fa5465a92ccaa4ed80e0883190a99d3f468c60f9ddbcf8`  
		Last Modified: Wed, 15 Feb 2023 18:43:19 GMT  
		Size: 13.8 MB (13838817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder`

```console
$ docker pull caddy@sha256:8fe3549f0a6c0db646ec94d25f0c2a87ea055f50cb73477405df8f6fd2349784
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4010; amd64
	-	windows version 10.0.20348.1547; amd64

### `caddy:2.6-builder` - linux; amd64

```console
$ docker pull caddy@sha256:47722ffc694507be1e2f34ca172e292fb5e226ea68d87871300b9d65f543fcce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131421587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4674ac67a52f4d29bc8349e9dcca7db8393d778c97c79d9e2f6e997603a99cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 08:21:54 GMT
RUN apk add --no-cache ca-certificates
# Sat, 11 Feb 2023 08:21:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:24:10 GMT
ENV GOLANG_VERSION=1.19.6
# Tue, 14 Feb 2023 19:25:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 14 Feb 2023 19:25:43 GMT
ENV GOPATH=/go
# Tue, 14 Feb 2023 19:25:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:25:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Feb 2023 19:25:44 GMT
WORKDIR /go
# Tue, 14 Feb 2023 19:47:10 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 14 Feb 2023 19:47:10 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 15 Feb 2023 19:19:27 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:19:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 15 Feb 2023 19:19:28 GMT
ENV XCADDY_SETCAP=1
# Wed, 15 Feb 2023 19:19:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 15 Feb 2023 19:19:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 15 Feb 2023 19:19:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d21d5440ebff5aaaaeb115a003f7a4a3897f1866a87de95bc4a21436fc563c`  
		Last Modified: Sat, 11 Feb 2023 08:29:10 GMT  
		Size: 284.8 KB (284816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f790f4c5274f100158d4c23bc5eddf659c1fe93ef4025488f9493d88f1490d88`  
		Last Modified: Tue, 14 Feb 2023 19:31:12 GMT  
		Size: 122.4 MB (122355677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bf170fd9e6726c86c0d4b478d9ec522e82c527a8e708668f48233a4d03f618`  
		Last Modified: Tue, 14 Feb 2023 19:30:55 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a5d1c1b6ed103f8c7f97c73ed546ff7e767b10473b55c15c0d4e1a13a69481`  
		Last Modified: Tue, 14 Feb 2023 19:47:34 GMT  
		Size: 4.2 MB (4188243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0130eaa2f0b1f7646719d82927743bd84c83ed450eb8be4db5327d280d5e4d0`  
		Last Modified: Wed, 15 Feb 2023 19:20:05 GMT  
		Size: 1.2 MB (1217841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab1f57409241476a86d26944527bc2c6c3903eadb21221b8d96da52120b3109`  
		Last Modified: Wed, 15 Feb 2023 19:20:05 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e2b8479c011649b6d47ead7051ebf36d10e2c764f2bc3bc507eab00a1812b6a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127455561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7351cc9a113eeb1deb8afa4c19e381df6b5e03cfef4e63e47bfe99f0b43d95ab`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:28 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Fri, 10 Feb 2023 20:49:28 GMT
CMD ["/bin/sh"]
# Tue, 07 Mar 2023 23:49:29 GMT
RUN apk add --no-cache ca-certificates
# Tue, 07 Mar 2023 23:49:29 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:53:43 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:55:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:55:31 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:55:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:55:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:55:32 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:17:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:17:50 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:17:50 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:17:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:17:51 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:17:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:17:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:17:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06dc45fa3a2f6e0270fe56d6b9f8efada3c9b5854707b52fe42dd55844fb1d5`  
		Last Modified: Tue, 07 Mar 2023 23:58:16 GMT  
		Size: 286.2 KB (286214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9c435c140baf308bcd21b10be4fe27e2cec5ec2acccb0cba35e7ec207d54ae`  
		Last Modified: Tue, 07 Mar 2023 23:59:54 GMT  
		Size: 118.7 MB (118731518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f756f642eb6722bcddfd36a868987c31f5583a7bac2ccf573f8c4fc55198ad49`  
		Last Modified: Tue, 07 Mar 2023 23:59:33 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c49be1b95c6f947e8aaed6708b2c0b38ea78e63b117ac389af00cca5f95334f`  
		Last Modified: Wed, 08 Mar 2023 00:18:51 GMT  
		Size: 4.2 MB (4160310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1cd39813132ad141affe91c6d7f78654e7dbe1e8454baf43e2ee60f2480ecd`  
		Last Modified: Wed, 08 Mar 2023 00:18:51 GMT  
		Size: 1.2 MB (1166071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6624093c59eca00c1b574cd2672bb86cf72a602c484c89dd864ab09d28d875b`  
		Last Modified: Wed, 08 Mar 2023 00:18:50 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:35dc985cc319ba4cd38b0f28d82ec4af14971a9336ce7870444c023c1415fa7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126524974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:822857d40d7e456ebf6b4405bd126f6499dd89ce092e55728fa8deaea4601da8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 02:15:04 GMT
RUN apk add --no-cache ca-certificates
# Thu, 02 Mar 2023 02:15:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 02:19:52 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 02 Mar 2023 02:21:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 02 Mar 2023 02:21:35 GMT
ENV GOPATH=/go
# Thu, 02 Mar 2023 02:21:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 02:21:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 02 Mar 2023 02:21:35 GMT
WORKDIR /go
# Thu, 02 Mar 2023 10:40:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 02 Mar 2023 10:40:26 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_SETCAP=1
# Thu, 02 Mar 2023 10:40:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 02 Mar 2023 10:40:28 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 02 Mar 2023 10:40:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4962ca8504034f69427a90f2b07cfde1e4c20297e4507d5620bb7ea27e646919`  
		Last Modified: Thu, 02 Mar 2023 02:26:02 GMT  
		Size: 285.4 KB (285445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20059bad54d9966d7995685d0c72ce1566c6370b4105df472360f5d2c8ecd21`  
		Last Modified: Thu, 02 Mar 2023 02:28:31 GMT  
		Size: 118.5 MB (118477876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4d49a4d60a68cc1326493b7f8b4cf548d4cec1694b7ccb266f06e4028b501d`  
		Last Modified: Thu, 02 Mar 2023 02:28:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0098f26d1429a39f7d8f6dd18417972d79d6706e530dbfbc4cf9991ff98f3c6`  
		Last Modified: Thu, 02 Mar 2023 10:41:22 GMT  
		Size: 3.7 MB (3729269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0aafe51cc793a860e8c2f2c4799c11f9bebe521643a6f6578f348ce06ae80d`  
		Last Modified: Thu, 02 Mar 2023 10:41:22 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24f3750a2b57fead59e3d812fa66ae7c79703a8a84d41670403b9dc7c23eb90`  
		Last Modified: Thu, 02 Mar 2023 10:41:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6e43472efedad7b414f4cce21a50e04578ea8527ad05ee901ba9eabc88d7718e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125849779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62beb7ef29ce475cb1f571275d3c9ac33185ec48844366ef16a99e8540239b2b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:38:33 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:38:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:43:17 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:44:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:44:26 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:44:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:44:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:44:27 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:06:06 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:06:06 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:06:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:06:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:06:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55522c79112429742fe76c795b9509c5cd1e8198e0caa2a1e355c0e60a719576`  
		Last Modified: Fri, 10 Feb 2023 22:44:19 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1815dcbf43e87e122cc76a24663b7c0d6e01ad03c3be30a7dc13c1bf941c595`  
		Last Modified: Tue, 07 Mar 2023 23:49:19 GMT  
		Size: 116.9 MB (116933985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5aad4e0c6f77e535fe5a51a211a4691a5002a111c52fa17708cf1bc7c01879`  
		Last Modified: Tue, 07 Mar 2023 23:49:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557acb83c53566587727172247e84b25f860b606c200b1fc863eafc75d6b0cf4`  
		Last Modified: Wed, 08 Mar 2023 00:06:29 GMT  
		Size: 4.2 MB (4243285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb71700cd911a18f7eb1f75d651639bc79bda4000e2f4e6a8afe570b03816eb`  
		Last Modified: Wed, 08 Mar 2023 00:06:29 GMT  
		Size: 1.1 MB (1123733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358517d9544ce3184d74860b7f2054339481407b928bb11ccbf7d35163006788`  
		Last Modified: Wed, 08 Mar 2023 00:06:28 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:8126a0d2b7cc9613f70b6b5375c14cc61dfca5dc1b83adc5be33efab8eacc69f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126579575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2da1cd24f35f4106a8a7176a2f2b5656a22982a1787b9204d3eaab9ec535ef58`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:40:13 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:40:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:46:09 GMT
ENV GOLANG_VERSION=1.19.6
# Tue, 14 Feb 2023 19:48:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 14 Feb 2023 19:48:44 GMT
ENV GOPATH=/go
# Tue, 14 Feb 2023 19:48:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:48:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Feb 2023 19:48:46 GMT
WORKDIR /go
# Tue, 14 Feb 2023 20:12:48 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 14 Feb 2023 20:12:48 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 15 Feb 2023 19:16:53 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 15 Feb 2023 19:16:54 GMT
ENV XCADDY_SETCAP=1
# Wed, 15 Feb 2023 19:16:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 15 Feb 2023 19:16:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 15 Feb 2023 19:16:57 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788962e1689dbb14c760601cbf633ae350e98e3a045f8010924cd585de6b6a3e`  
		Last Modified: Fri, 10 Feb 2023 22:53:32 GMT  
		Size: 286.6 KB (286645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ae39b9ad00c218f9156f0958fa48f3062eb5830b791b8592e5f25fd576c7c5`  
		Last Modified: Tue, 14 Feb 2023 19:56:18 GMT  
		Size: 117.3 MB (117316160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f3bf55d586b31bb5c97f2cbf5167fd359b61336f93bed839c2f4de055ced88`  
		Last Modified: Tue, 14 Feb 2023 19:55:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e012d53123423a5fe128ab31d41596d83d8e48699ad608e9eb58dd0b2322fe0`  
		Last Modified: Tue, 14 Feb 2023 20:13:35 GMT  
		Size: 4.5 MB (4479556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90177e6cf58218f094608b8401f41d0da78a0cf57d95718e48e8c6e2f77c6fae`  
		Last Modified: Wed, 15 Feb 2023 19:18:00 GMT  
		Size: 1.1 MB (1105899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e897949e5a46b09b4606d86b20ecb5684cb43f7e1bed1f208ee9b7e93d208c`  
		Last Modified: Wed, 15 Feb 2023 19:17:59 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; s390x

```console
$ docker pull caddy@sha256:8c80a3ba9211715e4a4892ab129d736ec6405a52630b14b828837b7307115c02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129610728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e05d79b3ea15e4e9b6f3f1a89c9e9b9580f66c78fcef17624a8c7bb9f3f51cb5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:27:44 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:27:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:47:03 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:48:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:48:53 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:48:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:48:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:48:53 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:10:01 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:10:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:10:01 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:10:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:10:02 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:10:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:10:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:10:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affa53ed2f1b70a83e3a15cae881ca47cd40f6ac11060717cdbbd4e405f9d586`  
		Last Modified: Fri, 10 Feb 2023 22:37:18 GMT  
		Size: 285.0 KB (285032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d83de48b90cbc8ae74a05d0af343e28f82727b9797b0b45ed9a70fa837a9a5`  
		Last Modified: Tue, 07 Mar 2023 23:53:54 GMT  
		Size: 120.8 MB (120808046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d22668a5d7432e1f8abda37a563ffa67f01cd8658b3247b89a7770eb41fe2a0`  
		Last Modified: Tue, 07 Mar 2023 23:53:38 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3beeef51570794945ced834a4af09db492ac50aadef9f4120ccc6b1dcb4f1251`  
		Last Modified: Wed, 08 Mar 2023 00:10:47 GMT  
		Size: 4.2 MB (4171573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57140a7518a2548d3fd2cef1ecb24c3b4ffb6aee2cc51f3921cb5497bf0863ce`  
		Last Modified: Wed, 08 Mar 2023 00:10:38 GMT  
		Size: 1.2 MB (1170402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe35434ab4b6dfcd2742bd2454af4cb9fe85cc900cacf2e2ef375861498fa09e`  
		Last Modified: Wed, 08 Mar 2023 00:10:38 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - windows version 10.0.17763.4010; amd64

```console
$ docker pull caddy@sha256:698c8dda106fb34e783e5030fd3ea5166df618f08c2a01204a7a82aabf6b20c9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2148348831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cee813843af987f6985470a05839367529db056040844b778343ebd71743f6a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 23:47:41 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Feb 2023 23:47:42 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Feb 2023 23:47:43 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Feb 2023 23:47:44 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Feb 2023 23:50:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Feb 2023 23:50:19 GMT
ENV GOPATH=C:\go
# Wed, 15 Feb 2023 23:51:42 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Feb 2023 00:11:44 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 16 Feb 2023 00:17:12 GMT
RUN $url = 'https://dl.google.com/go/go1.19.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '8d84af29e46c38b1eec77f9310310517c9e394ac7489e1c7329a94b443b0388d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Feb 2023 00:17:13 GMT
WORKDIR C:\go
# Thu, 16 Feb 2023 02:48:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:48:16 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Feb 2023 02:48:17 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:48:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Feb 2023 02:49:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Feb 2023 02:49:37 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03ac75ee62e05ad7b8b8f97fb78a769177c49d210eedcf0a93035e9a07d0ff2`  
		Last Modified: Thu, 16 Feb 2023 00:28:24 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4beb360c9024340aa5072ce67eab6b3cb005293938525c4f3b77c3bb03f9f501`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5051ce7a895da09ac63e7ca01ef4e30434d833dbd271107d6f96375f291752ad`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea419e1594fbbef3584b4731c356499c7b8a5616af16968e6fd693eccd92012b`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb97c6a047d2cfcb6f0ef6846e78c4d5f60212639a9d1892e2af05033c217df`  
		Last Modified: Thu, 16 Feb 2023 00:28:30 GMT  
		Size: 25.6 MB (25606151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941d25224d4bab25ba0b2304a5811b0fc2970ba6385afdbefbfec898720c3beb`  
		Last Modified: Thu, 16 Feb 2023 00:28:17 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa161895f771062e6d8e8aa2e0e44c15c5affdacc8d409f6e70f1fa743a9bb1`  
		Last Modified: Thu, 16 Feb 2023 00:28:17 GMT  
		Size: 335.6 KB (335550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd14ed3be87ab223f1391d40c3cdcfcee876586e89fbeed2aeccb318734a22`  
		Last Modified: Thu, 16 Feb 2023 00:32:40 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddec1d087c619cf7156e3dba04dd6a73e704d66c60e3fbc4b32c73b4401471b`  
		Last Modified: Thu, 16 Feb 2023 00:33:24 GMT  
		Size: 157.8 MB (157798436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50612066f9b2d86b5cecd95ce6897d89929be6a819c3de13dd9ecc32948832cb`  
		Last Modified: Thu, 16 Feb 2023 00:32:40 GMT  
		Size: 1.5 KB (1544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3bbcb2df900a9ead208e08eefd6faa32bbd6c5a189212d97b94eec1e5807a24`  
		Last Modified: Thu, 16 Feb 2023 02:51:49 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b5e7db448c55e5e60ab1aefceb414700fb99de06cc1c047404e32031064e0c`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7af0982eb604918cfaece327a35d278b59d5f2ca440882b5e7d402e7cce80f6`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad49ef8883b47edaa38ca21b422551a4da50f675370fc1596432938cd7de4d2`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce066417e925c257e21d7126cbbdcf5316022725a7ef7a89575b86fd534d133f`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.6 MB (1632671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbe58e4b6c6b7d8f16c2682325b6df5f61050915e6af7829adab49c1914e5c9`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - windows version 10.0.20348.1547; amd64

```console
$ docker pull caddy@sha256:21d50bd59eead7016b606e72f6dede55b7f2c718f306c823f3a34ef794622aa7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1865665598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f3a334b2d908beba62aa4ea43b950f4be8fa2261a29819fecc52e58eaadf2df`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 23:42:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Feb 2023 23:42:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Feb 2023 23:42:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Feb 2023 23:42:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Feb 2023 23:43:27 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Feb 2023 23:43:28 GMT
ENV GOPATH=C:\go
# Wed, 15 Feb 2023 23:44:03 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Feb 2023 00:07:02 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 16 Feb 2023 00:11:25 GMT
RUN $url = 'https://dl.google.com/go/go1.19.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '8d84af29e46c38b1eec77f9310310517c9e394ac7489e1c7329a94b443b0388d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Feb 2023 00:11:27 GMT
WORKDIR C:\go
# Thu, 16 Feb 2023 02:49:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:49:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Feb 2023 02:49:47 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:49:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Feb 2023 02:50:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Feb 2023 02:50:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4048a86b3278e59b840ad06b4cf5f5888ce1068d503522a95eb470d5126ed69a`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b07973952171f91c05aade363f3e6c9a2e84548f33eaa3c8e48632460e61f8`  
		Last Modified: Thu, 16 Feb 2023 00:26:45 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a95dff10905572b5f9177959a5a9f60a9364e1dd627ed52e34ec4bee3fb3069`  
		Last Modified: Thu, 16 Feb 2023 00:26:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4267caf437f5a3d92235ab7b8d55b2c812744f166725151ba701aef9d682c6e9`  
		Last Modified: Thu, 16 Feb 2023 00:26:41 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982a959ece2e33bce3f35c5c0adb01a3426c92111b309c15f8cc31200ebcf899`  
		Last Modified: Thu, 16 Feb 2023 00:26:54 GMT  
		Size: 25.9 MB (25852811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065416c07c5d80f7a085e0e84237051d7050a71103cc9d7fb6d5ef57725dc4c6`  
		Last Modified: Thu, 16 Feb 2023 00:26:39 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07015cae66c7ebb6b0adce2dfe424313b228bb703ac3e900deebe74ae961bb49`  
		Last Modified: Thu, 16 Feb 2023 00:26:40 GMT  
		Size: 571.7 KB (571672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285847798b3738c8863954b395d2e44410be1004e9f8513dd1546a0713f153d3`  
		Last Modified: Thu, 16 Feb 2023 00:31:40 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4f6797c9312e8b2093037565c19561d6152cca51a84614b32c0813526f219f`  
		Last Modified: Thu, 16 Feb 2023 00:32:31 GMT  
		Size: 158.0 MB (158008192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2bd8446758388c6c8ddb5d51dd63d25a0dbf5c8e1385928c5e64c83948d966`  
		Last Modified: Thu, 16 Feb 2023 00:31:40 GMT  
		Size: 1.6 KB (1561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd741098e5131c0452f3451d13ce2b131c36cbfcf24df5fbd2fb9e5751e85627`  
		Last Modified: Thu, 16 Feb 2023 02:52:08 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcd5d2a85aea028cd55d32ae579beb21aa5efc8eb3875d901dfcb623092327a`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f63b7e14eef097ca8f36e589d8d609a276d3196875467da71a714db6c8e583`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2e98e1ab65293643e4b2173a01d386c2129bf22ffaee5d1b730f19a26759a7`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15030494f30adf45739bdc5e411e1ae7ea0395ebcb4c2a4f74eedbc5f71d3acd`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.9 MB (1868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba874cf328299688fd26dd5261c439698422f93ce708e583e0e248444622caff`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder-alpine`

```console
$ docker pull caddy@sha256:68f552074b7668f5c49a7545bad89568f46b134851ee4bb7f558fe6b2e7b7749
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
$ docker pull caddy@sha256:47722ffc694507be1e2f34ca172e292fb5e226ea68d87871300b9d65f543fcce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131421587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4674ac67a52f4d29bc8349e9dcca7db8393d778c97c79d9e2f6e997603a99cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 08:21:54 GMT
RUN apk add --no-cache ca-certificates
# Sat, 11 Feb 2023 08:21:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:24:10 GMT
ENV GOLANG_VERSION=1.19.6
# Tue, 14 Feb 2023 19:25:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 14 Feb 2023 19:25:43 GMT
ENV GOPATH=/go
# Tue, 14 Feb 2023 19:25:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:25:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Feb 2023 19:25:44 GMT
WORKDIR /go
# Tue, 14 Feb 2023 19:47:10 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 14 Feb 2023 19:47:10 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 15 Feb 2023 19:19:27 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:19:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 15 Feb 2023 19:19:28 GMT
ENV XCADDY_SETCAP=1
# Wed, 15 Feb 2023 19:19:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 15 Feb 2023 19:19:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 15 Feb 2023 19:19:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d21d5440ebff5aaaaeb115a003f7a4a3897f1866a87de95bc4a21436fc563c`  
		Last Modified: Sat, 11 Feb 2023 08:29:10 GMT  
		Size: 284.8 KB (284816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f790f4c5274f100158d4c23bc5eddf659c1fe93ef4025488f9493d88f1490d88`  
		Last Modified: Tue, 14 Feb 2023 19:31:12 GMT  
		Size: 122.4 MB (122355677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bf170fd9e6726c86c0d4b478d9ec522e82c527a8e708668f48233a4d03f618`  
		Last Modified: Tue, 14 Feb 2023 19:30:55 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a5d1c1b6ed103f8c7f97c73ed546ff7e767b10473b55c15c0d4e1a13a69481`  
		Last Modified: Tue, 14 Feb 2023 19:47:34 GMT  
		Size: 4.2 MB (4188243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0130eaa2f0b1f7646719d82927743bd84c83ed450eb8be4db5327d280d5e4d0`  
		Last Modified: Wed, 15 Feb 2023 19:20:05 GMT  
		Size: 1.2 MB (1217841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab1f57409241476a86d26944527bc2c6c3903eadb21221b8d96da52120b3109`  
		Last Modified: Wed, 15 Feb 2023 19:20:05 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e2b8479c011649b6d47ead7051ebf36d10e2c764f2bc3bc507eab00a1812b6a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127455561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7351cc9a113eeb1deb8afa4c19e381df6b5e03cfef4e63e47bfe99f0b43d95ab`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:28 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Fri, 10 Feb 2023 20:49:28 GMT
CMD ["/bin/sh"]
# Tue, 07 Mar 2023 23:49:29 GMT
RUN apk add --no-cache ca-certificates
# Tue, 07 Mar 2023 23:49:29 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:53:43 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:55:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:55:31 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:55:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:55:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:55:32 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:17:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:17:50 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:17:50 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:17:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:17:51 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:17:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:17:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:17:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06dc45fa3a2f6e0270fe56d6b9f8efada3c9b5854707b52fe42dd55844fb1d5`  
		Last Modified: Tue, 07 Mar 2023 23:58:16 GMT  
		Size: 286.2 KB (286214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9c435c140baf308bcd21b10be4fe27e2cec5ec2acccb0cba35e7ec207d54ae`  
		Last Modified: Tue, 07 Mar 2023 23:59:54 GMT  
		Size: 118.7 MB (118731518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f756f642eb6722bcddfd36a868987c31f5583a7bac2ccf573f8c4fc55198ad49`  
		Last Modified: Tue, 07 Mar 2023 23:59:33 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c49be1b95c6f947e8aaed6708b2c0b38ea78e63b117ac389af00cca5f95334f`  
		Last Modified: Wed, 08 Mar 2023 00:18:51 GMT  
		Size: 4.2 MB (4160310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1cd39813132ad141affe91c6d7f78654e7dbe1e8454baf43e2ee60f2480ecd`  
		Last Modified: Wed, 08 Mar 2023 00:18:51 GMT  
		Size: 1.2 MB (1166071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6624093c59eca00c1b574cd2672bb86cf72a602c484c89dd864ab09d28d875b`  
		Last Modified: Wed, 08 Mar 2023 00:18:50 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:35dc985cc319ba4cd38b0f28d82ec4af14971a9336ce7870444c023c1415fa7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126524974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:822857d40d7e456ebf6b4405bd126f6499dd89ce092e55728fa8deaea4601da8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 02:15:04 GMT
RUN apk add --no-cache ca-certificates
# Thu, 02 Mar 2023 02:15:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 02:19:52 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 02 Mar 2023 02:21:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 02 Mar 2023 02:21:35 GMT
ENV GOPATH=/go
# Thu, 02 Mar 2023 02:21:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 02:21:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 02 Mar 2023 02:21:35 GMT
WORKDIR /go
# Thu, 02 Mar 2023 10:40:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 02 Mar 2023 10:40:26 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_SETCAP=1
# Thu, 02 Mar 2023 10:40:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 02 Mar 2023 10:40:28 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 02 Mar 2023 10:40:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4962ca8504034f69427a90f2b07cfde1e4c20297e4507d5620bb7ea27e646919`  
		Last Modified: Thu, 02 Mar 2023 02:26:02 GMT  
		Size: 285.4 KB (285445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20059bad54d9966d7995685d0c72ce1566c6370b4105df472360f5d2c8ecd21`  
		Last Modified: Thu, 02 Mar 2023 02:28:31 GMT  
		Size: 118.5 MB (118477876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4d49a4d60a68cc1326493b7f8b4cf548d4cec1694b7ccb266f06e4028b501d`  
		Last Modified: Thu, 02 Mar 2023 02:28:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0098f26d1429a39f7d8f6dd18417972d79d6706e530dbfbc4cf9991ff98f3c6`  
		Last Modified: Thu, 02 Mar 2023 10:41:22 GMT  
		Size: 3.7 MB (3729269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0aafe51cc793a860e8c2f2c4799c11f9bebe521643a6f6578f348ce06ae80d`  
		Last Modified: Thu, 02 Mar 2023 10:41:22 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24f3750a2b57fead59e3d812fa66ae7c79703a8a84d41670403b9dc7c23eb90`  
		Last Modified: Thu, 02 Mar 2023 10:41:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6e43472efedad7b414f4cce21a50e04578ea8527ad05ee901ba9eabc88d7718e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125849779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62beb7ef29ce475cb1f571275d3c9ac33185ec48844366ef16a99e8540239b2b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:38:33 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:38:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:43:17 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:44:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:44:26 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:44:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:44:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:44:27 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:06:06 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:06:06 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:06:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:06:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:06:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55522c79112429742fe76c795b9509c5cd1e8198e0caa2a1e355c0e60a719576`  
		Last Modified: Fri, 10 Feb 2023 22:44:19 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1815dcbf43e87e122cc76a24663b7c0d6e01ad03c3be30a7dc13c1bf941c595`  
		Last Modified: Tue, 07 Mar 2023 23:49:19 GMT  
		Size: 116.9 MB (116933985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5aad4e0c6f77e535fe5a51a211a4691a5002a111c52fa17708cf1bc7c01879`  
		Last Modified: Tue, 07 Mar 2023 23:49:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557acb83c53566587727172247e84b25f860b606c200b1fc863eafc75d6b0cf4`  
		Last Modified: Wed, 08 Mar 2023 00:06:29 GMT  
		Size: 4.2 MB (4243285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb71700cd911a18f7eb1f75d651639bc79bda4000e2f4e6a8afe570b03816eb`  
		Last Modified: Wed, 08 Mar 2023 00:06:29 GMT  
		Size: 1.1 MB (1123733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358517d9544ce3184d74860b7f2054339481407b928bb11ccbf7d35163006788`  
		Last Modified: Wed, 08 Mar 2023 00:06:28 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:8126a0d2b7cc9613f70b6b5375c14cc61dfca5dc1b83adc5be33efab8eacc69f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126579575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2da1cd24f35f4106a8a7176a2f2b5656a22982a1787b9204d3eaab9ec535ef58`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:40:13 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:40:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:46:09 GMT
ENV GOLANG_VERSION=1.19.6
# Tue, 14 Feb 2023 19:48:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 14 Feb 2023 19:48:44 GMT
ENV GOPATH=/go
# Tue, 14 Feb 2023 19:48:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:48:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Feb 2023 19:48:46 GMT
WORKDIR /go
# Tue, 14 Feb 2023 20:12:48 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 14 Feb 2023 20:12:48 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 15 Feb 2023 19:16:53 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 15 Feb 2023 19:16:54 GMT
ENV XCADDY_SETCAP=1
# Wed, 15 Feb 2023 19:16:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 15 Feb 2023 19:16:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 15 Feb 2023 19:16:57 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788962e1689dbb14c760601cbf633ae350e98e3a045f8010924cd585de6b6a3e`  
		Last Modified: Fri, 10 Feb 2023 22:53:32 GMT  
		Size: 286.6 KB (286645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ae39b9ad00c218f9156f0958fa48f3062eb5830b791b8592e5f25fd576c7c5`  
		Last Modified: Tue, 14 Feb 2023 19:56:18 GMT  
		Size: 117.3 MB (117316160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f3bf55d586b31bb5c97f2cbf5167fd359b61336f93bed839c2f4de055ced88`  
		Last Modified: Tue, 14 Feb 2023 19:55:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e012d53123423a5fe128ab31d41596d83d8e48699ad608e9eb58dd0b2322fe0`  
		Last Modified: Tue, 14 Feb 2023 20:13:35 GMT  
		Size: 4.5 MB (4479556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90177e6cf58218f094608b8401f41d0da78a0cf57d95718e48e8c6e2f77c6fae`  
		Last Modified: Wed, 15 Feb 2023 19:18:00 GMT  
		Size: 1.1 MB (1105899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e897949e5a46b09b4606d86b20ecb5684cb43f7e1bed1f208ee9b7e93d208c`  
		Last Modified: Wed, 15 Feb 2023 19:17:59 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:8c80a3ba9211715e4a4892ab129d736ec6405a52630b14b828837b7307115c02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129610728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e05d79b3ea15e4e9b6f3f1a89c9e9b9580f66c78fcef17624a8c7bb9f3f51cb5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:27:44 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:27:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:47:03 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:48:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:48:53 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:48:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:48:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:48:53 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:10:01 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:10:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:10:01 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:10:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:10:02 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:10:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:10:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:10:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affa53ed2f1b70a83e3a15cae881ca47cd40f6ac11060717cdbbd4e405f9d586`  
		Last Modified: Fri, 10 Feb 2023 22:37:18 GMT  
		Size: 285.0 KB (285032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d83de48b90cbc8ae74a05d0af343e28f82727b9797b0b45ed9a70fa837a9a5`  
		Last Modified: Tue, 07 Mar 2023 23:53:54 GMT  
		Size: 120.8 MB (120808046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d22668a5d7432e1f8abda37a563ffa67f01cd8658b3247b89a7770eb41fe2a0`  
		Last Modified: Tue, 07 Mar 2023 23:53:38 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3beeef51570794945ced834a4af09db492ac50aadef9f4120ccc6b1dcb4f1251`  
		Last Modified: Wed, 08 Mar 2023 00:10:47 GMT  
		Size: 4.2 MB (4171573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57140a7518a2548d3fd2cef1ecb24c3b4ffb6aee2cc51f3921cb5497bf0863ce`  
		Last Modified: Wed, 08 Mar 2023 00:10:38 GMT  
		Size: 1.2 MB (1170402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe35434ab4b6dfcd2742bd2454af4cb9fe85cc900cacf2e2ef375861498fa09e`  
		Last Modified: Wed, 08 Mar 2023 00:10:38 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:687ff9a9e85091470e7d84be08a4e96d119290226bfcd464502138db4b9f1542
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4010; amd64

### `caddy:2.6-builder-windowsservercore-1809` - windows version 10.0.17763.4010; amd64

```console
$ docker pull caddy@sha256:698c8dda106fb34e783e5030fd3ea5166df618f08c2a01204a7a82aabf6b20c9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2148348831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cee813843af987f6985470a05839367529db056040844b778343ebd71743f6a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 23:47:41 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Feb 2023 23:47:42 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Feb 2023 23:47:43 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Feb 2023 23:47:44 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Feb 2023 23:50:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Feb 2023 23:50:19 GMT
ENV GOPATH=C:\go
# Wed, 15 Feb 2023 23:51:42 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Feb 2023 00:11:44 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 16 Feb 2023 00:17:12 GMT
RUN $url = 'https://dl.google.com/go/go1.19.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '8d84af29e46c38b1eec77f9310310517c9e394ac7489e1c7329a94b443b0388d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Feb 2023 00:17:13 GMT
WORKDIR C:\go
# Thu, 16 Feb 2023 02:48:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:48:16 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Feb 2023 02:48:17 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:48:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Feb 2023 02:49:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Feb 2023 02:49:37 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03ac75ee62e05ad7b8b8f97fb78a769177c49d210eedcf0a93035e9a07d0ff2`  
		Last Modified: Thu, 16 Feb 2023 00:28:24 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4beb360c9024340aa5072ce67eab6b3cb005293938525c4f3b77c3bb03f9f501`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5051ce7a895da09ac63e7ca01ef4e30434d833dbd271107d6f96375f291752ad`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea419e1594fbbef3584b4731c356499c7b8a5616af16968e6fd693eccd92012b`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb97c6a047d2cfcb6f0ef6846e78c4d5f60212639a9d1892e2af05033c217df`  
		Last Modified: Thu, 16 Feb 2023 00:28:30 GMT  
		Size: 25.6 MB (25606151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941d25224d4bab25ba0b2304a5811b0fc2970ba6385afdbefbfec898720c3beb`  
		Last Modified: Thu, 16 Feb 2023 00:28:17 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa161895f771062e6d8e8aa2e0e44c15c5affdacc8d409f6e70f1fa743a9bb1`  
		Last Modified: Thu, 16 Feb 2023 00:28:17 GMT  
		Size: 335.6 KB (335550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd14ed3be87ab223f1391d40c3cdcfcee876586e89fbeed2aeccb318734a22`  
		Last Modified: Thu, 16 Feb 2023 00:32:40 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddec1d087c619cf7156e3dba04dd6a73e704d66c60e3fbc4b32c73b4401471b`  
		Last Modified: Thu, 16 Feb 2023 00:33:24 GMT  
		Size: 157.8 MB (157798436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50612066f9b2d86b5cecd95ce6897d89929be6a819c3de13dd9ecc32948832cb`  
		Last Modified: Thu, 16 Feb 2023 00:32:40 GMT  
		Size: 1.5 KB (1544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3bbcb2df900a9ead208e08eefd6faa32bbd6c5a189212d97b94eec1e5807a24`  
		Last Modified: Thu, 16 Feb 2023 02:51:49 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b5e7db448c55e5e60ab1aefceb414700fb99de06cc1c047404e32031064e0c`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7af0982eb604918cfaece327a35d278b59d5f2ca440882b5e7d402e7cce80f6`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad49ef8883b47edaa38ca21b422551a4da50f675370fc1596432938cd7de4d2`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce066417e925c257e21d7126cbbdcf5316022725a7ef7a89575b86fd534d133f`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.6 MB (1632671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbe58e4b6c6b7d8f16c2682325b6df5f61050915e6af7829adab49c1914e5c9`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:573ab227ac93b402974ef9c7f039983bc070f5e08c73d21e62345c13f8ccbaab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `caddy:2.6-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1547; amd64

```console
$ docker pull caddy@sha256:21d50bd59eead7016b606e72f6dede55b7f2c718f306c823f3a34ef794622aa7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1865665598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f3a334b2d908beba62aa4ea43b950f4be8fa2261a29819fecc52e58eaadf2df`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 23:42:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Feb 2023 23:42:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Feb 2023 23:42:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Feb 2023 23:42:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Feb 2023 23:43:27 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Feb 2023 23:43:28 GMT
ENV GOPATH=C:\go
# Wed, 15 Feb 2023 23:44:03 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Feb 2023 00:07:02 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 16 Feb 2023 00:11:25 GMT
RUN $url = 'https://dl.google.com/go/go1.19.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '8d84af29e46c38b1eec77f9310310517c9e394ac7489e1c7329a94b443b0388d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Feb 2023 00:11:27 GMT
WORKDIR C:\go
# Thu, 16 Feb 2023 02:49:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:49:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Feb 2023 02:49:47 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:49:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Feb 2023 02:50:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Feb 2023 02:50:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4048a86b3278e59b840ad06b4cf5f5888ce1068d503522a95eb470d5126ed69a`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b07973952171f91c05aade363f3e6c9a2e84548f33eaa3c8e48632460e61f8`  
		Last Modified: Thu, 16 Feb 2023 00:26:45 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a95dff10905572b5f9177959a5a9f60a9364e1dd627ed52e34ec4bee3fb3069`  
		Last Modified: Thu, 16 Feb 2023 00:26:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4267caf437f5a3d92235ab7b8d55b2c812744f166725151ba701aef9d682c6e9`  
		Last Modified: Thu, 16 Feb 2023 00:26:41 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982a959ece2e33bce3f35c5c0adb01a3426c92111b309c15f8cc31200ebcf899`  
		Last Modified: Thu, 16 Feb 2023 00:26:54 GMT  
		Size: 25.9 MB (25852811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065416c07c5d80f7a085e0e84237051d7050a71103cc9d7fb6d5ef57725dc4c6`  
		Last Modified: Thu, 16 Feb 2023 00:26:39 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07015cae66c7ebb6b0adce2dfe424313b228bb703ac3e900deebe74ae961bb49`  
		Last Modified: Thu, 16 Feb 2023 00:26:40 GMT  
		Size: 571.7 KB (571672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285847798b3738c8863954b395d2e44410be1004e9f8513dd1546a0713f153d3`  
		Last Modified: Thu, 16 Feb 2023 00:31:40 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4f6797c9312e8b2093037565c19561d6152cca51a84614b32c0813526f219f`  
		Last Modified: Thu, 16 Feb 2023 00:32:31 GMT  
		Size: 158.0 MB (158008192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2bd8446758388c6c8ddb5d51dd63d25a0dbf5c8e1385928c5e64c83948d966`  
		Last Modified: Thu, 16 Feb 2023 00:31:40 GMT  
		Size: 1.6 KB (1561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd741098e5131c0452f3451d13ce2b131c36cbfcf24df5fbd2fb9e5751e85627`  
		Last Modified: Thu, 16 Feb 2023 02:52:08 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcd5d2a85aea028cd55d32ae579beb21aa5efc8eb3875d901dfcb623092327a`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f63b7e14eef097ca8f36e589d8d609a276d3196875467da71a714db6c8e583`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2e98e1ab65293643e4b2173a01d386c2129bf22ffaee5d1b730f19a26759a7`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15030494f30adf45739bdc5e411e1ae7ea0395ebcb4c2a4f74eedbc5f71d3acd`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.9 MB (1868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba874cf328299688fd26dd5261c439698422f93ce708e583e0e248444622caff`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-windowsservercore`

```console
$ docker pull caddy@sha256:07fbc5a89186611e042f7ab23685ae8afbcce5678ff9b1315e742e6935052c9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4010; amd64
	-	windows version 10.0.20348.1547; amd64

### `caddy:2.6-windowsservercore` - windows version 10.0.17763.4010; amd64

```console
$ docker pull caddy@sha256:f78e6d4fc1641b322d4e44adcada628f9acb5106b2e166cbcba796764a4db257
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1978492183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:198e4772b4788d7810819799af107998abe8e241416654ca5406331afefc2908`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:43:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:44:00 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:45:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:45:08 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:45:09 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:45:10 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:45:11 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:45:12 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:45:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:45:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:45:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:45:17 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:45:19 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:46:11 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:46:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f19b532038d3c84c40068e825815f2b252b82869809b11745d9893f12a99ac1`  
		Last Modified: Thu, 16 Feb 2023 02:51:03 GMT  
		Size: 526.3 KB (526332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15f6c8f1e7f194b2b408bf6c4330db67cf7cd4783d39acba2d8384b2f3c31d4`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab346a52e8e98a31f0970c85a32f1653b5179dd5ad781a8764b08de792a4d99`  
		Last Modified: Thu, 16 Feb 2023 02:51:05 GMT  
		Size: 14.7 MB (14677251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4451f67396ee792e3ace473ca4a69e5e49639ab8b620e489635a7b2eeb775523`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9291ccd53cd67f009cd59c77d90d2623192e5e134fc2ad5a03f1c1860ab66b80`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3096247c037e7418f5efc50ce5c7e6bc272ccac5c014f5cb085d77c4c28a3a`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f902038f4ba892bc3e1e4d5fdcef6b7759891c41c067b744fa3d5b008776c90`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82e400c4f2072b1e2b2ff49169de3108075208b544f454b3cdf016be6356321`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0944799324319439cbaf2f01dd147e8cc496ea80243ddc22e59e301237acb293`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce6c226ffeaa8146cae1b818b43a4776a06f6ce0be460b7d9b42fcc503b39db`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0b36e09fd7994e37dd27ccdcfa4610fc1219c4044a95695c6de9f9eecda63b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f284721a924468c7a0ff80b2809a222ae20cae99d35aa761b5296272783263b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bec609c0b4d99a9726ad86662d32a57664d18dde9d9087c0695ec7e9c4a47c`  
		Last Modified: Thu, 16 Feb 2023 02:50:59 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ad796550cc1ac21dd77352cf12cc78cacbd0a9f8a1e728e7e4f6a02a0cb9fb`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1955699b7dbbfef476622c70f983565943bafe8909c80ec278dff19509fad86`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4096827c6eb36146321a048a5041be746e60afe4c8e90717d681f2d271e0143`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc99e795e3855739a0c170e77263147dec07ac66a9ae51c306705be5af6574b`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8683be90a75d0e97aa8b7002c075e040e7299bd1fde397a541df3e7e4168d97`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 308.1 KB (308099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156392510131bc65057e3573b9aa9838fccd38cc8ed89734e5255bcd4a315274`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-windowsservercore` - windows version 10.0.20348.1547; amd64

```console
$ docker pull caddy@sha256:87b9acadc87fc1f78b7ee864f06462a0f45aa263af20fa1744e2f2a0d0870b02
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1695421581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaff43d5343d972f345ff5561ee131879eaafd463e389a1c2607715ac3f6e793`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:46:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:46:57 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:47:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:47:26 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:47:27 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:47:28 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:47:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:47:31 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:47:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:47:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:47:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:47:36 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:47:37 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:47:56 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:47:57 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1961fba6606566986ddd1960cf8309d19fa9deaa486f5a162a60114f3d4c3c82`  
		Last Modified: Thu, 16 Feb 2023 02:51:29 GMT  
		Size: 778.8 KB (778807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af5d76bf41697a16b3336a1857d1e530a3137f28d997c6f5eca0121d42ea88d`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d935f5b810851a2833b69e65d9dcff828f1c6686dab6fa117e9bd08eb95f5990`  
		Last Modified: Thu, 16 Feb 2023 02:51:31 GMT  
		Size: 14.9 MB (14914232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54e2a419181dd9257efde40f9ab80121dd6cc1a478f6ff42d160ddbf5e17cd4`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c07f1bbb0931b3148683baae55ab0d85f8576b2a1d8c2a59bb28544572b5a9d`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06073fd741cf5968f24574903b70213f9743b648ebec9c53ccb8fe114ce01ae`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a17243f1184726e21bf0821ee5984a84575b55befba72594fbf0b3a32a47f1`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c403099e0a283f6f2b25b4235c61c8b564a832643f33280253dc040d2a2ab07`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cc4608f06891b205fbec74e83a221161a2f9d9b50a0b548c3c716d176ee1a4`  
		Last Modified: Thu, 16 Feb 2023 02:51:25 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfe2ac143052b1fa8973567134244ce4ecd1693f16205dd53f0d4cf1b5caa5a`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e217159efeb187bf7ae9a12f6f70764141dd97837f24a517851bc15a36b552`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc05a7da758918922e168d1b07b29f4a81d398dc805724dd6b23b4cb28c7b43`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832768cea319f33011657944b08b51ea41229fdd7a37f21162dd8aedceb31a6b`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443fc82ac63aefa17f6de497731a007fbc972b175040388a8fda7112834af9fa`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39ff50a2c37b226c6e79e3789d1706fc47cb355b14372a147024fc11b2dfb2b`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c6037df6cbd4b9e046dded7157e841a1c40659c4dd082ff9d397c95be6e411`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a470cfe53e2d01e3ca43a7211eb050493a97f430e3c5a52e2364f54a0a4e4834`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d12a1c4350235354af8011d0b2eccb56884eea72a0475197fb007c4fa6c111`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 359.9 KB (359894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea80c894fe52045adaa4c44b9f66422259571c7aec153753d27a56aa3ccbd930`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-windowsservercore-1809`

```console
$ docker pull caddy@sha256:1bd6dc9cf41fc94696e73caafb13f1e2aa4080c4961ffe195303c2a51811ff9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4010; amd64

### `caddy:2.6-windowsservercore-1809` - windows version 10.0.17763.4010; amd64

```console
$ docker pull caddy@sha256:f78e6d4fc1641b322d4e44adcada628f9acb5106b2e166cbcba796764a4db257
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1978492183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:198e4772b4788d7810819799af107998abe8e241416654ca5406331afefc2908`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:43:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:44:00 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:45:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:45:08 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:45:09 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:45:10 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:45:11 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:45:12 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:45:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:45:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:45:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:45:17 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:45:19 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:46:11 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:46:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f19b532038d3c84c40068e825815f2b252b82869809b11745d9893f12a99ac1`  
		Last Modified: Thu, 16 Feb 2023 02:51:03 GMT  
		Size: 526.3 KB (526332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15f6c8f1e7f194b2b408bf6c4330db67cf7cd4783d39acba2d8384b2f3c31d4`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab346a52e8e98a31f0970c85a32f1653b5179dd5ad781a8764b08de792a4d99`  
		Last Modified: Thu, 16 Feb 2023 02:51:05 GMT  
		Size: 14.7 MB (14677251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4451f67396ee792e3ace473ca4a69e5e49639ab8b620e489635a7b2eeb775523`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9291ccd53cd67f009cd59c77d90d2623192e5e134fc2ad5a03f1c1860ab66b80`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3096247c037e7418f5efc50ce5c7e6bc272ccac5c014f5cb085d77c4c28a3a`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f902038f4ba892bc3e1e4d5fdcef6b7759891c41c067b744fa3d5b008776c90`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82e400c4f2072b1e2b2ff49169de3108075208b544f454b3cdf016be6356321`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0944799324319439cbaf2f01dd147e8cc496ea80243ddc22e59e301237acb293`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce6c226ffeaa8146cae1b818b43a4776a06f6ce0be460b7d9b42fcc503b39db`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0b36e09fd7994e37dd27ccdcfa4610fc1219c4044a95695c6de9f9eecda63b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f284721a924468c7a0ff80b2809a222ae20cae99d35aa761b5296272783263b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bec609c0b4d99a9726ad86662d32a57664d18dde9d9087c0695ec7e9c4a47c`  
		Last Modified: Thu, 16 Feb 2023 02:50:59 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ad796550cc1ac21dd77352cf12cc78cacbd0a9f8a1e728e7e4f6a02a0cb9fb`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1955699b7dbbfef476622c70f983565943bafe8909c80ec278dff19509fad86`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4096827c6eb36146321a048a5041be746e60afe4c8e90717d681f2d271e0143`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc99e795e3855739a0c170e77263147dec07ac66a9ae51c306705be5af6574b`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8683be90a75d0e97aa8b7002c075e040e7299bd1fde397a541df3e7e4168d97`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 308.1 KB (308099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156392510131bc65057e3573b9aa9838fccd38cc8ed89734e5255bcd4a315274`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:bdada4aecbae3dbf7c909817361c5c5e025530a60f1017107cf4cbe628e5a12b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `caddy:2.6-windowsservercore-ltsc2022` - windows version 10.0.20348.1547; amd64

```console
$ docker pull caddy@sha256:87b9acadc87fc1f78b7ee864f06462a0f45aa263af20fa1744e2f2a0d0870b02
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1695421581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaff43d5343d972f345ff5561ee131879eaafd463e389a1c2607715ac3f6e793`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:46:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:46:57 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:47:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:47:26 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:47:27 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:47:28 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:47:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:47:31 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:47:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:47:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:47:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:47:36 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:47:37 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:47:56 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:47:57 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1961fba6606566986ddd1960cf8309d19fa9deaa486f5a162a60114f3d4c3c82`  
		Last Modified: Thu, 16 Feb 2023 02:51:29 GMT  
		Size: 778.8 KB (778807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af5d76bf41697a16b3336a1857d1e530a3137f28d997c6f5eca0121d42ea88d`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d935f5b810851a2833b69e65d9dcff828f1c6686dab6fa117e9bd08eb95f5990`  
		Last Modified: Thu, 16 Feb 2023 02:51:31 GMT  
		Size: 14.9 MB (14914232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54e2a419181dd9257efde40f9ab80121dd6cc1a478f6ff42d160ddbf5e17cd4`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c07f1bbb0931b3148683baae55ab0d85f8576b2a1d8c2a59bb28544572b5a9d`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06073fd741cf5968f24574903b70213f9743b648ebec9c53ccb8fe114ce01ae`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a17243f1184726e21bf0821ee5984a84575b55befba72594fbf0b3a32a47f1`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c403099e0a283f6f2b25b4235c61c8b564a832643f33280253dc040d2a2ab07`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cc4608f06891b205fbec74e83a221161a2f9d9b50a0b548c3c716d176ee1a4`  
		Last Modified: Thu, 16 Feb 2023 02:51:25 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfe2ac143052b1fa8973567134244ce4ecd1693f16205dd53f0d4cf1b5caa5a`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e217159efeb187bf7ae9a12f6f70764141dd97837f24a517851bc15a36b552`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc05a7da758918922e168d1b07b29f4a81d398dc805724dd6b23b4cb28c7b43`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832768cea319f33011657944b08b51ea41229fdd7a37f21162dd8aedceb31a6b`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443fc82ac63aefa17f6de497731a007fbc972b175040388a8fda7112834af9fa`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39ff50a2c37b226c6e79e3789d1706fc47cb355b14372a147024fc11b2dfb2b`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c6037df6cbd4b9e046dded7157e841a1c40659c4dd082ff9d397c95be6e411`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a470cfe53e2d01e3ca43a7211eb050493a97f430e3c5a52e2364f54a0a4e4834`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d12a1c4350235354af8011d0b2eccb56884eea72a0475197fb007c4fa6c111`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 359.9 KB (359894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea80c894fe52045adaa4c44b9f66422259571c7aec153753d27a56aa3ccbd930`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4`

```console
$ docker pull caddy@sha256:304185ec40295c7b7c33f98981c241d23d959fa0534eb34cd18c732fde51cd5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4010; amd64
	-	windows version 10.0.20348.1547; amd64

### `caddy:2.6.4` - linux; amd64

```console
$ docker pull caddy@sha256:36ba71b44afa613ecf0aadce8e4b9e3f56e0c4b0a78c8edf4e8c2485f21b35ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17449113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8464e23f16f9a82426bbdc3ac8c94270a84453ddc86b9147505a2378a7c2fd0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:38:34 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 11 Feb 2023 07:38:36 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:19:21 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:19:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:19:23 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:19:24 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:19:25 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e3e797818bc929d95bae8220b7b6034b559c217ef5bf622dc7fedc8d270a48`  
		Last Modified: Sat, 11 Feb 2023 07:39:01 GMT  
		Size: 351.2 KB (351178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cebb4c80b3906a9b751ee9a512c1581331b1fd691c84f575c01a29e28403dde`  
		Last Modified: Sat, 11 Feb 2023 07:39:00 GMT  
		Size: 7.6 KB (7552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90648ba22c191b969d8db393bf6138e7d6ecc1b70b3865d1717ec4d663192d89`  
		Last Modified: Wed, 15 Feb 2023 19:19:52 GMT  
		Size: 14.3 MB (14282621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4` - linux; arm variant v6

```console
$ docker pull caddy@sha256:db317e683b30c11665349301255c3c59f3f5b085d4e075553e445129981ad5e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16582515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4628532cad0308b1d01506925ca941dffeb3bdd058cd79ccd7f055dce243e3b6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:32 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Fri, 10 Feb 2023 20:49:32 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 00:17:32 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 08 Mar 2023 00:17:34 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 08 Mar 2023 00:17:34 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:17:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 08 Mar 2023 00:17:38 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 08 Mar 2023 00:17:39 GMT
ENV XDG_DATA_HOME=/data
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 08 Mar 2023 00:17:41 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 80
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 443
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 443/udp
# Wed, 08 Mar 2023 00:17:42 GMT
EXPOSE 2019
# Wed, 08 Mar 2023 00:17:42 GMT
WORKDIR /srv
# Wed, 08 Mar 2023 00:17:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e676ebf894f684676e3a3c92294bbc14ba7061c7d24285909e673075903c39a9`  
		Last Modified: Wed, 08 Mar 2023 00:18:32 GMT  
		Size: 345.9 KB (345903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b146a16f288a28f362ad572b56958616fb5f4e0572bbe406ce18868be0d5c3`  
		Last Modified: Wed, 08 Mar 2023 00:18:31 GMT  
		Size: 7.6 KB (7559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e662de32a44a67eae886e653355902b11fec7407264122f1e72b5c460cb4334`  
		Last Modified: Wed, 08 Mar 2023 00:18:34 GMT  
		Size: 13.6 MB (13612275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4` - linux; arm variant v7

```console
$ docker pull caddy@sha256:03b5f2d631567d2783e8977e4988bdc75f13acb5c5b7bb18f3984045fb557b11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16365710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bed848976d2f2ce06398c52bf359363302bd512c4c51f08acb50cdd7ec0db5a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 10:40:15 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 02 Mar 2023 10:40:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 02 Mar 2023 10:40:16 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 02 Mar 2023 10:40:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 02 Mar 2023 10:40:19 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 02 Mar 2023 10:40:19 GMT
ENV XDG_DATA_HOME=/data
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 02 Mar 2023 10:40:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 02 Mar 2023 10:40:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 80
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 443
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 443/udp
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 2019
# Thu, 02 Mar 2023 10:40:20 GMT
WORKDIR /srv
# Thu, 02 Mar 2023 10:40:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769efc94ebb1351d7f88e191e0e5c768fc2462e89d73fa4b373005e8a912f367`  
		Last Modified: Thu, 02 Mar 2023 10:41:04 GMT  
		Size: 342.7 KB (342688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fb7d44b5e1d66fb60d8593e306cfef844841aca960cacb7258951888fcf79e`  
		Last Modified: Thu, 02 Mar 2023 10:41:04 GMT  
		Size: 7.6 KB (7560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818d68e9d461fbb298a8bb8f5467049d89e77e6324f72842c3d45e5af3d0767b`  
		Last Modified: Thu, 02 Mar 2023 10:41:06 GMT  
		Size: 13.6 MB (13594968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6c2623f6bf30798be5c37fc7484e45ecc288d493fb657883f59ddb27ed714ad8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16130997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a38afdc517ef4cff6b6b51a1c6a633c2826599b07feb1e88380d0f783e35cf1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:00:35 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:00:37 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 18:39:20 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 18:39:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 18:39:22 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 18:39:22 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 80
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 443
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 18:39:23 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 18:39:23 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70730e8e2fb933ec157ec87f2a4fb4ad45e8e578b8f7c76cc4846631d773554`  
		Last Modified: Fri, 10 Feb 2023 22:01:02 GMT  
		Size: 350.2 KB (350153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a4b7390d269477c225f1d03e825d2d8bdf6b4d87b5f7bb8811b341e56b7d36`  
		Last Modified: Fri, 10 Feb 2023 22:01:02 GMT  
		Size: 7.6 KB (7555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2743d2ef53ee6edb0e39c89bf16957e3a00990410b2d1a126dca1b2d196182`  
		Last Modified: Wed, 15 Feb 2023 18:39:53 GMT  
		Size: 13.1 MB (13063787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4` - linux; ppc64le

```console
$ docker pull caddy@sha256:8861ab3ae3d0c180e38142c2f7482f9ce1773419eb29ed9d6d18308246858093
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5819f0ab4928a30c29293a27299a3b44371cd3bd97df91432ef7b3f43b692d8c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:13:21 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:13:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:16:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:16:41 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:16:42 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:16:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:16:47 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:16:47 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:16:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bd0321e6539bb7dac8574fd36bad22059ef06bb63dc842165f69d0a821572`  
		Last Modified: Fri, 10 Feb 2023 22:14:16 GMT  
		Size: 363.1 KB (363088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb806b2600b0209a73fc7175ab778d0224661034b2f722bd1a0aec1eb9eabe3d`  
		Last Modified: Fri, 10 Feb 2023 22:14:15 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd7c8ae860931dd79dea76d33bc21bb11d89cd4d133cdb41078b040afc6633e`  
		Last Modified: Wed, 15 Feb 2023 19:17:41 GMT  
		Size: 12.8 MB (12779898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4` - linux; s390x

```console
$ docker pull caddy@sha256:4e1ed99f133abf02d6a7c77849978bb621f748e18c9cb9f7a1dbf88480ddb8d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45cd164da734310b788dcbd4f6c94bccff6e48705fe4d42ecca07a54e9459a9c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:31 GMT
ADD file:17af250b49631cf2acf655c85df90977eddab4c9afd67bda3c577db5200364f1 in / 
# Fri, 10 Feb 2023 21:41:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:14:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:14:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 18:41:48 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 18:41:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 18:41:59 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 18:41:59 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 18:42:00 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 18:42:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 18:42:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 18:42:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 18:42:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 18:42:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 18:42:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 18:42:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 18:42:05 GMT
EXPOSE 80
# Wed, 15 Feb 2023 18:42:06 GMT
EXPOSE 443
# Wed, 15 Feb 2023 18:42:07 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 18:42:07 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 18:42:08 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 18:42:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:667d93a24f321610e24486f3148545191f113ab9ab2444804087dd65ebbda9ed`  
		Last Modified: Fri, 10 Feb 2023 21:42:26 GMT  
		Size: 2.6 MB (2593581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e6ec82400496ce74e37120e1655955b79303daaa5b8ca7e956e3cd96ddd6e9`  
		Last Modified: Fri, 10 Feb 2023 22:15:05 GMT  
		Size: 352.8 KB (352801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5b992687f93ced3715ad97bd95ab37daef5685b784e195209caefbc48f14e9`  
		Last Modified: Fri, 10 Feb 2023 22:15:05 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ccc40924ce2df3343fa5465a92ccaa4ed80e0883190a99d3f468c60f9ddbcf8`  
		Last Modified: Wed, 15 Feb 2023 18:43:19 GMT  
		Size: 13.8 MB (13838817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4` - windows version 10.0.17763.4010; amd64

```console
$ docker pull caddy@sha256:f78e6d4fc1641b322d4e44adcada628f9acb5106b2e166cbcba796764a4db257
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1978492183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:198e4772b4788d7810819799af107998abe8e241416654ca5406331afefc2908`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:43:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:44:00 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:45:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:45:08 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:45:09 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:45:10 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:45:11 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:45:12 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:45:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:45:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:45:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:45:17 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:45:19 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:46:11 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:46:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f19b532038d3c84c40068e825815f2b252b82869809b11745d9893f12a99ac1`  
		Last Modified: Thu, 16 Feb 2023 02:51:03 GMT  
		Size: 526.3 KB (526332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15f6c8f1e7f194b2b408bf6c4330db67cf7cd4783d39acba2d8384b2f3c31d4`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab346a52e8e98a31f0970c85a32f1653b5179dd5ad781a8764b08de792a4d99`  
		Last Modified: Thu, 16 Feb 2023 02:51:05 GMT  
		Size: 14.7 MB (14677251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4451f67396ee792e3ace473ca4a69e5e49639ab8b620e489635a7b2eeb775523`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9291ccd53cd67f009cd59c77d90d2623192e5e134fc2ad5a03f1c1860ab66b80`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3096247c037e7418f5efc50ce5c7e6bc272ccac5c014f5cb085d77c4c28a3a`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f902038f4ba892bc3e1e4d5fdcef6b7759891c41c067b744fa3d5b008776c90`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82e400c4f2072b1e2b2ff49169de3108075208b544f454b3cdf016be6356321`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0944799324319439cbaf2f01dd147e8cc496ea80243ddc22e59e301237acb293`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce6c226ffeaa8146cae1b818b43a4776a06f6ce0be460b7d9b42fcc503b39db`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0b36e09fd7994e37dd27ccdcfa4610fc1219c4044a95695c6de9f9eecda63b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f284721a924468c7a0ff80b2809a222ae20cae99d35aa761b5296272783263b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bec609c0b4d99a9726ad86662d32a57664d18dde9d9087c0695ec7e9c4a47c`  
		Last Modified: Thu, 16 Feb 2023 02:50:59 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ad796550cc1ac21dd77352cf12cc78cacbd0a9f8a1e728e7e4f6a02a0cb9fb`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1955699b7dbbfef476622c70f983565943bafe8909c80ec278dff19509fad86`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4096827c6eb36146321a048a5041be746e60afe4c8e90717d681f2d271e0143`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc99e795e3855739a0c170e77263147dec07ac66a9ae51c306705be5af6574b`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8683be90a75d0e97aa8b7002c075e040e7299bd1fde397a541df3e7e4168d97`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 308.1 KB (308099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156392510131bc65057e3573b9aa9838fccd38cc8ed89734e5255bcd4a315274`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4` - windows version 10.0.20348.1547; amd64

```console
$ docker pull caddy@sha256:87b9acadc87fc1f78b7ee864f06462a0f45aa263af20fa1744e2f2a0d0870b02
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1695421581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaff43d5343d972f345ff5561ee131879eaafd463e389a1c2607715ac3f6e793`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:46:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:46:57 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:47:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:47:26 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:47:27 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:47:28 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:47:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:47:31 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:47:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:47:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:47:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:47:36 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:47:37 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:47:56 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:47:57 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1961fba6606566986ddd1960cf8309d19fa9deaa486f5a162a60114f3d4c3c82`  
		Last Modified: Thu, 16 Feb 2023 02:51:29 GMT  
		Size: 778.8 KB (778807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af5d76bf41697a16b3336a1857d1e530a3137f28d997c6f5eca0121d42ea88d`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d935f5b810851a2833b69e65d9dcff828f1c6686dab6fa117e9bd08eb95f5990`  
		Last Modified: Thu, 16 Feb 2023 02:51:31 GMT  
		Size: 14.9 MB (14914232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54e2a419181dd9257efde40f9ab80121dd6cc1a478f6ff42d160ddbf5e17cd4`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c07f1bbb0931b3148683baae55ab0d85f8576b2a1d8c2a59bb28544572b5a9d`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06073fd741cf5968f24574903b70213f9743b648ebec9c53ccb8fe114ce01ae`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a17243f1184726e21bf0821ee5984a84575b55befba72594fbf0b3a32a47f1`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c403099e0a283f6f2b25b4235c61c8b564a832643f33280253dc040d2a2ab07`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cc4608f06891b205fbec74e83a221161a2f9d9b50a0b548c3c716d176ee1a4`  
		Last Modified: Thu, 16 Feb 2023 02:51:25 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfe2ac143052b1fa8973567134244ce4ecd1693f16205dd53f0d4cf1b5caa5a`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e217159efeb187bf7ae9a12f6f70764141dd97837f24a517851bc15a36b552`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc05a7da758918922e168d1b07b29f4a81d398dc805724dd6b23b4cb28c7b43`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832768cea319f33011657944b08b51ea41229fdd7a37f21162dd8aedceb31a6b`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443fc82ac63aefa17f6de497731a007fbc972b175040388a8fda7112834af9fa`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39ff50a2c37b226c6e79e3789d1706fc47cb355b14372a147024fc11b2dfb2b`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c6037df6cbd4b9e046dded7157e841a1c40659c4dd082ff9d397c95be6e411`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a470cfe53e2d01e3ca43a7211eb050493a97f430e3c5a52e2364f54a0a4e4834`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d12a1c4350235354af8011d0b2eccb56884eea72a0475197fb007c4fa6c111`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 359.9 KB (359894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea80c894fe52045adaa4c44b9f66422259571c7aec153753d27a56aa3ccbd930`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-alpine`

```console
$ docker pull caddy@sha256:3f4414616d9141c4fbd9f66641d9b91a3b67833dd4145738c536dee584db5314
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.6.4-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:36ba71b44afa613ecf0aadce8e4b9e3f56e0c4b0a78c8edf4e8c2485f21b35ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17449113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8464e23f16f9a82426bbdc3ac8c94270a84453ddc86b9147505a2378a7c2fd0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:38:34 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 11 Feb 2023 07:38:36 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:19:21 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:19:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:19:23 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:19:24 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:19:25 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e3e797818bc929d95bae8220b7b6034b559c217ef5bf622dc7fedc8d270a48`  
		Last Modified: Sat, 11 Feb 2023 07:39:01 GMT  
		Size: 351.2 KB (351178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cebb4c80b3906a9b751ee9a512c1581331b1fd691c84f575c01a29e28403dde`  
		Last Modified: Sat, 11 Feb 2023 07:39:00 GMT  
		Size: 7.6 KB (7552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90648ba22c191b969d8db393bf6138e7d6ecc1b70b3865d1717ec4d663192d89`  
		Last Modified: Wed, 15 Feb 2023 19:19:52 GMT  
		Size: 14.3 MB (14282621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:db317e683b30c11665349301255c3c59f3f5b085d4e075553e445129981ad5e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16582515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4628532cad0308b1d01506925ca941dffeb3bdd058cd79ccd7f055dce243e3b6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:32 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Fri, 10 Feb 2023 20:49:32 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 00:17:32 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 08 Mar 2023 00:17:34 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 08 Mar 2023 00:17:34 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:17:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 08 Mar 2023 00:17:38 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 08 Mar 2023 00:17:39 GMT
ENV XDG_DATA_HOME=/data
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 08 Mar 2023 00:17:41 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 80
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 443
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 443/udp
# Wed, 08 Mar 2023 00:17:42 GMT
EXPOSE 2019
# Wed, 08 Mar 2023 00:17:42 GMT
WORKDIR /srv
# Wed, 08 Mar 2023 00:17:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e676ebf894f684676e3a3c92294bbc14ba7061c7d24285909e673075903c39a9`  
		Last Modified: Wed, 08 Mar 2023 00:18:32 GMT  
		Size: 345.9 KB (345903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b146a16f288a28f362ad572b56958616fb5f4e0572bbe406ce18868be0d5c3`  
		Last Modified: Wed, 08 Mar 2023 00:18:31 GMT  
		Size: 7.6 KB (7559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e662de32a44a67eae886e653355902b11fec7407264122f1e72b5c460cb4334`  
		Last Modified: Wed, 08 Mar 2023 00:18:34 GMT  
		Size: 13.6 MB (13612275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:03b5f2d631567d2783e8977e4988bdc75f13acb5c5b7bb18f3984045fb557b11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16365710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bed848976d2f2ce06398c52bf359363302bd512c4c51f08acb50cdd7ec0db5a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 10:40:15 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 02 Mar 2023 10:40:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 02 Mar 2023 10:40:16 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 02 Mar 2023 10:40:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 02 Mar 2023 10:40:19 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 02 Mar 2023 10:40:19 GMT
ENV XDG_DATA_HOME=/data
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 02 Mar 2023 10:40:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 02 Mar 2023 10:40:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 80
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 443
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 443/udp
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 2019
# Thu, 02 Mar 2023 10:40:20 GMT
WORKDIR /srv
# Thu, 02 Mar 2023 10:40:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769efc94ebb1351d7f88e191e0e5c768fc2462e89d73fa4b373005e8a912f367`  
		Last Modified: Thu, 02 Mar 2023 10:41:04 GMT  
		Size: 342.7 KB (342688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fb7d44b5e1d66fb60d8593e306cfef844841aca960cacb7258951888fcf79e`  
		Last Modified: Thu, 02 Mar 2023 10:41:04 GMT  
		Size: 7.6 KB (7560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818d68e9d461fbb298a8bb8f5467049d89e77e6324f72842c3d45e5af3d0767b`  
		Last Modified: Thu, 02 Mar 2023 10:41:06 GMT  
		Size: 13.6 MB (13594968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6c2623f6bf30798be5c37fc7484e45ecc288d493fb657883f59ddb27ed714ad8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16130997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a38afdc517ef4cff6b6b51a1c6a633c2826599b07feb1e88380d0f783e35cf1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:00:35 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:00:37 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 18:39:20 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 18:39:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 18:39:22 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 18:39:22 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 80
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 443
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 18:39:23 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 18:39:23 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70730e8e2fb933ec157ec87f2a4fb4ad45e8e578b8f7c76cc4846631d773554`  
		Last Modified: Fri, 10 Feb 2023 22:01:02 GMT  
		Size: 350.2 KB (350153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a4b7390d269477c225f1d03e825d2d8bdf6b4d87b5f7bb8811b341e56b7d36`  
		Last Modified: Fri, 10 Feb 2023 22:01:02 GMT  
		Size: 7.6 KB (7555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2743d2ef53ee6edb0e39c89bf16957e3a00990410b2d1a126dca1b2d196182`  
		Last Modified: Wed, 15 Feb 2023 18:39:53 GMT  
		Size: 13.1 MB (13063787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:8861ab3ae3d0c180e38142c2f7482f9ce1773419eb29ed9d6d18308246858093
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5819f0ab4928a30c29293a27299a3b44371cd3bd97df91432ef7b3f43b692d8c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:13:21 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:13:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:16:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:16:41 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:16:42 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:16:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:16:47 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:16:47 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:16:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bd0321e6539bb7dac8574fd36bad22059ef06bb63dc842165f69d0a821572`  
		Last Modified: Fri, 10 Feb 2023 22:14:16 GMT  
		Size: 363.1 KB (363088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb806b2600b0209a73fc7175ab778d0224661034b2f722bd1a0aec1eb9eabe3d`  
		Last Modified: Fri, 10 Feb 2023 22:14:15 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd7c8ae860931dd79dea76d33bc21bb11d89cd4d133cdb41078b040afc6633e`  
		Last Modified: Wed, 15 Feb 2023 19:17:41 GMT  
		Size: 12.8 MB (12779898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:4e1ed99f133abf02d6a7c77849978bb621f748e18c9cb9f7a1dbf88480ddb8d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45cd164da734310b788dcbd4f6c94bccff6e48705fe4d42ecca07a54e9459a9c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:31 GMT
ADD file:17af250b49631cf2acf655c85df90977eddab4c9afd67bda3c577db5200364f1 in / 
# Fri, 10 Feb 2023 21:41:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:14:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:14:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 18:41:48 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 18:41:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 18:41:59 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 18:41:59 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 18:42:00 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 18:42:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 18:42:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 18:42:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 18:42:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 18:42:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 18:42:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 18:42:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 18:42:05 GMT
EXPOSE 80
# Wed, 15 Feb 2023 18:42:06 GMT
EXPOSE 443
# Wed, 15 Feb 2023 18:42:07 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 18:42:07 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 18:42:08 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 18:42:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:667d93a24f321610e24486f3148545191f113ab9ab2444804087dd65ebbda9ed`  
		Last Modified: Fri, 10 Feb 2023 21:42:26 GMT  
		Size: 2.6 MB (2593581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e6ec82400496ce74e37120e1655955b79303daaa5b8ca7e956e3cd96ddd6e9`  
		Last Modified: Fri, 10 Feb 2023 22:15:05 GMT  
		Size: 352.8 KB (352801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5b992687f93ced3715ad97bd95ab37daef5685b784e195209caefbc48f14e9`  
		Last Modified: Fri, 10 Feb 2023 22:15:05 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ccc40924ce2df3343fa5465a92ccaa4ed80e0883190a99d3f468c60f9ddbcf8`  
		Last Modified: Wed, 15 Feb 2023 18:43:19 GMT  
		Size: 13.8 MB (13838817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-builder`

```console
$ docker pull caddy@sha256:8fe3549f0a6c0db646ec94d25f0c2a87ea055f50cb73477405df8f6fd2349784
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4010; amd64
	-	windows version 10.0.20348.1547; amd64

### `caddy:2.6.4-builder` - linux; amd64

```console
$ docker pull caddy@sha256:47722ffc694507be1e2f34ca172e292fb5e226ea68d87871300b9d65f543fcce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131421587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4674ac67a52f4d29bc8349e9dcca7db8393d778c97c79d9e2f6e997603a99cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 08:21:54 GMT
RUN apk add --no-cache ca-certificates
# Sat, 11 Feb 2023 08:21:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:24:10 GMT
ENV GOLANG_VERSION=1.19.6
# Tue, 14 Feb 2023 19:25:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 14 Feb 2023 19:25:43 GMT
ENV GOPATH=/go
# Tue, 14 Feb 2023 19:25:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:25:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Feb 2023 19:25:44 GMT
WORKDIR /go
# Tue, 14 Feb 2023 19:47:10 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 14 Feb 2023 19:47:10 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 15 Feb 2023 19:19:27 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:19:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 15 Feb 2023 19:19:28 GMT
ENV XCADDY_SETCAP=1
# Wed, 15 Feb 2023 19:19:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 15 Feb 2023 19:19:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 15 Feb 2023 19:19:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d21d5440ebff5aaaaeb115a003f7a4a3897f1866a87de95bc4a21436fc563c`  
		Last Modified: Sat, 11 Feb 2023 08:29:10 GMT  
		Size: 284.8 KB (284816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f790f4c5274f100158d4c23bc5eddf659c1fe93ef4025488f9493d88f1490d88`  
		Last Modified: Tue, 14 Feb 2023 19:31:12 GMT  
		Size: 122.4 MB (122355677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bf170fd9e6726c86c0d4b478d9ec522e82c527a8e708668f48233a4d03f618`  
		Last Modified: Tue, 14 Feb 2023 19:30:55 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a5d1c1b6ed103f8c7f97c73ed546ff7e767b10473b55c15c0d4e1a13a69481`  
		Last Modified: Tue, 14 Feb 2023 19:47:34 GMT  
		Size: 4.2 MB (4188243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0130eaa2f0b1f7646719d82927743bd84c83ed450eb8be4db5327d280d5e4d0`  
		Last Modified: Wed, 15 Feb 2023 19:20:05 GMT  
		Size: 1.2 MB (1217841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab1f57409241476a86d26944527bc2c6c3903eadb21221b8d96da52120b3109`  
		Last Modified: Wed, 15 Feb 2023 19:20:05 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e2b8479c011649b6d47ead7051ebf36d10e2c764f2bc3bc507eab00a1812b6a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127455561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7351cc9a113eeb1deb8afa4c19e381df6b5e03cfef4e63e47bfe99f0b43d95ab`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:28 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Fri, 10 Feb 2023 20:49:28 GMT
CMD ["/bin/sh"]
# Tue, 07 Mar 2023 23:49:29 GMT
RUN apk add --no-cache ca-certificates
# Tue, 07 Mar 2023 23:49:29 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:53:43 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:55:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:55:31 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:55:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:55:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:55:32 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:17:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:17:50 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:17:50 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:17:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:17:51 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:17:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:17:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:17:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06dc45fa3a2f6e0270fe56d6b9f8efada3c9b5854707b52fe42dd55844fb1d5`  
		Last Modified: Tue, 07 Mar 2023 23:58:16 GMT  
		Size: 286.2 KB (286214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9c435c140baf308bcd21b10be4fe27e2cec5ec2acccb0cba35e7ec207d54ae`  
		Last Modified: Tue, 07 Mar 2023 23:59:54 GMT  
		Size: 118.7 MB (118731518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f756f642eb6722bcddfd36a868987c31f5583a7bac2ccf573f8c4fc55198ad49`  
		Last Modified: Tue, 07 Mar 2023 23:59:33 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c49be1b95c6f947e8aaed6708b2c0b38ea78e63b117ac389af00cca5f95334f`  
		Last Modified: Wed, 08 Mar 2023 00:18:51 GMT  
		Size: 4.2 MB (4160310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1cd39813132ad141affe91c6d7f78654e7dbe1e8454baf43e2ee60f2480ecd`  
		Last Modified: Wed, 08 Mar 2023 00:18:51 GMT  
		Size: 1.2 MB (1166071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6624093c59eca00c1b574cd2672bb86cf72a602c484c89dd864ab09d28d875b`  
		Last Modified: Wed, 08 Mar 2023 00:18:50 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:35dc985cc319ba4cd38b0f28d82ec4af14971a9336ce7870444c023c1415fa7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126524974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:822857d40d7e456ebf6b4405bd126f6499dd89ce092e55728fa8deaea4601da8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 02:15:04 GMT
RUN apk add --no-cache ca-certificates
# Thu, 02 Mar 2023 02:15:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 02:19:52 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 02 Mar 2023 02:21:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 02 Mar 2023 02:21:35 GMT
ENV GOPATH=/go
# Thu, 02 Mar 2023 02:21:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 02:21:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 02 Mar 2023 02:21:35 GMT
WORKDIR /go
# Thu, 02 Mar 2023 10:40:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 02 Mar 2023 10:40:26 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_SETCAP=1
# Thu, 02 Mar 2023 10:40:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 02 Mar 2023 10:40:28 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 02 Mar 2023 10:40:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4962ca8504034f69427a90f2b07cfde1e4c20297e4507d5620bb7ea27e646919`  
		Last Modified: Thu, 02 Mar 2023 02:26:02 GMT  
		Size: 285.4 KB (285445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20059bad54d9966d7995685d0c72ce1566c6370b4105df472360f5d2c8ecd21`  
		Last Modified: Thu, 02 Mar 2023 02:28:31 GMT  
		Size: 118.5 MB (118477876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4d49a4d60a68cc1326493b7f8b4cf548d4cec1694b7ccb266f06e4028b501d`  
		Last Modified: Thu, 02 Mar 2023 02:28:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0098f26d1429a39f7d8f6dd18417972d79d6706e530dbfbc4cf9991ff98f3c6`  
		Last Modified: Thu, 02 Mar 2023 10:41:22 GMT  
		Size: 3.7 MB (3729269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0aafe51cc793a860e8c2f2c4799c11f9bebe521643a6f6578f348ce06ae80d`  
		Last Modified: Thu, 02 Mar 2023 10:41:22 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24f3750a2b57fead59e3d812fa66ae7c79703a8a84d41670403b9dc7c23eb90`  
		Last Modified: Thu, 02 Mar 2023 10:41:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6e43472efedad7b414f4cce21a50e04578ea8527ad05ee901ba9eabc88d7718e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125849779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62beb7ef29ce475cb1f571275d3c9ac33185ec48844366ef16a99e8540239b2b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:38:33 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:38:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:43:17 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:44:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:44:26 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:44:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:44:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:44:27 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:06:06 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:06:06 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:06:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:06:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:06:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55522c79112429742fe76c795b9509c5cd1e8198e0caa2a1e355c0e60a719576`  
		Last Modified: Fri, 10 Feb 2023 22:44:19 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1815dcbf43e87e122cc76a24663b7c0d6e01ad03c3be30a7dc13c1bf941c595`  
		Last Modified: Tue, 07 Mar 2023 23:49:19 GMT  
		Size: 116.9 MB (116933985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5aad4e0c6f77e535fe5a51a211a4691a5002a111c52fa17708cf1bc7c01879`  
		Last Modified: Tue, 07 Mar 2023 23:49:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557acb83c53566587727172247e84b25f860b606c200b1fc863eafc75d6b0cf4`  
		Last Modified: Wed, 08 Mar 2023 00:06:29 GMT  
		Size: 4.2 MB (4243285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb71700cd911a18f7eb1f75d651639bc79bda4000e2f4e6a8afe570b03816eb`  
		Last Modified: Wed, 08 Mar 2023 00:06:29 GMT  
		Size: 1.1 MB (1123733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358517d9544ce3184d74860b7f2054339481407b928bb11ccbf7d35163006788`  
		Last Modified: Wed, 08 Mar 2023 00:06:28 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:8126a0d2b7cc9613f70b6b5375c14cc61dfca5dc1b83adc5be33efab8eacc69f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126579575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2da1cd24f35f4106a8a7176a2f2b5656a22982a1787b9204d3eaab9ec535ef58`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:40:13 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:40:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:46:09 GMT
ENV GOLANG_VERSION=1.19.6
# Tue, 14 Feb 2023 19:48:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 14 Feb 2023 19:48:44 GMT
ENV GOPATH=/go
# Tue, 14 Feb 2023 19:48:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:48:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Feb 2023 19:48:46 GMT
WORKDIR /go
# Tue, 14 Feb 2023 20:12:48 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 14 Feb 2023 20:12:48 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 15 Feb 2023 19:16:53 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 15 Feb 2023 19:16:54 GMT
ENV XCADDY_SETCAP=1
# Wed, 15 Feb 2023 19:16:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 15 Feb 2023 19:16:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 15 Feb 2023 19:16:57 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788962e1689dbb14c760601cbf633ae350e98e3a045f8010924cd585de6b6a3e`  
		Last Modified: Fri, 10 Feb 2023 22:53:32 GMT  
		Size: 286.6 KB (286645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ae39b9ad00c218f9156f0958fa48f3062eb5830b791b8592e5f25fd576c7c5`  
		Last Modified: Tue, 14 Feb 2023 19:56:18 GMT  
		Size: 117.3 MB (117316160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f3bf55d586b31bb5c97f2cbf5167fd359b61336f93bed839c2f4de055ced88`  
		Last Modified: Tue, 14 Feb 2023 19:55:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e012d53123423a5fe128ab31d41596d83d8e48699ad608e9eb58dd0b2322fe0`  
		Last Modified: Tue, 14 Feb 2023 20:13:35 GMT  
		Size: 4.5 MB (4479556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90177e6cf58218f094608b8401f41d0da78a0cf57d95718e48e8c6e2f77c6fae`  
		Last Modified: Wed, 15 Feb 2023 19:18:00 GMT  
		Size: 1.1 MB (1105899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e897949e5a46b09b4606d86b20ecb5684cb43f7e1bed1f208ee9b7e93d208c`  
		Last Modified: Wed, 15 Feb 2023 19:17:59 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - linux; s390x

```console
$ docker pull caddy@sha256:8c80a3ba9211715e4a4892ab129d736ec6405a52630b14b828837b7307115c02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129610728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e05d79b3ea15e4e9b6f3f1a89c9e9b9580f66c78fcef17624a8c7bb9f3f51cb5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:27:44 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:27:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:47:03 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:48:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:48:53 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:48:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:48:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:48:53 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:10:01 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:10:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:10:01 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:10:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:10:02 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:10:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:10:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:10:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affa53ed2f1b70a83e3a15cae881ca47cd40f6ac11060717cdbbd4e405f9d586`  
		Last Modified: Fri, 10 Feb 2023 22:37:18 GMT  
		Size: 285.0 KB (285032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d83de48b90cbc8ae74a05d0af343e28f82727b9797b0b45ed9a70fa837a9a5`  
		Last Modified: Tue, 07 Mar 2023 23:53:54 GMT  
		Size: 120.8 MB (120808046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d22668a5d7432e1f8abda37a563ffa67f01cd8658b3247b89a7770eb41fe2a0`  
		Last Modified: Tue, 07 Mar 2023 23:53:38 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3beeef51570794945ced834a4af09db492ac50aadef9f4120ccc6b1dcb4f1251`  
		Last Modified: Wed, 08 Mar 2023 00:10:47 GMT  
		Size: 4.2 MB (4171573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57140a7518a2548d3fd2cef1ecb24c3b4ffb6aee2cc51f3921cb5497bf0863ce`  
		Last Modified: Wed, 08 Mar 2023 00:10:38 GMT  
		Size: 1.2 MB (1170402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe35434ab4b6dfcd2742bd2454af4cb9fe85cc900cacf2e2ef375861498fa09e`  
		Last Modified: Wed, 08 Mar 2023 00:10:38 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - windows version 10.0.17763.4010; amd64

```console
$ docker pull caddy@sha256:698c8dda106fb34e783e5030fd3ea5166df618f08c2a01204a7a82aabf6b20c9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2148348831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cee813843af987f6985470a05839367529db056040844b778343ebd71743f6a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 23:47:41 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Feb 2023 23:47:42 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Feb 2023 23:47:43 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Feb 2023 23:47:44 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Feb 2023 23:50:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Feb 2023 23:50:19 GMT
ENV GOPATH=C:\go
# Wed, 15 Feb 2023 23:51:42 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Feb 2023 00:11:44 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 16 Feb 2023 00:17:12 GMT
RUN $url = 'https://dl.google.com/go/go1.19.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '8d84af29e46c38b1eec77f9310310517c9e394ac7489e1c7329a94b443b0388d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Feb 2023 00:17:13 GMT
WORKDIR C:\go
# Thu, 16 Feb 2023 02:48:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:48:16 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Feb 2023 02:48:17 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:48:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Feb 2023 02:49:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Feb 2023 02:49:37 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03ac75ee62e05ad7b8b8f97fb78a769177c49d210eedcf0a93035e9a07d0ff2`  
		Last Modified: Thu, 16 Feb 2023 00:28:24 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4beb360c9024340aa5072ce67eab6b3cb005293938525c4f3b77c3bb03f9f501`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5051ce7a895da09ac63e7ca01ef4e30434d833dbd271107d6f96375f291752ad`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea419e1594fbbef3584b4731c356499c7b8a5616af16968e6fd693eccd92012b`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb97c6a047d2cfcb6f0ef6846e78c4d5f60212639a9d1892e2af05033c217df`  
		Last Modified: Thu, 16 Feb 2023 00:28:30 GMT  
		Size: 25.6 MB (25606151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941d25224d4bab25ba0b2304a5811b0fc2970ba6385afdbefbfec898720c3beb`  
		Last Modified: Thu, 16 Feb 2023 00:28:17 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa161895f771062e6d8e8aa2e0e44c15c5affdacc8d409f6e70f1fa743a9bb1`  
		Last Modified: Thu, 16 Feb 2023 00:28:17 GMT  
		Size: 335.6 KB (335550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd14ed3be87ab223f1391d40c3cdcfcee876586e89fbeed2aeccb318734a22`  
		Last Modified: Thu, 16 Feb 2023 00:32:40 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddec1d087c619cf7156e3dba04dd6a73e704d66c60e3fbc4b32c73b4401471b`  
		Last Modified: Thu, 16 Feb 2023 00:33:24 GMT  
		Size: 157.8 MB (157798436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50612066f9b2d86b5cecd95ce6897d89929be6a819c3de13dd9ecc32948832cb`  
		Last Modified: Thu, 16 Feb 2023 00:32:40 GMT  
		Size: 1.5 KB (1544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3bbcb2df900a9ead208e08eefd6faa32bbd6c5a189212d97b94eec1e5807a24`  
		Last Modified: Thu, 16 Feb 2023 02:51:49 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b5e7db448c55e5e60ab1aefceb414700fb99de06cc1c047404e32031064e0c`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7af0982eb604918cfaece327a35d278b59d5f2ca440882b5e7d402e7cce80f6`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad49ef8883b47edaa38ca21b422551a4da50f675370fc1596432938cd7de4d2`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce066417e925c257e21d7126cbbdcf5316022725a7ef7a89575b86fd534d133f`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.6 MB (1632671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbe58e4b6c6b7d8f16c2682325b6df5f61050915e6af7829adab49c1914e5c9`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - windows version 10.0.20348.1547; amd64

```console
$ docker pull caddy@sha256:21d50bd59eead7016b606e72f6dede55b7f2c718f306c823f3a34ef794622aa7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1865665598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f3a334b2d908beba62aa4ea43b950f4be8fa2261a29819fecc52e58eaadf2df`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 23:42:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Feb 2023 23:42:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Feb 2023 23:42:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Feb 2023 23:42:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Feb 2023 23:43:27 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Feb 2023 23:43:28 GMT
ENV GOPATH=C:\go
# Wed, 15 Feb 2023 23:44:03 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Feb 2023 00:07:02 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 16 Feb 2023 00:11:25 GMT
RUN $url = 'https://dl.google.com/go/go1.19.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '8d84af29e46c38b1eec77f9310310517c9e394ac7489e1c7329a94b443b0388d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Feb 2023 00:11:27 GMT
WORKDIR C:\go
# Thu, 16 Feb 2023 02:49:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:49:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Feb 2023 02:49:47 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:49:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Feb 2023 02:50:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Feb 2023 02:50:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4048a86b3278e59b840ad06b4cf5f5888ce1068d503522a95eb470d5126ed69a`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b07973952171f91c05aade363f3e6c9a2e84548f33eaa3c8e48632460e61f8`  
		Last Modified: Thu, 16 Feb 2023 00:26:45 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a95dff10905572b5f9177959a5a9f60a9364e1dd627ed52e34ec4bee3fb3069`  
		Last Modified: Thu, 16 Feb 2023 00:26:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4267caf437f5a3d92235ab7b8d55b2c812744f166725151ba701aef9d682c6e9`  
		Last Modified: Thu, 16 Feb 2023 00:26:41 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982a959ece2e33bce3f35c5c0adb01a3426c92111b309c15f8cc31200ebcf899`  
		Last Modified: Thu, 16 Feb 2023 00:26:54 GMT  
		Size: 25.9 MB (25852811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065416c07c5d80f7a085e0e84237051d7050a71103cc9d7fb6d5ef57725dc4c6`  
		Last Modified: Thu, 16 Feb 2023 00:26:39 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07015cae66c7ebb6b0adce2dfe424313b228bb703ac3e900deebe74ae961bb49`  
		Last Modified: Thu, 16 Feb 2023 00:26:40 GMT  
		Size: 571.7 KB (571672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285847798b3738c8863954b395d2e44410be1004e9f8513dd1546a0713f153d3`  
		Last Modified: Thu, 16 Feb 2023 00:31:40 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4f6797c9312e8b2093037565c19561d6152cca51a84614b32c0813526f219f`  
		Last Modified: Thu, 16 Feb 2023 00:32:31 GMT  
		Size: 158.0 MB (158008192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2bd8446758388c6c8ddb5d51dd63d25a0dbf5c8e1385928c5e64c83948d966`  
		Last Modified: Thu, 16 Feb 2023 00:31:40 GMT  
		Size: 1.6 KB (1561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd741098e5131c0452f3451d13ce2b131c36cbfcf24df5fbd2fb9e5751e85627`  
		Last Modified: Thu, 16 Feb 2023 02:52:08 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcd5d2a85aea028cd55d32ae579beb21aa5efc8eb3875d901dfcb623092327a`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f63b7e14eef097ca8f36e589d8d609a276d3196875467da71a714db6c8e583`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2e98e1ab65293643e4b2173a01d386c2129bf22ffaee5d1b730f19a26759a7`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15030494f30adf45739bdc5e411e1ae7ea0395ebcb4c2a4f74eedbc5f71d3acd`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.9 MB (1868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba874cf328299688fd26dd5261c439698422f93ce708e583e0e248444622caff`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-builder-alpine`

```console
$ docker pull caddy@sha256:68f552074b7668f5c49a7545bad89568f46b134851ee4bb7f558fe6b2e7b7749
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.6.4-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:47722ffc694507be1e2f34ca172e292fb5e226ea68d87871300b9d65f543fcce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131421587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4674ac67a52f4d29bc8349e9dcca7db8393d778c97c79d9e2f6e997603a99cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 08:21:54 GMT
RUN apk add --no-cache ca-certificates
# Sat, 11 Feb 2023 08:21:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:24:10 GMT
ENV GOLANG_VERSION=1.19.6
# Tue, 14 Feb 2023 19:25:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 14 Feb 2023 19:25:43 GMT
ENV GOPATH=/go
# Tue, 14 Feb 2023 19:25:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:25:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Feb 2023 19:25:44 GMT
WORKDIR /go
# Tue, 14 Feb 2023 19:47:10 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 14 Feb 2023 19:47:10 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 15 Feb 2023 19:19:27 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:19:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 15 Feb 2023 19:19:28 GMT
ENV XCADDY_SETCAP=1
# Wed, 15 Feb 2023 19:19:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 15 Feb 2023 19:19:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 15 Feb 2023 19:19:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d21d5440ebff5aaaaeb115a003f7a4a3897f1866a87de95bc4a21436fc563c`  
		Last Modified: Sat, 11 Feb 2023 08:29:10 GMT  
		Size: 284.8 KB (284816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f790f4c5274f100158d4c23bc5eddf659c1fe93ef4025488f9493d88f1490d88`  
		Last Modified: Tue, 14 Feb 2023 19:31:12 GMT  
		Size: 122.4 MB (122355677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bf170fd9e6726c86c0d4b478d9ec522e82c527a8e708668f48233a4d03f618`  
		Last Modified: Tue, 14 Feb 2023 19:30:55 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a5d1c1b6ed103f8c7f97c73ed546ff7e767b10473b55c15c0d4e1a13a69481`  
		Last Modified: Tue, 14 Feb 2023 19:47:34 GMT  
		Size: 4.2 MB (4188243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0130eaa2f0b1f7646719d82927743bd84c83ed450eb8be4db5327d280d5e4d0`  
		Last Modified: Wed, 15 Feb 2023 19:20:05 GMT  
		Size: 1.2 MB (1217841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab1f57409241476a86d26944527bc2c6c3903eadb21221b8d96da52120b3109`  
		Last Modified: Wed, 15 Feb 2023 19:20:05 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e2b8479c011649b6d47ead7051ebf36d10e2c764f2bc3bc507eab00a1812b6a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127455561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7351cc9a113eeb1deb8afa4c19e381df6b5e03cfef4e63e47bfe99f0b43d95ab`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:28 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Fri, 10 Feb 2023 20:49:28 GMT
CMD ["/bin/sh"]
# Tue, 07 Mar 2023 23:49:29 GMT
RUN apk add --no-cache ca-certificates
# Tue, 07 Mar 2023 23:49:29 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:53:43 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:55:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:55:31 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:55:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:55:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:55:32 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:17:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:17:50 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:17:50 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:17:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:17:51 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:17:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:17:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:17:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06dc45fa3a2f6e0270fe56d6b9f8efada3c9b5854707b52fe42dd55844fb1d5`  
		Last Modified: Tue, 07 Mar 2023 23:58:16 GMT  
		Size: 286.2 KB (286214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9c435c140baf308bcd21b10be4fe27e2cec5ec2acccb0cba35e7ec207d54ae`  
		Last Modified: Tue, 07 Mar 2023 23:59:54 GMT  
		Size: 118.7 MB (118731518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f756f642eb6722bcddfd36a868987c31f5583a7bac2ccf573f8c4fc55198ad49`  
		Last Modified: Tue, 07 Mar 2023 23:59:33 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c49be1b95c6f947e8aaed6708b2c0b38ea78e63b117ac389af00cca5f95334f`  
		Last Modified: Wed, 08 Mar 2023 00:18:51 GMT  
		Size: 4.2 MB (4160310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1cd39813132ad141affe91c6d7f78654e7dbe1e8454baf43e2ee60f2480ecd`  
		Last Modified: Wed, 08 Mar 2023 00:18:51 GMT  
		Size: 1.2 MB (1166071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6624093c59eca00c1b574cd2672bb86cf72a602c484c89dd864ab09d28d875b`  
		Last Modified: Wed, 08 Mar 2023 00:18:50 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:35dc985cc319ba4cd38b0f28d82ec4af14971a9336ce7870444c023c1415fa7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126524974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:822857d40d7e456ebf6b4405bd126f6499dd89ce092e55728fa8deaea4601da8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 02:15:04 GMT
RUN apk add --no-cache ca-certificates
# Thu, 02 Mar 2023 02:15:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 02:19:52 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 02 Mar 2023 02:21:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 02 Mar 2023 02:21:35 GMT
ENV GOPATH=/go
# Thu, 02 Mar 2023 02:21:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 02:21:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 02 Mar 2023 02:21:35 GMT
WORKDIR /go
# Thu, 02 Mar 2023 10:40:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 02 Mar 2023 10:40:26 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_SETCAP=1
# Thu, 02 Mar 2023 10:40:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 02 Mar 2023 10:40:28 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 02 Mar 2023 10:40:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4962ca8504034f69427a90f2b07cfde1e4c20297e4507d5620bb7ea27e646919`  
		Last Modified: Thu, 02 Mar 2023 02:26:02 GMT  
		Size: 285.4 KB (285445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20059bad54d9966d7995685d0c72ce1566c6370b4105df472360f5d2c8ecd21`  
		Last Modified: Thu, 02 Mar 2023 02:28:31 GMT  
		Size: 118.5 MB (118477876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4d49a4d60a68cc1326493b7f8b4cf548d4cec1694b7ccb266f06e4028b501d`  
		Last Modified: Thu, 02 Mar 2023 02:28:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0098f26d1429a39f7d8f6dd18417972d79d6706e530dbfbc4cf9991ff98f3c6`  
		Last Modified: Thu, 02 Mar 2023 10:41:22 GMT  
		Size: 3.7 MB (3729269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0aafe51cc793a860e8c2f2c4799c11f9bebe521643a6f6578f348ce06ae80d`  
		Last Modified: Thu, 02 Mar 2023 10:41:22 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24f3750a2b57fead59e3d812fa66ae7c79703a8a84d41670403b9dc7c23eb90`  
		Last Modified: Thu, 02 Mar 2023 10:41:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6e43472efedad7b414f4cce21a50e04578ea8527ad05ee901ba9eabc88d7718e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125849779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62beb7ef29ce475cb1f571275d3c9ac33185ec48844366ef16a99e8540239b2b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:38:33 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:38:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:43:17 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:44:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:44:26 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:44:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:44:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:44:27 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:06:06 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:06:06 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:06:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:06:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:06:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55522c79112429742fe76c795b9509c5cd1e8198e0caa2a1e355c0e60a719576`  
		Last Modified: Fri, 10 Feb 2023 22:44:19 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1815dcbf43e87e122cc76a24663b7c0d6e01ad03c3be30a7dc13c1bf941c595`  
		Last Modified: Tue, 07 Mar 2023 23:49:19 GMT  
		Size: 116.9 MB (116933985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5aad4e0c6f77e535fe5a51a211a4691a5002a111c52fa17708cf1bc7c01879`  
		Last Modified: Tue, 07 Mar 2023 23:49:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557acb83c53566587727172247e84b25f860b606c200b1fc863eafc75d6b0cf4`  
		Last Modified: Wed, 08 Mar 2023 00:06:29 GMT  
		Size: 4.2 MB (4243285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb71700cd911a18f7eb1f75d651639bc79bda4000e2f4e6a8afe570b03816eb`  
		Last Modified: Wed, 08 Mar 2023 00:06:29 GMT  
		Size: 1.1 MB (1123733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358517d9544ce3184d74860b7f2054339481407b928bb11ccbf7d35163006788`  
		Last Modified: Wed, 08 Mar 2023 00:06:28 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:8126a0d2b7cc9613f70b6b5375c14cc61dfca5dc1b83adc5be33efab8eacc69f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126579575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2da1cd24f35f4106a8a7176a2f2b5656a22982a1787b9204d3eaab9ec535ef58`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:40:13 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:40:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:46:09 GMT
ENV GOLANG_VERSION=1.19.6
# Tue, 14 Feb 2023 19:48:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 14 Feb 2023 19:48:44 GMT
ENV GOPATH=/go
# Tue, 14 Feb 2023 19:48:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:48:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Feb 2023 19:48:46 GMT
WORKDIR /go
# Tue, 14 Feb 2023 20:12:48 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 14 Feb 2023 20:12:48 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 15 Feb 2023 19:16:53 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 15 Feb 2023 19:16:54 GMT
ENV XCADDY_SETCAP=1
# Wed, 15 Feb 2023 19:16:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 15 Feb 2023 19:16:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 15 Feb 2023 19:16:57 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788962e1689dbb14c760601cbf633ae350e98e3a045f8010924cd585de6b6a3e`  
		Last Modified: Fri, 10 Feb 2023 22:53:32 GMT  
		Size: 286.6 KB (286645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ae39b9ad00c218f9156f0958fa48f3062eb5830b791b8592e5f25fd576c7c5`  
		Last Modified: Tue, 14 Feb 2023 19:56:18 GMT  
		Size: 117.3 MB (117316160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f3bf55d586b31bb5c97f2cbf5167fd359b61336f93bed839c2f4de055ced88`  
		Last Modified: Tue, 14 Feb 2023 19:55:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e012d53123423a5fe128ab31d41596d83d8e48699ad608e9eb58dd0b2322fe0`  
		Last Modified: Tue, 14 Feb 2023 20:13:35 GMT  
		Size: 4.5 MB (4479556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90177e6cf58218f094608b8401f41d0da78a0cf57d95718e48e8c6e2f77c6fae`  
		Last Modified: Wed, 15 Feb 2023 19:18:00 GMT  
		Size: 1.1 MB (1105899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e897949e5a46b09b4606d86b20ecb5684cb43f7e1bed1f208ee9b7e93d208c`  
		Last Modified: Wed, 15 Feb 2023 19:17:59 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:8c80a3ba9211715e4a4892ab129d736ec6405a52630b14b828837b7307115c02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129610728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e05d79b3ea15e4e9b6f3f1a89c9e9b9580f66c78fcef17624a8c7bb9f3f51cb5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:27:44 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:27:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:47:03 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:48:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:48:53 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:48:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:48:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:48:53 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:10:01 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:10:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:10:01 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:10:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:10:02 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:10:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:10:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:10:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affa53ed2f1b70a83e3a15cae881ca47cd40f6ac11060717cdbbd4e405f9d586`  
		Last Modified: Fri, 10 Feb 2023 22:37:18 GMT  
		Size: 285.0 KB (285032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d83de48b90cbc8ae74a05d0af343e28f82727b9797b0b45ed9a70fa837a9a5`  
		Last Modified: Tue, 07 Mar 2023 23:53:54 GMT  
		Size: 120.8 MB (120808046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d22668a5d7432e1f8abda37a563ffa67f01cd8658b3247b89a7770eb41fe2a0`  
		Last Modified: Tue, 07 Mar 2023 23:53:38 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3beeef51570794945ced834a4af09db492ac50aadef9f4120ccc6b1dcb4f1251`  
		Last Modified: Wed, 08 Mar 2023 00:10:47 GMT  
		Size: 4.2 MB (4171573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57140a7518a2548d3fd2cef1ecb24c3b4ffb6aee2cc51f3921cb5497bf0863ce`  
		Last Modified: Wed, 08 Mar 2023 00:10:38 GMT  
		Size: 1.2 MB (1170402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe35434ab4b6dfcd2742bd2454af4cb9fe85cc900cacf2e2ef375861498fa09e`  
		Last Modified: Wed, 08 Mar 2023 00:10:38 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:687ff9a9e85091470e7d84be08a4e96d119290226bfcd464502138db4b9f1542
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4010; amd64

### `caddy:2.6.4-builder-windowsservercore-1809` - windows version 10.0.17763.4010; amd64

```console
$ docker pull caddy@sha256:698c8dda106fb34e783e5030fd3ea5166df618f08c2a01204a7a82aabf6b20c9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2148348831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cee813843af987f6985470a05839367529db056040844b778343ebd71743f6a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 23:47:41 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Feb 2023 23:47:42 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Feb 2023 23:47:43 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Feb 2023 23:47:44 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Feb 2023 23:50:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Feb 2023 23:50:19 GMT
ENV GOPATH=C:\go
# Wed, 15 Feb 2023 23:51:42 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Feb 2023 00:11:44 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 16 Feb 2023 00:17:12 GMT
RUN $url = 'https://dl.google.com/go/go1.19.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '8d84af29e46c38b1eec77f9310310517c9e394ac7489e1c7329a94b443b0388d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Feb 2023 00:17:13 GMT
WORKDIR C:\go
# Thu, 16 Feb 2023 02:48:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:48:16 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Feb 2023 02:48:17 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:48:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Feb 2023 02:49:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Feb 2023 02:49:37 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03ac75ee62e05ad7b8b8f97fb78a769177c49d210eedcf0a93035e9a07d0ff2`  
		Last Modified: Thu, 16 Feb 2023 00:28:24 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4beb360c9024340aa5072ce67eab6b3cb005293938525c4f3b77c3bb03f9f501`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5051ce7a895da09ac63e7ca01ef4e30434d833dbd271107d6f96375f291752ad`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea419e1594fbbef3584b4731c356499c7b8a5616af16968e6fd693eccd92012b`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb97c6a047d2cfcb6f0ef6846e78c4d5f60212639a9d1892e2af05033c217df`  
		Last Modified: Thu, 16 Feb 2023 00:28:30 GMT  
		Size: 25.6 MB (25606151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941d25224d4bab25ba0b2304a5811b0fc2970ba6385afdbefbfec898720c3beb`  
		Last Modified: Thu, 16 Feb 2023 00:28:17 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa161895f771062e6d8e8aa2e0e44c15c5affdacc8d409f6e70f1fa743a9bb1`  
		Last Modified: Thu, 16 Feb 2023 00:28:17 GMT  
		Size: 335.6 KB (335550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd14ed3be87ab223f1391d40c3cdcfcee876586e89fbeed2aeccb318734a22`  
		Last Modified: Thu, 16 Feb 2023 00:32:40 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddec1d087c619cf7156e3dba04dd6a73e704d66c60e3fbc4b32c73b4401471b`  
		Last Modified: Thu, 16 Feb 2023 00:33:24 GMT  
		Size: 157.8 MB (157798436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50612066f9b2d86b5cecd95ce6897d89929be6a819c3de13dd9ecc32948832cb`  
		Last Modified: Thu, 16 Feb 2023 00:32:40 GMT  
		Size: 1.5 KB (1544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3bbcb2df900a9ead208e08eefd6faa32bbd6c5a189212d97b94eec1e5807a24`  
		Last Modified: Thu, 16 Feb 2023 02:51:49 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b5e7db448c55e5e60ab1aefceb414700fb99de06cc1c047404e32031064e0c`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7af0982eb604918cfaece327a35d278b59d5f2ca440882b5e7d402e7cce80f6`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad49ef8883b47edaa38ca21b422551a4da50f675370fc1596432938cd7de4d2`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce066417e925c257e21d7126cbbdcf5316022725a7ef7a89575b86fd534d133f`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.6 MB (1632671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbe58e4b6c6b7d8f16c2682325b6df5f61050915e6af7829adab49c1914e5c9`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:573ab227ac93b402974ef9c7f039983bc070f5e08c73d21e62345c13f8ccbaab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `caddy:2.6.4-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1547; amd64

```console
$ docker pull caddy@sha256:21d50bd59eead7016b606e72f6dede55b7f2c718f306c823f3a34ef794622aa7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1865665598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f3a334b2d908beba62aa4ea43b950f4be8fa2261a29819fecc52e58eaadf2df`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 23:42:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Feb 2023 23:42:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Feb 2023 23:42:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Feb 2023 23:42:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Feb 2023 23:43:27 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Feb 2023 23:43:28 GMT
ENV GOPATH=C:\go
# Wed, 15 Feb 2023 23:44:03 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Feb 2023 00:07:02 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 16 Feb 2023 00:11:25 GMT
RUN $url = 'https://dl.google.com/go/go1.19.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '8d84af29e46c38b1eec77f9310310517c9e394ac7489e1c7329a94b443b0388d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Feb 2023 00:11:27 GMT
WORKDIR C:\go
# Thu, 16 Feb 2023 02:49:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:49:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Feb 2023 02:49:47 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:49:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Feb 2023 02:50:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Feb 2023 02:50:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4048a86b3278e59b840ad06b4cf5f5888ce1068d503522a95eb470d5126ed69a`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b07973952171f91c05aade363f3e6c9a2e84548f33eaa3c8e48632460e61f8`  
		Last Modified: Thu, 16 Feb 2023 00:26:45 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a95dff10905572b5f9177959a5a9f60a9364e1dd627ed52e34ec4bee3fb3069`  
		Last Modified: Thu, 16 Feb 2023 00:26:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4267caf437f5a3d92235ab7b8d55b2c812744f166725151ba701aef9d682c6e9`  
		Last Modified: Thu, 16 Feb 2023 00:26:41 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982a959ece2e33bce3f35c5c0adb01a3426c92111b309c15f8cc31200ebcf899`  
		Last Modified: Thu, 16 Feb 2023 00:26:54 GMT  
		Size: 25.9 MB (25852811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065416c07c5d80f7a085e0e84237051d7050a71103cc9d7fb6d5ef57725dc4c6`  
		Last Modified: Thu, 16 Feb 2023 00:26:39 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07015cae66c7ebb6b0adce2dfe424313b228bb703ac3e900deebe74ae961bb49`  
		Last Modified: Thu, 16 Feb 2023 00:26:40 GMT  
		Size: 571.7 KB (571672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285847798b3738c8863954b395d2e44410be1004e9f8513dd1546a0713f153d3`  
		Last Modified: Thu, 16 Feb 2023 00:31:40 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4f6797c9312e8b2093037565c19561d6152cca51a84614b32c0813526f219f`  
		Last Modified: Thu, 16 Feb 2023 00:32:31 GMT  
		Size: 158.0 MB (158008192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2bd8446758388c6c8ddb5d51dd63d25a0dbf5c8e1385928c5e64c83948d966`  
		Last Modified: Thu, 16 Feb 2023 00:31:40 GMT  
		Size: 1.6 KB (1561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd741098e5131c0452f3451d13ce2b131c36cbfcf24df5fbd2fb9e5751e85627`  
		Last Modified: Thu, 16 Feb 2023 02:52:08 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcd5d2a85aea028cd55d32ae579beb21aa5efc8eb3875d901dfcb623092327a`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f63b7e14eef097ca8f36e589d8d609a276d3196875467da71a714db6c8e583`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2e98e1ab65293643e4b2173a01d386c2129bf22ffaee5d1b730f19a26759a7`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15030494f30adf45739bdc5e411e1ae7ea0395ebcb4c2a4f74eedbc5f71d3acd`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.9 MB (1868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba874cf328299688fd26dd5261c439698422f93ce708e583e0e248444622caff`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-windowsservercore`

```console
$ docker pull caddy@sha256:07fbc5a89186611e042f7ab23685ae8afbcce5678ff9b1315e742e6935052c9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4010; amd64
	-	windows version 10.0.20348.1547; amd64

### `caddy:2.6.4-windowsservercore` - windows version 10.0.17763.4010; amd64

```console
$ docker pull caddy@sha256:f78e6d4fc1641b322d4e44adcada628f9acb5106b2e166cbcba796764a4db257
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1978492183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:198e4772b4788d7810819799af107998abe8e241416654ca5406331afefc2908`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:43:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:44:00 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:45:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:45:08 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:45:09 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:45:10 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:45:11 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:45:12 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:45:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:45:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:45:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:45:17 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:45:19 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:46:11 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:46:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f19b532038d3c84c40068e825815f2b252b82869809b11745d9893f12a99ac1`  
		Last Modified: Thu, 16 Feb 2023 02:51:03 GMT  
		Size: 526.3 KB (526332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15f6c8f1e7f194b2b408bf6c4330db67cf7cd4783d39acba2d8384b2f3c31d4`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab346a52e8e98a31f0970c85a32f1653b5179dd5ad781a8764b08de792a4d99`  
		Last Modified: Thu, 16 Feb 2023 02:51:05 GMT  
		Size: 14.7 MB (14677251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4451f67396ee792e3ace473ca4a69e5e49639ab8b620e489635a7b2eeb775523`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9291ccd53cd67f009cd59c77d90d2623192e5e134fc2ad5a03f1c1860ab66b80`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3096247c037e7418f5efc50ce5c7e6bc272ccac5c014f5cb085d77c4c28a3a`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f902038f4ba892bc3e1e4d5fdcef6b7759891c41c067b744fa3d5b008776c90`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82e400c4f2072b1e2b2ff49169de3108075208b544f454b3cdf016be6356321`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0944799324319439cbaf2f01dd147e8cc496ea80243ddc22e59e301237acb293`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce6c226ffeaa8146cae1b818b43a4776a06f6ce0be460b7d9b42fcc503b39db`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0b36e09fd7994e37dd27ccdcfa4610fc1219c4044a95695c6de9f9eecda63b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f284721a924468c7a0ff80b2809a222ae20cae99d35aa761b5296272783263b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bec609c0b4d99a9726ad86662d32a57664d18dde9d9087c0695ec7e9c4a47c`  
		Last Modified: Thu, 16 Feb 2023 02:50:59 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ad796550cc1ac21dd77352cf12cc78cacbd0a9f8a1e728e7e4f6a02a0cb9fb`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1955699b7dbbfef476622c70f983565943bafe8909c80ec278dff19509fad86`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4096827c6eb36146321a048a5041be746e60afe4c8e90717d681f2d271e0143`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc99e795e3855739a0c170e77263147dec07ac66a9ae51c306705be5af6574b`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8683be90a75d0e97aa8b7002c075e040e7299bd1fde397a541df3e7e4168d97`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 308.1 KB (308099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156392510131bc65057e3573b9aa9838fccd38cc8ed89734e5255bcd4a315274`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-windowsservercore` - windows version 10.0.20348.1547; amd64

```console
$ docker pull caddy@sha256:87b9acadc87fc1f78b7ee864f06462a0f45aa263af20fa1744e2f2a0d0870b02
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1695421581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaff43d5343d972f345ff5561ee131879eaafd463e389a1c2607715ac3f6e793`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:46:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:46:57 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:47:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:47:26 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:47:27 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:47:28 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:47:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:47:31 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:47:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:47:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:47:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:47:36 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:47:37 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:47:56 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:47:57 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1961fba6606566986ddd1960cf8309d19fa9deaa486f5a162a60114f3d4c3c82`  
		Last Modified: Thu, 16 Feb 2023 02:51:29 GMT  
		Size: 778.8 KB (778807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af5d76bf41697a16b3336a1857d1e530a3137f28d997c6f5eca0121d42ea88d`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d935f5b810851a2833b69e65d9dcff828f1c6686dab6fa117e9bd08eb95f5990`  
		Last Modified: Thu, 16 Feb 2023 02:51:31 GMT  
		Size: 14.9 MB (14914232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54e2a419181dd9257efde40f9ab80121dd6cc1a478f6ff42d160ddbf5e17cd4`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c07f1bbb0931b3148683baae55ab0d85f8576b2a1d8c2a59bb28544572b5a9d`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06073fd741cf5968f24574903b70213f9743b648ebec9c53ccb8fe114ce01ae`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a17243f1184726e21bf0821ee5984a84575b55befba72594fbf0b3a32a47f1`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c403099e0a283f6f2b25b4235c61c8b564a832643f33280253dc040d2a2ab07`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cc4608f06891b205fbec74e83a221161a2f9d9b50a0b548c3c716d176ee1a4`  
		Last Modified: Thu, 16 Feb 2023 02:51:25 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfe2ac143052b1fa8973567134244ce4ecd1693f16205dd53f0d4cf1b5caa5a`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e217159efeb187bf7ae9a12f6f70764141dd97837f24a517851bc15a36b552`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc05a7da758918922e168d1b07b29f4a81d398dc805724dd6b23b4cb28c7b43`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832768cea319f33011657944b08b51ea41229fdd7a37f21162dd8aedceb31a6b`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443fc82ac63aefa17f6de497731a007fbc972b175040388a8fda7112834af9fa`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39ff50a2c37b226c6e79e3789d1706fc47cb355b14372a147024fc11b2dfb2b`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c6037df6cbd4b9e046dded7157e841a1c40659c4dd082ff9d397c95be6e411`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a470cfe53e2d01e3ca43a7211eb050493a97f430e3c5a52e2364f54a0a4e4834`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d12a1c4350235354af8011d0b2eccb56884eea72a0475197fb007c4fa6c111`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 359.9 KB (359894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea80c894fe52045adaa4c44b9f66422259571c7aec153753d27a56aa3ccbd930`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-windowsservercore-1809`

```console
$ docker pull caddy@sha256:1bd6dc9cf41fc94696e73caafb13f1e2aa4080c4961ffe195303c2a51811ff9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4010; amd64

### `caddy:2.6.4-windowsservercore-1809` - windows version 10.0.17763.4010; amd64

```console
$ docker pull caddy@sha256:f78e6d4fc1641b322d4e44adcada628f9acb5106b2e166cbcba796764a4db257
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1978492183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:198e4772b4788d7810819799af107998abe8e241416654ca5406331afefc2908`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:43:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:44:00 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:45:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:45:08 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:45:09 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:45:10 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:45:11 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:45:12 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:45:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:45:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:45:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:45:17 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:45:19 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:46:11 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:46:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f19b532038d3c84c40068e825815f2b252b82869809b11745d9893f12a99ac1`  
		Last Modified: Thu, 16 Feb 2023 02:51:03 GMT  
		Size: 526.3 KB (526332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15f6c8f1e7f194b2b408bf6c4330db67cf7cd4783d39acba2d8384b2f3c31d4`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab346a52e8e98a31f0970c85a32f1653b5179dd5ad781a8764b08de792a4d99`  
		Last Modified: Thu, 16 Feb 2023 02:51:05 GMT  
		Size: 14.7 MB (14677251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4451f67396ee792e3ace473ca4a69e5e49639ab8b620e489635a7b2eeb775523`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9291ccd53cd67f009cd59c77d90d2623192e5e134fc2ad5a03f1c1860ab66b80`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3096247c037e7418f5efc50ce5c7e6bc272ccac5c014f5cb085d77c4c28a3a`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f902038f4ba892bc3e1e4d5fdcef6b7759891c41c067b744fa3d5b008776c90`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82e400c4f2072b1e2b2ff49169de3108075208b544f454b3cdf016be6356321`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0944799324319439cbaf2f01dd147e8cc496ea80243ddc22e59e301237acb293`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce6c226ffeaa8146cae1b818b43a4776a06f6ce0be460b7d9b42fcc503b39db`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0b36e09fd7994e37dd27ccdcfa4610fc1219c4044a95695c6de9f9eecda63b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f284721a924468c7a0ff80b2809a222ae20cae99d35aa761b5296272783263b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bec609c0b4d99a9726ad86662d32a57664d18dde9d9087c0695ec7e9c4a47c`  
		Last Modified: Thu, 16 Feb 2023 02:50:59 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ad796550cc1ac21dd77352cf12cc78cacbd0a9f8a1e728e7e4f6a02a0cb9fb`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1955699b7dbbfef476622c70f983565943bafe8909c80ec278dff19509fad86`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4096827c6eb36146321a048a5041be746e60afe4c8e90717d681f2d271e0143`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc99e795e3855739a0c170e77263147dec07ac66a9ae51c306705be5af6574b`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8683be90a75d0e97aa8b7002c075e040e7299bd1fde397a541df3e7e4168d97`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 308.1 KB (308099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156392510131bc65057e3573b9aa9838fccd38cc8ed89734e5255bcd4a315274`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:bdada4aecbae3dbf7c909817361c5c5e025530a60f1017107cf4cbe628e5a12b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `caddy:2.6.4-windowsservercore-ltsc2022` - windows version 10.0.20348.1547; amd64

```console
$ docker pull caddy@sha256:87b9acadc87fc1f78b7ee864f06462a0f45aa263af20fa1744e2f2a0d0870b02
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1695421581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaff43d5343d972f345ff5561ee131879eaafd463e389a1c2607715ac3f6e793`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:46:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:46:57 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:47:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:47:26 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:47:27 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:47:28 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:47:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:47:31 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:47:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:47:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:47:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:47:36 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:47:37 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:47:56 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:47:57 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1961fba6606566986ddd1960cf8309d19fa9deaa486f5a162a60114f3d4c3c82`  
		Last Modified: Thu, 16 Feb 2023 02:51:29 GMT  
		Size: 778.8 KB (778807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af5d76bf41697a16b3336a1857d1e530a3137f28d997c6f5eca0121d42ea88d`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d935f5b810851a2833b69e65d9dcff828f1c6686dab6fa117e9bd08eb95f5990`  
		Last Modified: Thu, 16 Feb 2023 02:51:31 GMT  
		Size: 14.9 MB (14914232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54e2a419181dd9257efde40f9ab80121dd6cc1a478f6ff42d160ddbf5e17cd4`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c07f1bbb0931b3148683baae55ab0d85f8576b2a1d8c2a59bb28544572b5a9d`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06073fd741cf5968f24574903b70213f9743b648ebec9c53ccb8fe114ce01ae`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a17243f1184726e21bf0821ee5984a84575b55befba72594fbf0b3a32a47f1`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c403099e0a283f6f2b25b4235c61c8b564a832643f33280253dc040d2a2ab07`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cc4608f06891b205fbec74e83a221161a2f9d9b50a0b548c3c716d176ee1a4`  
		Last Modified: Thu, 16 Feb 2023 02:51:25 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfe2ac143052b1fa8973567134244ce4ecd1693f16205dd53f0d4cf1b5caa5a`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e217159efeb187bf7ae9a12f6f70764141dd97837f24a517851bc15a36b552`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc05a7da758918922e168d1b07b29f4a81d398dc805724dd6b23b4cb28c7b43`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832768cea319f33011657944b08b51ea41229fdd7a37f21162dd8aedceb31a6b`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443fc82ac63aefa17f6de497731a007fbc972b175040388a8fda7112834af9fa`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39ff50a2c37b226c6e79e3789d1706fc47cb355b14372a147024fc11b2dfb2b`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c6037df6cbd4b9e046dded7157e841a1c40659c4dd082ff9d397c95be6e411`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a470cfe53e2d01e3ca43a7211eb050493a97f430e3c5a52e2364f54a0a4e4834`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d12a1c4350235354af8011d0b2eccb56884eea72a0475197fb007c4fa6c111`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 359.9 KB (359894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea80c894fe52045adaa4c44b9f66422259571c7aec153753d27a56aa3ccbd930`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:3f4414616d9141c4fbd9f66641d9b91a3b67833dd4145738c536dee584db5314
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
$ docker pull caddy@sha256:36ba71b44afa613ecf0aadce8e4b9e3f56e0c4b0a78c8edf4e8c2485f21b35ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17449113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8464e23f16f9a82426bbdc3ac8c94270a84453ddc86b9147505a2378a7c2fd0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:38:34 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 11 Feb 2023 07:38:36 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:19:21 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:19:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:19:23 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:19:24 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:19:25 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e3e797818bc929d95bae8220b7b6034b559c217ef5bf622dc7fedc8d270a48`  
		Last Modified: Sat, 11 Feb 2023 07:39:01 GMT  
		Size: 351.2 KB (351178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cebb4c80b3906a9b751ee9a512c1581331b1fd691c84f575c01a29e28403dde`  
		Last Modified: Sat, 11 Feb 2023 07:39:00 GMT  
		Size: 7.6 KB (7552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90648ba22c191b969d8db393bf6138e7d6ecc1b70b3865d1717ec4d663192d89`  
		Last Modified: Wed, 15 Feb 2023 19:19:52 GMT  
		Size: 14.3 MB (14282621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:db317e683b30c11665349301255c3c59f3f5b085d4e075553e445129981ad5e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16582515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4628532cad0308b1d01506925ca941dffeb3bdd058cd79ccd7f055dce243e3b6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:32 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Fri, 10 Feb 2023 20:49:32 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 00:17:32 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 08 Mar 2023 00:17:34 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 08 Mar 2023 00:17:34 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:17:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 08 Mar 2023 00:17:38 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 08 Mar 2023 00:17:39 GMT
ENV XDG_DATA_HOME=/data
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 08 Mar 2023 00:17:41 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 80
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 443
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 443/udp
# Wed, 08 Mar 2023 00:17:42 GMT
EXPOSE 2019
# Wed, 08 Mar 2023 00:17:42 GMT
WORKDIR /srv
# Wed, 08 Mar 2023 00:17:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e676ebf894f684676e3a3c92294bbc14ba7061c7d24285909e673075903c39a9`  
		Last Modified: Wed, 08 Mar 2023 00:18:32 GMT  
		Size: 345.9 KB (345903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b146a16f288a28f362ad572b56958616fb5f4e0572bbe406ce18868be0d5c3`  
		Last Modified: Wed, 08 Mar 2023 00:18:31 GMT  
		Size: 7.6 KB (7559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e662de32a44a67eae886e653355902b11fec7407264122f1e72b5c460cb4334`  
		Last Modified: Wed, 08 Mar 2023 00:18:34 GMT  
		Size: 13.6 MB (13612275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:03b5f2d631567d2783e8977e4988bdc75f13acb5c5b7bb18f3984045fb557b11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16365710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bed848976d2f2ce06398c52bf359363302bd512c4c51f08acb50cdd7ec0db5a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 10:40:15 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 02 Mar 2023 10:40:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 02 Mar 2023 10:40:16 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 02 Mar 2023 10:40:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 02 Mar 2023 10:40:19 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 02 Mar 2023 10:40:19 GMT
ENV XDG_DATA_HOME=/data
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 02 Mar 2023 10:40:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 02 Mar 2023 10:40:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 80
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 443
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 443/udp
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 2019
# Thu, 02 Mar 2023 10:40:20 GMT
WORKDIR /srv
# Thu, 02 Mar 2023 10:40:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769efc94ebb1351d7f88e191e0e5c768fc2462e89d73fa4b373005e8a912f367`  
		Last Modified: Thu, 02 Mar 2023 10:41:04 GMT  
		Size: 342.7 KB (342688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fb7d44b5e1d66fb60d8593e306cfef844841aca960cacb7258951888fcf79e`  
		Last Modified: Thu, 02 Mar 2023 10:41:04 GMT  
		Size: 7.6 KB (7560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818d68e9d461fbb298a8bb8f5467049d89e77e6324f72842c3d45e5af3d0767b`  
		Last Modified: Thu, 02 Mar 2023 10:41:06 GMT  
		Size: 13.6 MB (13594968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6c2623f6bf30798be5c37fc7484e45ecc288d493fb657883f59ddb27ed714ad8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16130997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a38afdc517ef4cff6b6b51a1c6a633c2826599b07feb1e88380d0f783e35cf1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:00:35 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:00:37 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 18:39:20 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 18:39:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 18:39:22 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 18:39:22 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 80
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 443
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 18:39:23 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 18:39:23 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70730e8e2fb933ec157ec87f2a4fb4ad45e8e578b8f7c76cc4846631d773554`  
		Last Modified: Fri, 10 Feb 2023 22:01:02 GMT  
		Size: 350.2 KB (350153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a4b7390d269477c225f1d03e825d2d8bdf6b4d87b5f7bb8811b341e56b7d36`  
		Last Modified: Fri, 10 Feb 2023 22:01:02 GMT  
		Size: 7.6 KB (7555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2743d2ef53ee6edb0e39c89bf16957e3a00990410b2d1a126dca1b2d196182`  
		Last Modified: Wed, 15 Feb 2023 18:39:53 GMT  
		Size: 13.1 MB (13063787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:8861ab3ae3d0c180e38142c2f7482f9ce1773419eb29ed9d6d18308246858093
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5819f0ab4928a30c29293a27299a3b44371cd3bd97df91432ef7b3f43b692d8c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:13:21 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:13:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:16:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:16:41 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:16:42 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:16:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:16:47 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:16:47 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:16:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bd0321e6539bb7dac8574fd36bad22059ef06bb63dc842165f69d0a821572`  
		Last Modified: Fri, 10 Feb 2023 22:14:16 GMT  
		Size: 363.1 KB (363088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb806b2600b0209a73fc7175ab778d0224661034b2f722bd1a0aec1eb9eabe3d`  
		Last Modified: Fri, 10 Feb 2023 22:14:15 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd7c8ae860931dd79dea76d33bc21bb11d89cd4d133cdb41078b040afc6633e`  
		Last Modified: Wed, 15 Feb 2023 19:17:41 GMT  
		Size: 12.8 MB (12779898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:4e1ed99f133abf02d6a7c77849978bb621f748e18c9cb9f7a1dbf88480ddb8d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45cd164da734310b788dcbd4f6c94bccff6e48705fe4d42ecca07a54e9459a9c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:31 GMT
ADD file:17af250b49631cf2acf655c85df90977eddab4c9afd67bda3c577db5200364f1 in / 
# Fri, 10 Feb 2023 21:41:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:14:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:14:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 18:41:48 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 18:41:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 18:41:59 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 18:41:59 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 18:42:00 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 18:42:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 18:42:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 18:42:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 18:42:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 18:42:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 18:42:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 18:42:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 18:42:05 GMT
EXPOSE 80
# Wed, 15 Feb 2023 18:42:06 GMT
EXPOSE 443
# Wed, 15 Feb 2023 18:42:07 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 18:42:07 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 18:42:08 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 18:42:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:667d93a24f321610e24486f3148545191f113ab9ab2444804087dd65ebbda9ed`  
		Last Modified: Fri, 10 Feb 2023 21:42:26 GMT  
		Size: 2.6 MB (2593581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e6ec82400496ce74e37120e1655955b79303daaa5b8ca7e956e3cd96ddd6e9`  
		Last Modified: Fri, 10 Feb 2023 22:15:05 GMT  
		Size: 352.8 KB (352801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5b992687f93ced3715ad97bd95ab37daef5685b784e195209caefbc48f14e9`  
		Last Modified: Fri, 10 Feb 2023 22:15:05 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ccc40924ce2df3343fa5465a92ccaa4ed80e0883190a99d3f468c60f9ddbcf8`  
		Last Modified: Wed, 15 Feb 2023 18:43:19 GMT  
		Size: 13.8 MB (13838817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:8fe3549f0a6c0db646ec94d25f0c2a87ea055f50cb73477405df8f6fd2349784
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4010; amd64
	-	windows version 10.0.20348.1547; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:47722ffc694507be1e2f34ca172e292fb5e226ea68d87871300b9d65f543fcce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131421587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4674ac67a52f4d29bc8349e9dcca7db8393d778c97c79d9e2f6e997603a99cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 08:21:54 GMT
RUN apk add --no-cache ca-certificates
# Sat, 11 Feb 2023 08:21:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:24:10 GMT
ENV GOLANG_VERSION=1.19.6
# Tue, 14 Feb 2023 19:25:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 14 Feb 2023 19:25:43 GMT
ENV GOPATH=/go
# Tue, 14 Feb 2023 19:25:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:25:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Feb 2023 19:25:44 GMT
WORKDIR /go
# Tue, 14 Feb 2023 19:47:10 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 14 Feb 2023 19:47:10 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 15 Feb 2023 19:19:27 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:19:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 15 Feb 2023 19:19:28 GMT
ENV XCADDY_SETCAP=1
# Wed, 15 Feb 2023 19:19:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 15 Feb 2023 19:19:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 15 Feb 2023 19:19:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d21d5440ebff5aaaaeb115a003f7a4a3897f1866a87de95bc4a21436fc563c`  
		Last Modified: Sat, 11 Feb 2023 08:29:10 GMT  
		Size: 284.8 KB (284816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f790f4c5274f100158d4c23bc5eddf659c1fe93ef4025488f9493d88f1490d88`  
		Last Modified: Tue, 14 Feb 2023 19:31:12 GMT  
		Size: 122.4 MB (122355677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bf170fd9e6726c86c0d4b478d9ec522e82c527a8e708668f48233a4d03f618`  
		Last Modified: Tue, 14 Feb 2023 19:30:55 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a5d1c1b6ed103f8c7f97c73ed546ff7e767b10473b55c15c0d4e1a13a69481`  
		Last Modified: Tue, 14 Feb 2023 19:47:34 GMT  
		Size: 4.2 MB (4188243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0130eaa2f0b1f7646719d82927743bd84c83ed450eb8be4db5327d280d5e4d0`  
		Last Modified: Wed, 15 Feb 2023 19:20:05 GMT  
		Size: 1.2 MB (1217841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab1f57409241476a86d26944527bc2c6c3903eadb21221b8d96da52120b3109`  
		Last Modified: Wed, 15 Feb 2023 19:20:05 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e2b8479c011649b6d47ead7051ebf36d10e2c764f2bc3bc507eab00a1812b6a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127455561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7351cc9a113eeb1deb8afa4c19e381df6b5e03cfef4e63e47bfe99f0b43d95ab`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:28 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Fri, 10 Feb 2023 20:49:28 GMT
CMD ["/bin/sh"]
# Tue, 07 Mar 2023 23:49:29 GMT
RUN apk add --no-cache ca-certificates
# Tue, 07 Mar 2023 23:49:29 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:53:43 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:55:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:55:31 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:55:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:55:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:55:32 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:17:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:17:50 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:17:50 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:17:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:17:51 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:17:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:17:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:17:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06dc45fa3a2f6e0270fe56d6b9f8efada3c9b5854707b52fe42dd55844fb1d5`  
		Last Modified: Tue, 07 Mar 2023 23:58:16 GMT  
		Size: 286.2 KB (286214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9c435c140baf308bcd21b10be4fe27e2cec5ec2acccb0cba35e7ec207d54ae`  
		Last Modified: Tue, 07 Mar 2023 23:59:54 GMT  
		Size: 118.7 MB (118731518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f756f642eb6722bcddfd36a868987c31f5583a7bac2ccf573f8c4fc55198ad49`  
		Last Modified: Tue, 07 Mar 2023 23:59:33 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c49be1b95c6f947e8aaed6708b2c0b38ea78e63b117ac389af00cca5f95334f`  
		Last Modified: Wed, 08 Mar 2023 00:18:51 GMT  
		Size: 4.2 MB (4160310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1cd39813132ad141affe91c6d7f78654e7dbe1e8454baf43e2ee60f2480ecd`  
		Last Modified: Wed, 08 Mar 2023 00:18:51 GMT  
		Size: 1.2 MB (1166071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6624093c59eca00c1b574cd2672bb86cf72a602c484c89dd864ab09d28d875b`  
		Last Modified: Wed, 08 Mar 2023 00:18:50 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:35dc985cc319ba4cd38b0f28d82ec4af14971a9336ce7870444c023c1415fa7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126524974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:822857d40d7e456ebf6b4405bd126f6499dd89ce092e55728fa8deaea4601da8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 02:15:04 GMT
RUN apk add --no-cache ca-certificates
# Thu, 02 Mar 2023 02:15:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 02:19:52 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 02 Mar 2023 02:21:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 02 Mar 2023 02:21:35 GMT
ENV GOPATH=/go
# Thu, 02 Mar 2023 02:21:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 02:21:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 02 Mar 2023 02:21:35 GMT
WORKDIR /go
# Thu, 02 Mar 2023 10:40:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 02 Mar 2023 10:40:26 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_SETCAP=1
# Thu, 02 Mar 2023 10:40:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 02 Mar 2023 10:40:28 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 02 Mar 2023 10:40:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4962ca8504034f69427a90f2b07cfde1e4c20297e4507d5620bb7ea27e646919`  
		Last Modified: Thu, 02 Mar 2023 02:26:02 GMT  
		Size: 285.4 KB (285445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20059bad54d9966d7995685d0c72ce1566c6370b4105df472360f5d2c8ecd21`  
		Last Modified: Thu, 02 Mar 2023 02:28:31 GMT  
		Size: 118.5 MB (118477876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4d49a4d60a68cc1326493b7f8b4cf548d4cec1694b7ccb266f06e4028b501d`  
		Last Modified: Thu, 02 Mar 2023 02:28:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0098f26d1429a39f7d8f6dd18417972d79d6706e530dbfbc4cf9991ff98f3c6`  
		Last Modified: Thu, 02 Mar 2023 10:41:22 GMT  
		Size: 3.7 MB (3729269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0aafe51cc793a860e8c2f2c4799c11f9bebe521643a6f6578f348ce06ae80d`  
		Last Modified: Thu, 02 Mar 2023 10:41:22 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24f3750a2b57fead59e3d812fa66ae7c79703a8a84d41670403b9dc7c23eb90`  
		Last Modified: Thu, 02 Mar 2023 10:41:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6e43472efedad7b414f4cce21a50e04578ea8527ad05ee901ba9eabc88d7718e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125849779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62beb7ef29ce475cb1f571275d3c9ac33185ec48844366ef16a99e8540239b2b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:38:33 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:38:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:43:17 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:44:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:44:26 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:44:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:44:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:44:27 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:06:06 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:06:06 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:06:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:06:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:06:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55522c79112429742fe76c795b9509c5cd1e8198e0caa2a1e355c0e60a719576`  
		Last Modified: Fri, 10 Feb 2023 22:44:19 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1815dcbf43e87e122cc76a24663b7c0d6e01ad03c3be30a7dc13c1bf941c595`  
		Last Modified: Tue, 07 Mar 2023 23:49:19 GMT  
		Size: 116.9 MB (116933985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5aad4e0c6f77e535fe5a51a211a4691a5002a111c52fa17708cf1bc7c01879`  
		Last Modified: Tue, 07 Mar 2023 23:49:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557acb83c53566587727172247e84b25f860b606c200b1fc863eafc75d6b0cf4`  
		Last Modified: Wed, 08 Mar 2023 00:06:29 GMT  
		Size: 4.2 MB (4243285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb71700cd911a18f7eb1f75d651639bc79bda4000e2f4e6a8afe570b03816eb`  
		Last Modified: Wed, 08 Mar 2023 00:06:29 GMT  
		Size: 1.1 MB (1123733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358517d9544ce3184d74860b7f2054339481407b928bb11ccbf7d35163006788`  
		Last Modified: Wed, 08 Mar 2023 00:06:28 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:8126a0d2b7cc9613f70b6b5375c14cc61dfca5dc1b83adc5be33efab8eacc69f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126579575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2da1cd24f35f4106a8a7176a2f2b5656a22982a1787b9204d3eaab9ec535ef58`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:40:13 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:40:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:46:09 GMT
ENV GOLANG_VERSION=1.19.6
# Tue, 14 Feb 2023 19:48:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 14 Feb 2023 19:48:44 GMT
ENV GOPATH=/go
# Tue, 14 Feb 2023 19:48:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:48:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Feb 2023 19:48:46 GMT
WORKDIR /go
# Tue, 14 Feb 2023 20:12:48 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 14 Feb 2023 20:12:48 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 15 Feb 2023 19:16:53 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 15 Feb 2023 19:16:54 GMT
ENV XCADDY_SETCAP=1
# Wed, 15 Feb 2023 19:16:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 15 Feb 2023 19:16:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 15 Feb 2023 19:16:57 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788962e1689dbb14c760601cbf633ae350e98e3a045f8010924cd585de6b6a3e`  
		Last Modified: Fri, 10 Feb 2023 22:53:32 GMT  
		Size: 286.6 KB (286645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ae39b9ad00c218f9156f0958fa48f3062eb5830b791b8592e5f25fd576c7c5`  
		Last Modified: Tue, 14 Feb 2023 19:56:18 GMT  
		Size: 117.3 MB (117316160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f3bf55d586b31bb5c97f2cbf5167fd359b61336f93bed839c2f4de055ced88`  
		Last Modified: Tue, 14 Feb 2023 19:55:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e012d53123423a5fe128ab31d41596d83d8e48699ad608e9eb58dd0b2322fe0`  
		Last Modified: Tue, 14 Feb 2023 20:13:35 GMT  
		Size: 4.5 MB (4479556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90177e6cf58218f094608b8401f41d0da78a0cf57d95718e48e8c6e2f77c6fae`  
		Last Modified: Wed, 15 Feb 2023 19:18:00 GMT  
		Size: 1.1 MB (1105899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e897949e5a46b09b4606d86b20ecb5684cb43f7e1bed1f208ee9b7e93d208c`  
		Last Modified: Wed, 15 Feb 2023 19:17:59 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:8c80a3ba9211715e4a4892ab129d736ec6405a52630b14b828837b7307115c02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129610728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e05d79b3ea15e4e9b6f3f1a89c9e9b9580f66c78fcef17624a8c7bb9f3f51cb5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:27:44 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:27:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:47:03 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:48:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:48:53 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:48:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:48:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:48:53 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:10:01 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:10:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:10:01 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:10:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:10:02 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:10:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:10:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:10:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affa53ed2f1b70a83e3a15cae881ca47cd40f6ac11060717cdbbd4e405f9d586`  
		Last Modified: Fri, 10 Feb 2023 22:37:18 GMT  
		Size: 285.0 KB (285032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d83de48b90cbc8ae74a05d0af343e28f82727b9797b0b45ed9a70fa837a9a5`  
		Last Modified: Tue, 07 Mar 2023 23:53:54 GMT  
		Size: 120.8 MB (120808046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d22668a5d7432e1f8abda37a563ffa67f01cd8658b3247b89a7770eb41fe2a0`  
		Last Modified: Tue, 07 Mar 2023 23:53:38 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3beeef51570794945ced834a4af09db492ac50aadef9f4120ccc6b1dcb4f1251`  
		Last Modified: Wed, 08 Mar 2023 00:10:47 GMT  
		Size: 4.2 MB (4171573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57140a7518a2548d3fd2cef1ecb24c3b4ffb6aee2cc51f3921cb5497bf0863ce`  
		Last Modified: Wed, 08 Mar 2023 00:10:38 GMT  
		Size: 1.2 MB (1170402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe35434ab4b6dfcd2742bd2454af4cb9fe85cc900cacf2e2ef375861498fa09e`  
		Last Modified: Wed, 08 Mar 2023 00:10:38 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.4010; amd64

```console
$ docker pull caddy@sha256:698c8dda106fb34e783e5030fd3ea5166df618f08c2a01204a7a82aabf6b20c9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2148348831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cee813843af987f6985470a05839367529db056040844b778343ebd71743f6a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 23:47:41 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Feb 2023 23:47:42 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Feb 2023 23:47:43 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Feb 2023 23:47:44 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Feb 2023 23:50:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Feb 2023 23:50:19 GMT
ENV GOPATH=C:\go
# Wed, 15 Feb 2023 23:51:42 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Feb 2023 00:11:44 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 16 Feb 2023 00:17:12 GMT
RUN $url = 'https://dl.google.com/go/go1.19.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '8d84af29e46c38b1eec77f9310310517c9e394ac7489e1c7329a94b443b0388d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Feb 2023 00:17:13 GMT
WORKDIR C:\go
# Thu, 16 Feb 2023 02:48:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:48:16 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Feb 2023 02:48:17 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:48:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Feb 2023 02:49:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Feb 2023 02:49:37 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03ac75ee62e05ad7b8b8f97fb78a769177c49d210eedcf0a93035e9a07d0ff2`  
		Last Modified: Thu, 16 Feb 2023 00:28:24 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4beb360c9024340aa5072ce67eab6b3cb005293938525c4f3b77c3bb03f9f501`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5051ce7a895da09ac63e7ca01ef4e30434d833dbd271107d6f96375f291752ad`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea419e1594fbbef3584b4731c356499c7b8a5616af16968e6fd693eccd92012b`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb97c6a047d2cfcb6f0ef6846e78c4d5f60212639a9d1892e2af05033c217df`  
		Last Modified: Thu, 16 Feb 2023 00:28:30 GMT  
		Size: 25.6 MB (25606151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941d25224d4bab25ba0b2304a5811b0fc2970ba6385afdbefbfec898720c3beb`  
		Last Modified: Thu, 16 Feb 2023 00:28:17 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa161895f771062e6d8e8aa2e0e44c15c5affdacc8d409f6e70f1fa743a9bb1`  
		Last Modified: Thu, 16 Feb 2023 00:28:17 GMT  
		Size: 335.6 KB (335550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd14ed3be87ab223f1391d40c3cdcfcee876586e89fbeed2aeccb318734a22`  
		Last Modified: Thu, 16 Feb 2023 00:32:40 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddec1d087c619cf7156e3dba04dd6a73e704d66c60e3fbc4b32c73b4401471b`  
		Last Modified: Thu, 16 Feb 2023 00:33:24 GMT  
		Size: 157.8 MB (157798436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50612066f9b2d86b5cecd95ce6897d89929be6a819c3de13dd9ecc32948832cb`  
		Last Modified: Thu, 16 Feb 2023 00:32:40 GMT  
		Size: 1.5 KB (1544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3bbcb2df900a9ead208e08eefd6faa32bbd6c5a189212d97b94eec1e5807a24`  
		Last Modified: Thu, 16 Feb 2023 02:51:49 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b5e7db448c55e5e60ab1aefceb414700fb99de06cc1c047404e32031064e0c`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7af0982eb604918cfaece327a35d278b59d5f2ca440882b5e7d402e7cce80f6`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad49ef8883b47edaa38ca21b422551a4da50f675370fc1596432938cd7de4d2`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce066417e925c257e21d7126cbbdcf5316022725a7ef7a89575b86fd534d133f`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.6 MB (1632671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbe58e4b6c6b7d8f16c2682325b6df5f61050915e6af7829adab49c1914e5c9`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.20348.1547; amd64

```console
$ docker pull caddy@sha256:21d50bd59eead7016b606e72f6dede55b7f2c718f306c823f3a34ef794622aa7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1865665598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f3a334b2d908beba62aa4ea43b950f4be8fa2261a29819fecc52e58eaadf2df`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 23:42:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Feb 2023 23:42:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Feb 2023 23:42:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Feb 2023 23:42:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Feb 2023 23:43:27 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Feb 2023 23:43:28 GMT
ENV GOPATH=C:\go
# Wed, 15 Feb 2023 23:44:03 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Feb 2023 00:07:02 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 16 Feb 2023 00:11:25 GMT
RUN $url = 'https://dl.google.com/go/go1.19.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '8d84af29e46c38b1eec77f9310310517c9e394ac7489e1c7329a94b443b0388d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Feb 2023 00:11:27 GMT
WORKDIR C:\go
# Thu, 16 Feb 2023 02:49:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:49:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Feb 2023 02:49:47 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:49:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Feb 2023 02:50:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Feb 2023 02:50:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4048a86b3278e59b840ad06b4cf5f5888ce1068d503522a95eb470d5126ed69a`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b07973952171f91c05aade363f3e6c9a2e84548f33eaa3c8e48632460e61f8`  
		Last Modified: Thu, 16 Feb 2023 00:26:45 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a95dff10905572b5f9177959a5a9f60a9364e1dd627ed52e34ec4bee3fb3069`  
		Last Modified: Thu, 16 Feb 2023 00:26:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4267caf437f5a3d92235ab7b8d55b2c812744f166725151ba701aef9d682c6e9`  
		Last Modified: Thu, 16 Feb 2023 00:26:41 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982a959ece2e33bce3f35c5c0adb01a3426c92111b309c15f8cc31200ebcf899`  
		Last Modified: Thu, 16 Feb 2023 00:26:54 GMT  
		Size: 25.9 MB (25852811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065416c07c5d80f7a085e0e84237051d7050a71103cc9d7fb6d5ef57725dc4c6`  
		Last Modified: Thu, 16 Feb 2023 00:26:39 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07015cae66c7ebb6b0adce2dfe424313b228bb703ac3e900deebe74ae961bb49`  
		Last Modified: Thu, 16 Feb 2023 00:26:40 GMT  
		Size: 571.7 KB (571672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285847798b3738c8863954b395d2e44410be1004e9f8513dd1546a0713f153d3`  
		Last Modified: Thu, 16 Feb 2023 00:31:40 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4f6797c9312e8b2093037565c19561d6152cca51a84614b32c0813526f219f`  
		Last Modified: Thu, 16 Feb 2023 00:32:31 GMT  
		Size: 158.0 MB (158008192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2bd8446758388c6c8ddb5d51dd63d25a0dbf5c8e1385928c5e64c83948d966`  
		Last Modified: Thu, 16 Feb 2023 00:31:40 GMT  
		Size: 1.6 KB (1561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd741098e5131c0452f3451d13ce2b131c36cbfcf24df5fbd2fb9e5751e85627`  
		Last Modified: Thu, 16 Feb 2023 02:52:08 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcd5d2a85aea028cd55d32ae579beb21aa5efc8eb3875d901dfcb623092327a`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f63b7e14eef097ca8f36e589d8d609a276d3196875467da71a714db6c8e583`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2e98e1ab65293643e4b2173a01d386c2129bf22ffaee5d1b730f19a26759a7`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15030494f30adf45739bdc5e411e1ae7ea0395ebcb4c2a4f74eedbc5f71d3acd`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.9 MB (1868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba874cf328299688fd26dd5261c439698422f93ce708e583e0e248444622caff`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:68f552074b7668f5c49a7545bad89568f46b134851ee4bb7f558fe6b2e7b7749
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
$ docker pull caddy@sha256:47722ffc694507be1e2f34ca172e292fb5e226ea68d87871300b9d65f543fcce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131421587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4674ac67a52f4d29bc8349e9dcca7db8393d778c97c79d9e2f6e997603a99cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 08:21:54 GMT
RUN apk add --no-cache ca-certificates
# Sat, 11 Feb 2023 08:21:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:24:10 GMT
ENV GOLANG_VERSION=1.19.6
# Tue, 14 Feb 2023 19:25:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 14 Feb 2023 19:25:43 GMT
ENV GOPATH=/go
# Tue, 14 Feb 2023 19:25:43 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:25:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Feb 2023 19:25:44 GMT
WORKDIR /go
# Tue, 14 Feb 2023 19:47:10 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 14 Feb 2023 19:47:10 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 15 Feb 2023 19:19:27 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:19:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 15 Feb 2023 19:19:28 GMT
ENV XCADDY_SETCAP=1
# Wed, 15 Feb 2023 19:19:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 15 Feb 2023 19:19:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 15 Feb 2023 19:19:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d21d5440ebff5aaaaeb115a003f7a4a3897f1866a87de95bc4a21436fc563c`  
		Last Modified: Sat, 11 Feb 2023 08:29:10 GMT  
		Size: 284.8 KB (284816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f790f4c5274f100158d4c23bc5eddf659c1fe93ef4025488f9493d88f1490d88`  
		Last Modified: Tue, 14 Feb 2023 19:31:12 GMT  
		Size: 122.4 MB (122355677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bf170fd9e6726c86c0d4b478d9ec522e82c527a8e708668f48233a4d03f618`  
		Last Modified: Tue, 14 Feb 2023 19:30:55 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a5d1c1b6ed103f8c7f97c73ed546ff7e767b10473b55c15c0d4e1a13a69481`  
		Last Modified: Tue, 14 Feb 2023 19:47:34 GMT  
		Size: 4.2 MB (4188243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0130eaa2f0b1f7646719d82927743bd84c83ed450eb8be4db5327d280d5e4d0`  
		Last Modified: Wed, 15 Feb 2023 19:20:05 GMT  
		Size: 1.2 MB (1217841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab1f57409241476a86d26944527bc2c6c3903eadb21221b8d96da52120b3109`  
		Last Modified: Wed, 15 Feb 2023 19:20:05 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e2b8479c011649b6d47ead7051ebf36d10e2c764f2bc3bc507eab00a1812b6a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127455561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7351cc9a113eeb1deb8afa4c19e381df6b5e03cfef4e63e47bfe99f0b43d95ab`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:28 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Fri, 10 Feb 2023 20:49:28 GMT
CMD ["/bin/sh"]
# Tue, 07 Mar 2023 23:49:29 GMT
RUN apk add --no-cache ca-certificates
# Tue, 07 Mar 2023 23:49:29 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:53:43 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:55:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:55:31 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:55:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:55:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:55:32 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:17:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:17:50 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:17:50 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:17:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:17:51 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:17:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:17:52 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:17:52 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06dc45fa3a2f6e0270fe56d6b9f8efada3c9b5854707b52fe42dd55844fb1d5`  
		Last Modified: Tue, 07 Mar 2023 23:58:16 GMT  
		Size: 286.2 KB (286214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9c435c140baf308bcd21b10be4fe27e2cec5ec2acccb0cba35e7ec207d54ae`  
		Last Modified: Tue, 07 Mar 2023 23:59:54 GMT  
		Size: 118.7 MB (118731518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f756f642eb6722bcddfd36a868987c31f5583a7bac2ccf573f8c4fc55198ad49`  
		Last Modified: Tue, 07 Mar 2023 23:59:33 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c49be1b95c6f947e8aaed6708b2c0b38ea78e63b117ac389af00cca5f95334f`  
		Last Modified: Wed, 08 Mar 2023 00:18:51 GMT  
		Size: 4.2 MB (4160310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1cd39813132ad141affe91c6d7f78654e7dbe1e8454baf43e2ee60f2480ecd`  
		Last Modified: Wed, 08 Mar 2023 00:18:51 GMT  
		Size: 1.2 MB (1166071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6624093c59eca00c1b574cd2672bb86cf72a602c484c89dd864ab09d28d875b`  
		Last Modified: Wed, 08 Mar 2023 00:18:50 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:35dc985cc319ba4cd38b0f28d82ec4af14971a9336ce7870444c023c1415fa7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126524974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:822857d40d7e456ebf6b4405bd126f6499dd89ce092e55728fa8deaea4601da8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 02:15:04 GMT
RUN apk add --no-cache ca-certificates
# Thu, 02 Mar 2023 02:15:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 02:19:52 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 02 Mar 2023 02:21:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 02 Mar 2023 02:21:35 GMT
ENV GOPATH=/go
# Thu, 02 Mar 2023 02:21:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 02:21:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 02 Mar 2023 02:21:35 GMT
WORKDIR /go
# Thu, 02 Mar 2023 10:40:26 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 02 Mar 2023 10:40:26 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 02 Mar 2023 10:40:26 GMT
ENV XCADDY_SETCAP=1
# Thu, 02 Mar 2023 10:40:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 02 Mar 2023 10:40:28 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 02 Mar 2023 10:40:28 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4962ca8504034f69427a90f2b07cfde1e4c20297e4507d5620bb7ea27e646919`  
		Last Modified: Thu, 02 Mar 2023 02:26:02 GMT  
		Size: 285.4 KB (285445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20059bad54d9966d7995685d0c72ce1566c6370b4105df472360f5d2c8ecd21`  
		Last Modified: Thu, 02 Mar 2023 02:28:31 GMT  
		Size: 118.5 MB (118477876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4d49a4d60a68cc1326493b7f8b4cf548d4cec1694b7ccb266f06e4028b501d`  
		Last Modified: Thu, 02 Mar 2023 02:28:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0098f26d1429a39f7d8f6dd18417972d79d6706e530dbfbc4cf9991ff98f3c6`  
		Last Modified: Thu, 02 Mar 2023 10:41:22 GMT  
		Size: 3.7 MB (3729269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0aafe51cc793a860e8c2f2c4799c11f9bebe521643a6f6578f348ce06ae80d`  
		Last Modified: Thu, 02 Mar 2023 10:41:22 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24f3750a2b57fead59e3d812fa66ae7c79703a8a84d41670403b9dc7c23eb90`  
		Last Modified: Thu, 02 Mar 2023 10:41:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6e43472efedad7b414f4cce21a50e04578ea8527ad05ee901ba9eabc88d7718e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125849779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62beb7ef29ce475cb1f571275d3c9ac33185ec48844366ef16a99e8540239b2b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:38:33 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:38:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:43:17 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:44:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:44:26 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:44:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:44:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:44:27 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:06:06 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:06:06 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:06:06 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:06:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:06:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:06:08 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55522c79112429742fe76c795b9509c5cd1e8198e0caa2a1e355c0e60a719576`  
		Last Modified: Fri, 10 Feb 2023 22:44:19 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1815dcbf43e87e122cc76a24663b7c0d6e01ad03c3be30a7dc13c1bf941c595`  
		Last Modified: Tue, 07 Mar 2023 23:49:19 GMT  
		Size: 116.9 MB (116933985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5aad4e0c6f77e535fe5a51a211a4691a5002a111c52fa17708cf1bc7c01879`  
		Last Modified: Tue, 07 Mar 2023 23:49:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557acb83c53566587727172247e84b25f860b606c200b1fc863eafc75d6b0cf4`  
		Last Modified: Wed, 08 Mar 2023 00:06:29 GMT  
		Size: 4.2 MB (4243285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb71700cd911a18f7eb1f75d651639bc79bda4000e2f4e6a8afe570b03816eb`  
		Last Modified: Wed, 08 Mar 2023 00:06:29 GMT  
		Size: 1.1 MB (1123733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358517d9544ce3184d74860b7f2054339481407b928bb11ccbf7d35163006788`  
		Last Modified: Wed, 08 Mar 2023 00:06:28 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:8126a0d2b7cc9613f70b6b5375c14cc61dfca5dc1b83adc5be33efab8eacc69f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126579575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2da1cd24f35f4106a8a7176a2f2b5656a22982a1787b9204d3eaab9ec535ef58`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:40:13 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:40:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:46:09 GMT
ENV GOLANG_VERSION=1.19.6
# Tue, 14 Feb 2023 19:48:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.6.src.tar.gz'; 		sha256='d7f0013f82e6d7f862cc6cb5c8cdb48eef5f2e239b35baa97e2f1a7466043767'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 14 Feb 2023 19:48:44 GMT
ENV GOPATH=/go
# Tue, 14 Feb 2023 19:48:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Feb 2023 19:48:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 14 Feb 2023 19:48:46 GMT
WORKDIR /go
# Tue, 14 Feb 2023 20:12:48 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 14 Feb 2023 20:12:48 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 15 Feb 2023 19:16:53 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 15 Feb 2023 19:16:54 GMT
ENV XCADDY_SETCAP=1
# Wed, 15 Feb 2023 19:16:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 15 Feb 2023 19:16:56 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 15 Feb 2023 19:16:57 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788962e1689dbb14c760601cbf633ae350e98e3a045f8010924cd585de6b6a3e`  
		Last Modified: Fri, 10 Feb 2023 22:53:32 GMT  
		Size: 286.6 KB (286645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ae39b9ad00c218f9156f0958fa48f3062eb5830b791b8592e5f25fd576c7c5`  
		Last Modified: Tue, 14 Feb 2023 19:56:18 GMT  
		Size: 117.3 MB (117316160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f3bf55d586b31bb5c97f2cbf5167fd359b61336f93bed839c2f4de055ced88`  
		Last Modified: Tue, 14 Feb 2023 19:55:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e012d53123423a5fe128ab31d41596d83d8e48699ad608e9eb58dd0b2322fe0`  
		Last Modified: Tue, 14 Feb 2023 20:13:35 GMT  
		Size: 4.5 MB (4479556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90177e6cf58218f094608b8401f41d0da78a0cf57d95718e48e8c6e2f77c6fae`  
		Last Modified: Wed, 15 Feb 2023 19:18:00 GMT  
		Size: 1.1 MB (1105899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e897949e5a46b09b4606d86b20ecb5684cb43f7e1bed1f208ee9b7e93d208c`  
		Last Modified: Wed, 15 Feb 2023 19:17:59 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:8c80a3ba9211715e4a4892ab129d736ec6405a52630b14b828837b7307115c02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129610728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e05d79b3ea15e4e9b6f3f1a89c9e9b9580f66c78fcef17624a8c7bb9f3f51cb5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:27:44 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:27:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:47:03 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:48:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:48:53 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:48:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:48:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 07 Mar 2023 23:48:53 GMT
WORKDIR /go
# Wed, 08 Mar 2023 00:10:01 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Mar 2023 00:10:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Mar 2023 00:10:01 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:10:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Mar 2023 00:10:02 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Mar 2023 00:10:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Mar 2023 00:10:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Mar 2023 00:10:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affa53ed2f1b70a83e3a15cae881ca47cd40f6ac11060717cdbbd4e405f9d586`  
		Last Modified: Fri, 10 Feb 2023 22:37:18 GMT  
		Size: 285.0 KB (285032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d83de48b90cbc8ae74a05d0af343e28f82727b9797b0b45ed9a70fa837a9a5`  
		Last Modified: Tue, 07 Mar 2023 23:53:54 GMT  
		Size: 120.8 MB (120808046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d22668a5d7432e1f8abda37a563ffa67f01cd8658b3247b89a7770eb41fe2a0`  
		Last Modified: Tue, 07 Mar 2023 23:53:38 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3beeef51570794945ced834a4af09db492ac50aadef9f4120ccc6b1dcb4f1251`  
		Last Modified: Wed, 08 Mar 2023 00:10:47 GMT  
		Size: 4.2 MB (4171573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57140a7518a2548d3fd2cef1ecb24c3b4ffb6aee2cc51f3921cb5497bf0863ce`  
		Last Modified: Wed, 08 Mar 2023 00:10:38 GMT  
		Size: 1.2 MB (1170402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe35434ab4b6dfcd2742bd2454af4cb9fe85cc900cacf2e2ef375861498fa09e`  
		Last Modified: Wed, 08 Mar 2023 00:10:38 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:687ff9a9e85091470e7d84be08a4e96d119290226bfcd464502138db4b9f1542
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4010; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.4010; amd64

```console
$ docker pull caddy@sha256:698c8dda106fb34e783e5030fd3ea5166df618f08c2a01204a7a82aabf6b20c9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2148348831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cee813843af987f6985470a05839367529db056040844b778343ebd71743f6a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 23:47:41 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Feb 2023 23:47:42 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Feb 2023 23:47:43 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Feb 2023 23:47:44 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Feb 2023 23:50:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Feb 2023 23:50:19 GMT
ENV GOPATH=C:\go
# Wed, 15 Feb 2023 23:51:42 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Feb 2023 00:11:44 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 16 Feb 2023 00:17:12 GMT
RUN $url = 'https://dl.google.com/go/go1.19.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '8d84af29e46c38b1eec77f9310310517c9e394ac7489e1c7329a94b443b0388d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Feb 2023 00:17:13 GMT
WORKDIR C:\go
# Thu, 16 Feb 2023 02:48:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:48:16 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Feb 2023 02:48:17 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:48:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Feb 2023 02:49:36 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Feb 2023 02:49:37 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03ac75ee62e05ad7b8b8f97fb78a769177c49d210eedcf0a93035e9a07d0ff2`  
		Last Modified: Thu, 16 Feb 2023 00:28:24 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4beb360c9024340aa5072ce67eab6b3cb005293938525c4f3b77c3bb03f9f501`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5051ce7a895da09ac63e7ca01ef4e30434d833dbd271107d6f96375f291752ad`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea419e1594fbbef3584b4731c356499c7b8a5616af16968e6fd693eccd92012b`  
		Last Modified: Thu, 16 Feb 2023 00:28:19 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb97c6a047d2cfcb6f0ef6846e78c4d5f60212639a9d1892e2af05033c217df`  
		Last Modified: Thu, 16 Feb 2023 00:28:30 GMT  
		Size: 25.6 MB (25606151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941d25224d4bab25ba0b2304a5811b0fc2970ba6385afdbefbfec898720c3beb`  
		Last Modified: Thu, 16 Feb 2023 00:28:17 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa161895f771062e6d8e8aa2e0e44c15c5affdacc8d409f6e70f1fa743a9bb1`  
		Last Modified: Thu, 16 Feb 2023 00:28:17 GMT  
		Size: 335.6 KB (335550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bd14ed3be87ab223f1391d40c3cdcfcee876586e89fbeed2aeccb318734a22`  
		Last Modified: Thu, 16 Feb 2023 00:32:40 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddec1d087c619cf7156e3dba04dd6a73e704d66c60e3fbc4b32c73b4401471b`  
		Last Modified: Thu, 16 Feb 2023 00:33:24 GMT  
		Size: 157.8 MB (157798436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50612066f9b2d86b5cecd95ce6897d89929be6a819c3de13dd9ecc32948832cb`  
		Last Modified: Thu, 16 Feb 2023 00:32:40 GMT  
		Size: 1.5 KB (1544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3bbcb2df900a9ead208e08eefd6faa32bbd6c5a189212d97b94eec1e5807a24`  
		Last Modified: Thu, 16 Feb 2023 02:51:49 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b5e7db448c55e5e60ab1aefceb414700fb99de06cc1c047404e32031064e0c`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7af0982eb604918cfaece327a35d278b59d5f2ca440882b5e7d402e7cce80f6`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad49ef8883b47edaa38ca21b422551a4da50f675370fc1596432938cd7de4d2`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce066417e925c257e21d7126cbbdcf5316022725a7ef7a89575b86fd534d133f`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.6 MB (1632671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbe58e4b6c6b7d8f16c2682325b6df5f61050915e6af7829adab49c1914e5c9`  
		Last Modified: Thu, 16 Feb 2023 02:51:47 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:573ab227ac93b402974ef9c7f039983bc070f5e08c73d21e62345c13f8ccbaab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `caddy:builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1547; amd64

```console
$ docker pull caddy@sha256:21d50bd59eead7016b606e72f6dede55b7f2c718f306c823f3a34ef794622aa7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1865665598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f3a334b2d908beba62aa4ea43b950f4be8fa2261a29819fecc52e58eaadf2df`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 23:42:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 15 Feb 2023 23:42:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 15 Feb 2023 23:42:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 15 Feb 2023 23:42:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 15 Feb 2023 23:43:27 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 15 Feb 2023 23:43:28 GMT
ENV GOPATH=C:\go
# Wed, 15 Feb 2023 23:44:03 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Feb 2023 00:07:02 GMT
ENV GOLANG_VERSION=1.19.6
# Thu, 16 Feb 2023 00:11:25 GMT
RUN $url = 'https://dl.google.com/go/go1.19.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '8d84af29e46c38b1eec77f9310310517c9e394ac7489e1c7329a94b443b0388d'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Feb 2023 00:11:27 GMT
WORKDIR C:\go
# Thu, 16 Feb 2023 02:49:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:49:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Feb 2023 02:49:47 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:49:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Feb 2023 02:50:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Feb 2023 02:50:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4048a86b3278e59b840ad06b4cf5f5888ce1068d503522a95eb470d5126ed69a`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b07973952171f91c05aade363f3e6c9a2e84548f33eaa3c8e48632460e61f8`  
		Last Modified: Thu, 16 Feb 2023 00:26:45 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a95dff10905572b5f9177959a5a9f60a9364e1dd627ed52e34ec4bee3fb3069`  
		Last Modified: Thu, 16 Feb 2023 00:26:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4267caf437f5a3d92235ab7b8d55b2c812744f166725151ba701aef9d682c6e9`  
		Last Modified: Thu, 16 Feb 2023 00:26:41 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982a959ece2e33bce3f35c5c0adb01a3426c92111b309c15f8cc31200ebcf899`  
		Last Modified: Thu, 16 Feb 2023 00:26:54 GMT  
		Size: 25.9 MB (25852811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065416c07c5d80f7a085e0e84237051d7050a71103cc9d7fb6d5ef57725dc4c6`  
		Last Modified: Thu, 16 Feb 2023 00:26:39 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07015cae66c7ebb6b0adce2dfe424313b228bb703ac3e900deebe74ae961bb49`  
		Last Modified: Thu, 16 Feb 2023 00:26:40 GMT  
		Size: 571.7 KB (571672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285847798b3738c8863954b395d2e44410be1004e9f8513dd1546a0713f153d3`  
		Last Modified: Thu, 16 Feb 2023 00:31:40 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4f6797c9312e8b2093037565c19561d6152cca51a84614b32c0813526f219f`  
		Last Modified: Thu, 16 Feb 2023 00:32:31 GMT  
		Size: 158.0 MB (158008192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2bd8446758388c6c8ddb5d51dd63d25a0dbf5c8e1385928c5e64c83948d966`  
		Last Modified: Thu, 16 Feb 2023 00:31:40 GMT  
		Size: 1.6 KB (1561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd741098e5131c0452f3451d13ce2b131c36cbfcf24df5fbd2fb9e5751e85627`  
		Last Modified: Thu, 16 Feb 2023 02:52:08 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcd5d2a85aea028cd55d32ae579beb21aa5efc8eb3875d901dfcb623092327a`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f63b7e14eef097ca8f36e589d8d609a276d3196875467da71a714db6c8e583`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2e98e1ab65293643e4b2173a01d386c2129bf22ffaee5d1b730f19a26759a7`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15030494f30adf45739bdc5e411e1ae7ea0395ebcb4c2a4f74eedbc5f71d3acd`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.9 MB (1868121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba874cf328299688fd26dd5261c439698422f93ce708e583e0e248444622caff`  
		Last Modified: Thu, 16 Feb 2023 02:52:06 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:304185ec40295c7b7c33f98981c241d23d959fa0534eb34cd18c732fde51cd5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4010; amd64
	-	windows version 10.0.20348.1547; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:36ba71b44afa613ecf0aadce8e4b9e3f56e0c4b0a78c8edf4e8c2485f21b35ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17449113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8464e23f16f9a82426bbdc3ac8c94270a84453ddc86b9147505a2378a7c2fd0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:38:34 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 11 Feb 2023 07:38:36 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:19:21 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:19:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:19:23 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:19:24 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:19:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:19:25 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:19:25 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e3e797818bc929d95bae8220b7b6034b559c217ef5bf622dc7fedc8d270a48`  
		Last Modified: Sat, 11 Feb 2023 07:39:01 GMT  
		Size: 351.2 KB (351178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cebb4c80b3906a9b751ee9a512c1581331b1fd691c84f575c01a29e28403dde`  
		Last Modified: Sat, 11 Feb 2023 07:39:00 GMT  
		Size: 7.6 KB (7552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90648ba22c191b969d8db393bf6138e7d6ecc1b70b3865d1717ec4d663192d89`  
		Last Modified: Wed, 15 Feb 2023 19:19:52 GMT  
		Size: 14.3 MB (14282621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:db317e683b30c11665349301255c3c59f3f5b085d4e075553e445129981ad5e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16582515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4628532cad0308b1d01506925ca941dffeb3bdd058cd79ccd7f055dce243e3b6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:32 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Fri, 10 Feb 2023 20:49:32 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 00:17:32 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 08 Mar 2023 00:17:34 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 08 Mar 2023 00:17:34 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 08 Mar 2023 00:17:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 08 Mar 2023 00:17:38 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 08 Mar 2023 00:17:39 GMT
ENV XDG_DATA_HOME=/data
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 08 Mar 2023 00:17:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 08 Mar 2023 00:17:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 08 Mar 2023 00:17:41 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 80
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 443
# Wed, 08 Mar 2023 00:17:41 GMT
EXPOSE 443/udp
# Wed, 08 Mar 2023 00:17:42 GMT
EXPOSE 2019
# Wed, 08 Mar 2023 00:17:42 GMT
WORKDIR /srv
# Wed, 08 Mar 2023 00:17:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e676ebf894f684676e3a3c92294bbc14ba7061c7d24285909e673075903c39a9`  
		Last Modified: Wed, 08 Mar 2023 00:18:32 GMT  
		Size: 345.9 KB (345903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b146a16f288a28f362ad572b56958616fb5f4e0572bbe406ce18868be0d5c3`  
		Last Modified: Wed, 08 Mar 2023 00:18:31 GMT  
		Size: 7.6 KB (7559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e662de32a44a67eae886e653355902b11fec7407264122f1e72b5c460cb4334`  
		Last Modified: Wed, 08 Mar 2023 00:18:34 GMT  
		Size: 13.6 MB (13612275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:03b5f2d631567d2783e8977e4988bdc75f13acb5c5b7bb18f3984045fb557b11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16365710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bed848976d2f2ce06398c52bf359363302bd512c4c51f08acb50cdd7ec0db5a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 10:40:15 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 02 Mar 2023 10:40:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 02 Mar 2023 10:40:16 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 02 Mar 2023 10:40:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 02 Mar 2023 10:40:19 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 02 Mar 2023 10:40:19 GMT
ENV XDG_DATA_HOME=/data
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 02 Mar 2023 10:40:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 02 Mar 2023 10:40:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 02 Mar 2023 10:40:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 80
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 443
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 443/udp
# Thu, 02 Mar 2023 10:40:20 GMT
EXPOSE 2019
# Thu, 02 Mar 2023 10:40:20 GMT
WORKDIR /srv
# Thu, 02 Mar 2023 10:40:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769efc94ebb1351d7f88e191e0e5c768fc2462e89d73fa4b373005e8a912f367`  
		Last Modified: Thu, 02 Mar 2023 10:41:04 GMT  
		Size: 342.7 KB (342688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fb7d44b5e1d66fb60d8593e306cfef844841aca960cacb7258951888fcf79e`  
		Last Modified: Thu, 02 Mar 2023 10:41:04 GMT  
		Size: 7.6 KB (7560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818d68e9d461fbb298a8bb8f5467049d89e77e6324f72842c3d45e5af3d0767b`  
		Last Modified: Thu, 02 Mar 2023 10:41:06 GMT  
		Size: 13.6 MB (13594968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6c2623f6bf30798be5c37fc7484e45ecc288d493fb657883f59ddb27ed714ad8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16130997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a38afdc517ef4cff6b6b51a1c6a633c2826599b07feb1e88380d0f783e35cf1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:00:35 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:00:37 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 18:39:20 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 18:39:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 18:39:22 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 18:39:22 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 18:39:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 18:39:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 80
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 443
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 18:39:23 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 18:39:23 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 18:39:23 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70730e8e2fb933ec157ec87f2a4fb4ad45e8e578b8f7c76cc4846631d773554`  
		Last Modified: Fri, 10 Feb 2023 22:01:02 GMT  
		Size: 350.2 KB (350153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a4b7390d269477c225f1d03e825d2d8bdf6b4d87b5f7bb8811b341e56b7d36`  
		Last Modified: Fri, 10 Feb 2023 22:01:02 GMT  
		Size: 7.6 KB (7555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2743d2ef53ee6edb0e39c89bf16957e3a00990410b2d1a126dca1b2d196182`  
		Last Modified: Wed, 15 Feb 2023 18:39:53 GMT  
		Size: 13.1 MB (13063787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:8861ab3ae3d0c180e38142c2f7482f9ce1773419eb29ed9d6d18308246858093
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5819f0ab4928a30c29293a27299a3b44371cd3bd97df91432ef7b3f43b692d8c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:13:21 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:13:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:16:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:16:41 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:16:42 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:16:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:16:47 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:16:47 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:16:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bd0321e6539bb7dac8574fd36bad22059ef06bb63dc842165f69d0a821572`  
		Last Modified: Fri, 10 Feb 2023 22:14:16 GMT  
		Size: 363.1 KB (363088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb806b2600b0209a73fc7175ab778d0224661034b2f722bd1a0aec1eb9eabe3d`  
		Last Modified: Fri, 10 Feb 2023 22:14:15 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd7c8ae860931dd79dea76d33bc21bb11d89cd4d133cdb41078b040afc6633e`  
		Last Modified: Wed, 15 Feb 2023 19:17:41 GMT  
		Size: 12.8 MB (12779898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:4e1ed99f133abf02d6a7c77849978bb621f748e18c9cb9f7a1dbf88480ddb8d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45cd164da734310b788dcbd4f6c94bccff6e48705fe4d42ecca07a54e9459a9c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:31 GMT
ADD file:17af250b49631cf2acf655c85df90977eddab4c9afd67bda3c577db5200364f1 in / 
# Fri, 10 Feb 2023 21:41:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:14:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:14:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 18:41:48 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 18:41:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 18:41:59 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 18:41:59 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 18:42:00 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 18:42:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 18:42:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 18:42:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 18:42:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 18:42:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 18:42:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 18:42:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 18:42:05 GMT
EXPOSE 80
# Wed, 15 Feb 2023 18:42:06 GMT
EXPOSE 443
# Wed, 15 Feb 2023 18:42:07 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 18:42:07 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 18:42:08 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 18:42:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:667d93a24f321610e24486f3148545191f113ab9ab2444804087dd65ebbda9ed`  
		Last Modified: Fri, 10 Feb 2023 21:42:26 GMT  
		Size: 2.6 MB (2593581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e6ec82400496ce74e37120e1655955b79303daaa5b8ca7e956e3cd96ddd6e9`  
		Last Modified: Fri, 10 Feb 2023 22:15:05 GMT  
		Size: 352.8 KB (352801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5b992687f93ced3715ad97bd95ab37daef5685b784e195209caefbc48f14e9`  
		Last Modified: Fri, 10 Feb 2023 22:15:05 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ccc40924ce2df3343fa5465a92ccaa4ed80e0883190a99d3f468c60f9ddbcf8`  
		Last Modified: Wed, 15 Feb 2023 18:43:19 GMT  
		Size: 13.8 MB (13838817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.4010; amd64

```console
$ docker pull caddy@sha256:f78e6d4fc1641b322d4e44adcada628f9acb5106b2e166cbcba796764a4db257
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1978492183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:198e4772b4788d7810819799af107998abe8e241416654ca5406331afefc2908`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:43:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:44:00 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:45:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:45:08 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:45:09 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:45:10 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:45:11 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:45:12 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:45:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:45:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:45:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:45:17 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:45:19 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:46:11 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:46:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f19b532038d3c84c40068e825815f2b252b82869809b11745d9893f12a99ac1`  
		Last Modified: Thu, 16 Feb 2023 02:51:03 GMT  
		Size: 526.3 KB (526332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15f6c8f1e7f194b2b408bf6c4330db67cf7cd4783d39acba2d8384b2f3c31d4`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab346a52e8e98a31f0970c85a32f1653b5179dd5ad781a8764b08de792a4d99`  
		Last Modified: Thu, 16 Feb 2023 02:51:05 GMT  
		Size: 14.7 MB (14677251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4451f67396ee792e3ace473ca4a69e5e49639ab8b620e489635a7b2eeb775523`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9291ccd53cd67f009cd59c77d90d2623192e5e134fc2ad5a03f1c1860ab66b80`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3096247c037e7418f5efc50ce5c7e6bc272ccac5c014f5cb085d77c4c28a3a`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f902038f4ba892bc3e1e4d5fdcef6b7759891c41c067b744fa3d5b008776c90`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82e400c4f2072b1e2b2ff49169de3108075208b544f454b3cdf016be6356321`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0944799324319439cbaf2f01dd147e8cc496ea80243ddc22e59e301237acb293`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce6c226ffeaa8146cae1b818b43a4776a06f6ce0be460b7d9b42fcc503b39db`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0b36e09fd7994e37dd27ccdcfa4610fc1219c4044a95695c6de9f9eecda63b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f284721a924468c7a0ff80b2809a222ae20cae99d35aa761b5296272783263b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bec609c0b4d99a9726ad86662d32a57664d18dde9d9087c0695ec7e9c4a47c`  
		Last Modified: Thu, 16 Feb 2023 02:50:59 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ad796550cc1ac21dd77352cf12cc78cacbd0a9f8a1e728e7e4f6a02a0cb9fb`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1955699b7dbbfef476622c70f983565943bafe8909c80ec278dff19509fad86`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4096827c6eb36146321a048a5041be746e60afe4c8e90717d681f2d271e0143`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc99e795e3855739a0c170e77263147dec07ac66a9ae51c306705be5af6574b`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8683be90a75d0e97aa8b7002c075e040e7299bd1fde397a541df3e7e4168d97`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 308.1 KB (308099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156392510131bc65057e3573b9aa9838fccd38cc8ed89734e5255bcd4a315274`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.20348.1547; amd64

```console
$ docker pull caddy@sha256:87b9acadc87fc1f78b7ee864f06462a0f45aa263af20fa1744e2f2a0d0870b02
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1695421581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaff43d5343d972f345ff5561ee131879eaafd463e389a1c2607715ac3f6e793`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:46:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:46:57 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:47:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:47:26 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:47:27 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:47:28 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:47:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:47:31 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:47:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:47:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:47:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:47:36 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:47:37 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:47:56 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:47:57 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1961fba6606566986ddd1960cf8309d19fa9deaa486f5a162a60114f3d4c3c82`  
		Last Modified: Thu, 16 Feb 2023 02:51:29 GMT  
		Size: 778.8 KB (778807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af5d76bf41697a16b3336a1857d1e530a3137f28d997c6f5eca0121d42ea88d`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d935f5b810851a2833b69e65d9dcff828f1c6686dab6fa117e9bd08eb95f5990`  
		Last Modified: Thu, 16 Feb 2023 02:51:31 GMT  
		Size: 14.9 MB (14914232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54e2a419181dd9257efde40f9ab80121dd6cc1a478f6ff42d160ddbf5e17cd4`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c07f1bbb0931b3148683baae55ab0d85f8576b2a1d8c2a59bb28544572b5a9d`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06073fd741cf5968f24574903b70213f9743b648ebec9c53ccb8fe114ce01ae`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a17243f1184726e21bf0821ee5984a84575b55befba72594fbf0b3a32a47f1`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c403099e0a283f6f2b25b4235c61c8b564a832643f33280253dc040d2a2ab07`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cc4608f06891b205fbec74e83a221161a2f9d9b50a0b548c3c716d176ee1a4`  
		Last Modified: Thu, 16 Feb 2023 02:51:25 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfe2ac143052b1fa8973567134244ce4ecd1693f16205dd53f0d4cf1b5caa5a`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e217159efeb187bf7ae9a12f6f70764141dd97837f24a517851bc15a36b552`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc05a7da758918922e168d1b07b29f4a81d398dc805724dd6b23b4cb28c7b43`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832768cea319f33011657944b08b51ea41229fdd7a37f21162dd8aedceb31a6b`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443fc82ac63aefa17f6de497731a007fbc972b175040388a8fda7112834af9fa`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39ff50a2c37b226c6e79e3789d1706fc47cb355b14372a147024fc11b2dfb2b`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c6037df6cbd4b9e046dded7157e841a1c40659c4dd082ff9d397c95be6e411`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a470cfe53e2d01e3ca43a7211eb050493a97f430e3c5a52e2364f54a0a4e4834`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d12a1c4350235354af8011d0b2eccb56884eea72a0475197fb007c4fa6c111`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 359.9 KB (359894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea80c894fe52045adaa4c44b9f66422259571c7aec153753d27a56aa3ccbd930`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:07fbc5a89186611e042f7ab23685ae8afbcce5678ff9b1315e742e6935052c9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4010; amd64
	-	windows version 10.0.20348.1547; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.4010; amd64

```console
$ docker pull caddy@sha256:f78e6d4fc1641b322d4e44adcada628f9acb5106b2e166cbcba796764a4db257
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1978492183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:198e4772b4788d7810819799af107998abe8e241416654ca5406331afefc2908`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:43:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:44:00 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:45:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:45:08 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:45:09 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:45:10 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:45:11 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:45:12 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:45:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:45:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:45:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:45:17 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:45:19 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:46:11 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:46:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f19b532038d3c84c40068e825815f2b252b82869809b11745d9893f12a99ac1`  
		Last Modified: Thu, 16 Feb 2023 02:51:03 GMT  
		Size: 526.3 KB (526332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15f6c8f1e7f194b2b408bf6c4330db67cf7cd4783d39acba2d8384b2f3c31d4`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab346a52e8e98a31f0970c85a32f1653b5179dd5ad781a8764b08de792a4d99`  
		Last Modified: Thu, 16 Feb 2023 02:51:05 GMT  
		Size: 14.7 MB (14677251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4451f67396ee792e3ace473ca4a69e5e49639ab8b620e489635a7b2eeb775523`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9291ccd53cd67f009cd59c77d90d2623192e5e134fc2ad5a03f1c1860ab66b80`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3096247c037e7418f5efc50ce5c7e6bc272ccac5c014f5cb085d77c4c28a3a`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f902038f4ba892bc3e1e4d5fdcef6b7759891c41c067b744fa3d5b008776c90`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82e400c4f2072b1e2b2ff49169de3108075208b544f454b3cdf016be6356321`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0944799324319439cbaf2f01dd147e8cc496ea80243ddc22e59e301237acb293`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce6c226ffeaa8146cae1b818b43a4776a06f6ce0be460b7d9b42fcc503b39db`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0b36e09fd7994e37dd27ccdcfa4610fc1219c4044a95695c6de9f9eecda63b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f284721a924468c7a0ff80b2809a222ae20cae99d35aa761b5296272783263b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bec609c0b4d99a9726ad86662d32a57664d18dde9d9087c0695ec7e9c4a47c`  
		Last Modified: Thu, 16 Feb 2023 02:50:59 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ad796550cc1ac21dd77352cf12cc78cacbd0a9f8a1e728e7e4f6a02a0cb9fb`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1955699b7dbbfef476622c70f983565943bafe8909c80ec278dff19509fad86`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4096827c6eb36146321a048a5041be746e60afe4c8e90717d681f2d271e0143`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc99e795e3855739a0c170e77263147dec07ac66a9ae51c306705be5af6574b`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8683be90a75d0e97aa8b7002c075e040e7299bd1fde397a541df3e7e4168d97`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 308.1 KB (308099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156392510131bc65057e3573b9aa9838fccd38cc8ed89734e5255bcd4a315274`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.20348.1547; amd64

```console
$ docker pull caddy@sha256:87b9acadc87fc1f78b7ee864f06462a0f45aa263af20fa1744e2f2a0d0870b02
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1695421581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaff43d5343d972f345ff5561ee131879eaafd463e389a1c2607715ac3f6e793`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:46:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:46:57 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:47:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:47:26 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:47:27 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:47:28 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:47:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:47:31 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:47:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:47:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:47:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:47:36 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:47:37 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:47:56 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:47:57 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1961fba6606566986ddd1960cf8309d19fa9deaa486f5a162a60114f3d4c3c82`  
		Last Modified: Thu, 16 Feb 2023 02:51:29 GMT  
		Size: 778.8 KB (778807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af5d76bf41697a16b3336a1857d1e530a3137f28d997c6f5eca0121d42ea88d`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d935f5b810851a2833b69e65d9dcff828f1c6686dab6fa117e9bd08eb95f5990`  
		Last Modified: Thu, 16 Feb 2023 02:51:31 GMT  
		Size: 14.9 MB (14914232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54e2a419181dd9257efde40f9ab80121dd6cc1a478f6ff42d160ddbf5e17cd4`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c07f1bbb0931b3148683baae55ab0d85f8576b2a1d8c2a59bb28544572b5a9d`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06073fd741cf5968f24574903b70213f9743b648ebec9c53ccb8fe114ce01ae`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a17243f1184726e21bf0821ee5984a84575b55befba72594fbf0b3a32a47f1`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c403099e0a283f6f2b25b4235c61c8b564a832643f33280253dc040d2a2ab07`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cc4608f06891b205fbec74e83a221161a2f9d9b50a0b548c3c716d176ee1a4`  
		Last Modified: Thu, 16 Feb 2023 02:51:25 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfe2ac143052b1fa8973567134244ce4ecd1693f16205dd53f0d4cf1b5caa5a`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e217159efeb187bf7ae9a12f6f70764141dd97837f24a517851bc15a36b552`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc05a7da758918922e168d1b07b29f4a81d398dc805724dd6b23b4cb28c7b43`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832768cea319f33011657944b08b51ea41229fdd7a37f21162dd8aedceb31a6b`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443fc82ac63aefa17f6de497731a007fbc972b175040388a8fda7112834af9fa`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39ff50a2c37b226c6e79e3789d1706fc47cb355b14372a147024fc11b2dfb2b`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c6037df6cbd4b9e046dded7157e841a1c40659c4dd082ff9d397c95be6e411`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a470cfe53e2d01e3ca43a7211eb050493a97f430e3c5a52e2364f54a0a4e4834`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d12a1c4350235354af8011d0b2eccb56884eea72a0475197fb007c4fa6c111`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 359.9 KB (359894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea80c894fe52045adaa4c44b9f66422259571c7aec153753d27a56aa3ccbd930`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:1bd6dc9cf41fc94696e73caafb13f1e2aa4080c4961ffe195303c2a51811ff9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4010; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.4010; amd64

```console
$ docker pull caddy@sha256:f78e6d4fc1641b322d4e44adcada628f9acb5106b2e166cbcba796764a4db257
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1978492183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:198e4772b4788d7810819799af107998abe8e241416654ca5406331afefc2908`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:43:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:44:00 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:45:07 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:45:08 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:45:09 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:45:10 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:45:11 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:45:12 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:45:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:45:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:45:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:45:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:45:17 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:45:18 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:45:19 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:46:11 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:46:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f19b532038d3c84c40068e825815f2b252b82869809b11745d9893f12a99ac1`  
		Last Modified: Thu, 16 Feb 2023 02:51:03 GMT  
		Size: 526.3 KB (526332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15f6c8f1e7f194b2b408bf6c4330db67cf7cd4783d39acba2d8384b2f3c31d4`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab346a52e8e98a31f0970c85a32f1653b5179dd5ad781a8764b08de792a4d99`  
		Last Modified: Thu, 16 Feb 2023 02:51:05 GMT  
		Size: 14.7 MB (14677251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4451f67396ee792e3ace473ca4a69e5e49639ab8b620e489635a7b2eeb775523`  
		Last Modified: Thu, 16 Feb 2023 02:51:02 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9291ccd53cd67f009cd59c77d90d2623192e5e134fc2ad5a03f1c1860ab66b80`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3096247c037e7418f5efc50ce5c7e6bc272ccac5c014f5cb085d77c4c28a3a`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f902038f4ba892bc3e1e4d5fdcef6b7759891c41c067b744fa3d5b008776c90`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82e400c4f2072b1e2b2ff49169de3108075208b544f454b3cdf016be6356321`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0944799324319439cbaf2f01dd147e8cc496ea80243ddc22e59e301237acb293`  
		Last Modified: Thu, 16 Feb 2023 02:51:00 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce6c226ffeaa8146cae1b818b43a4776a06f6ce0be460b7d9b42fcc503b39db`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0b36e09fd7994e37dd27ccdcfa4610fc1219c4044a95695c6de9f9eecda63b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f284721a924468c7a0ff80b2809a222ae20cae99d35aa761b5296272783263b`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bec609c0b4d99a9726ad86662d32a57664d18dde9d9087c0695ec7e9c4a47c`  
		Last Modified: Thu, 16 Feb 2023 02:50:59 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ad796550cc1ac21dd77352cf12cc78cacbd0a9f8a1e728e7e4f6a02a0cb9fb`  
		Last Modified: Thu, 16 Feb 2023 02:50:58 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1955699b7dbbfef476622c70f983565943bafe8909c80ec278dff19509fad86`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4096827c6eb36146321a048a5041be746e60afe4c8e90717d681f2d271e0143`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc99e795e3855739a0c170e77263147dec07ac66a9ae51c306705be5af6574b`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8683be90a75d0e97aa8b7002c075e040e7299bd1fde397a541df3e7e4168d97`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 308.1 KB (308099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156392510131bc65057e3573b9aa9838fccd38cc8ed89734e5255bcd4a315274`  
		Last Modified: Thu, 16 Feb 2023 02:50:56 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:bdada4aecbae3dbf7c909817361c5c5e025530a60f1017107cf4cbe628e5a12b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `caddy:windowsservercore-ltsc2022` - windows version 10.0.20348.1547; amd64

```console
$ docker pull caddy@sha256:87b9acadc87fc1f78b7ee864f06462a0f45aa263af20fa1744e2f2a0d0870b02
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1695421581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaff43d5343d972f345ff5561ee131879eaafd463e389a1c2607715ac3f6e793`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:46:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Feb 2023 02:46:57 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Feb 2023 02:47:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Feb 2023 02:47:26 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Feb 2023 02:47:27 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Feb 2023 02:47:28 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Feb 2023 02:47:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Feb 2023 02:47:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Feb 2023 02:47:31 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Feb 2023 02:47:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Feb 2023 02:47:33 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Feb 2023 02:47:34 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 80
# Thu, 16 Feb 2023 02:47:35 GMT
EXPOSE 443
# Thu, 16 Feb 2023 02:47:36 GMT
EXPOSE 443/udp
# Thu, 16 Feb 2023 02:47:37 GMT
EXPOSE 2019
# Thu, 16 Feb 2023 02:47:56 GMT
RUN caddy version
# Thu, 16 Feb 2023 02:47:57 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1961fba6606566986ddd1960cf8309d19fa9deaa486f5a162a60114f3d4c3c82`  
		Last Modified: Thu, 16 Feb 2023 02:51:29 GMT  
		Size: 778.8 KB (778807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af5d76bf41697a16b3336a1857d1e530a3137f28d997c6f5eca0121d42ea88d`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d935f5b810851a2833b69e65d9dcff828f1c6686dab6fa117e9bd08eb95f5990`  
		Last Modified: Thu, 16 Feb 2023 02:51:31 GMT  
		Size: 14.9 MB (14914232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54e2a419181dd9257efde40f9ab80121dd6cc1a478f6ff42d160ddbf5e17cd4`  
		Last Modified: Thu, 16 Feb 2023 02:51:28 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c07f1bbb0931b3148683baae55ab0d85f8576b2a1d8c2a59bb28544572b5a9d`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06073fd741cf5968f24574903b70213f9743b648ebec9c53ccb8fe114ce01ae`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a17243f1184726e21bf0821ee5984a84575b55befba72594fbf0b3a32a47f1`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c403099e0a283f6f2b25b4235c61c8b564a832643f33280253dc040d2a2ab07`  
		Last Modified: Thu, 16 Feb 2023 02:51:26 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cc4608f06891b205fbec74e83a221161a2f9d9b50a0b548c3c716d176ee1a4`  
		Last Modified: Thu, 16 Feb 2023 02:51:25 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfe2ac143052b1fa8973567134244ce4ecd1693f16205dd53f0d4cf1b5caa5a`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e217159efeb187bf7ae9a12f6f70764141dd97837f24a517851bc15a36b552`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc05a7da758918922e168d1b07b29f4a81d398dc805724dd6b23b4cb28c7b43`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832768cea319f33011657944b08b51ea41229fdd7a37f21162dd8aedceb31a6b`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443fc82ac63aefa17f6de497731a007fbc972b175040388a8fda7112834af9fa`  
		Last Modified: Thu, 16 Feb 2023 02:51:24 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39ff50a2c37b226c6e79e3789d1706fc47cb355b14372a147024fc11b2dfb2b`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c6037df6cbd4b9e046dded7157e841a1c40659c4dd082ff9d397c95be6e411`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a470cfe53e2d01e3ca43a7211eb050493a97f430e3c5a52e2364f54a0a4e4834`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d12a1c4350235354af8011d0b2eccb56884eea72a0475197fb007c4fa6c111`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 359.9 KB (359894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea80c894fe52045adaa4c44b9f66422259571c7aec153753d27a56aa3ccbd930`  
		Last Modified: Thu, 16 Feb 2023 02:51:22 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
