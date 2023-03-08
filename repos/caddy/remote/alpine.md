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
