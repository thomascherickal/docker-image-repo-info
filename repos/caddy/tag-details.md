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
-	[`caddy:2.7`](#caddy27)
-	[`caddy:2.7-alpine`](#caddy27-alpine)
-	[`caddy:2.7-builder`](#caddy27-builder)
-	[`caddy:2.7-builder-alpine`](#caddy27-builder-alpine)
-	[`caddy:2.7-builder-windowsservercore-1809`](#caddy27-builder-windowsservercore-1809)
-	[`caddy:2.7-builder-windowsservercore-ltsc2022`](#caddy27-builder-windowsservercore-ltsc2022)
-	[`caddy:2.7-windowsservercore`](#caddy27-windowsservercore)
-	[`caddy:2.7-windowsservercore-1809`](#caddy27-windowsservercore-1809)
-	[`caddy:2.7-windowsservercore-ltsc2022`](#caddy27-windowsservercore-ltsc2022)
-	[`caddy:2.7.5`](#caddy275)
-	[`caddy:2.7.5-alpine`](#caddy275-alpine)
-	[`caddy:2.7.5-builder`](#caddy275-builder)
-	[`caddy:2.7.5-builder-alpine`](#caddy275-builder-alpine)
-	[`caddy:2.7.5-builder-windowsservercore-1809`](#caddy275-builder-windowsservercore-1809)
-	[`caddy:2.7.5-builder-windowsservercore-ltsc2022`](#caddy275-builder-windowsservercore-ltsc2022)
-	[`caddy:2.7.5-windowsservercore`](#caddy275-windowsservercore)
-	[`caddy:2.7.5-windowsservercore-1809`](#caddy275-windowsservercore-1809)
-	[`caddy:2.7.5-windowsservercore-ltsc2022`](#caddy275-windowsservercore-ltsc2022)
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
$ docker pull caddy@sha256:325f81ca0328db0737503a53f43717fce79ea0c574e83f8e586c8d350cadf34b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4974; amd64
	-	windows version 10.0.20348.2031; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:a9c7585fdc50bb28d686b73a9b1f0eb9a3d103efd63c48dc334ccb5f51aa1722
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18474311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70c3913f54e294079c54cc8b651576b08dd4add42a0f4c0bc93d539913ae335d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:11:11 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:11:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:11:12 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:11:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:11:15 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:11:15 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:11:16 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:11:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5433daac73cddf3f03243a31c38d460570073f83e9a8cf64c7f0e3387b85807`  
		Last Modified: Sat, 21 Oct 2023 00:11:36 GMT  
		Size: 350.8 KB (350840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c6b4aafe2c09344f58425bb0fe037a429808edb7b2ba37d79cd35b2775a422`  
		Last Modified: Sat, 21 Oct 2023 00:11:36 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a182bff4e1b33f3d5dd80f809e697793466287c3da7704863c3d0b51d42b5b`  
		Last Modified: Sat, 21 Oct 2023 00:11:39 GMT  
		Size: 14.7 MB (14713998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f43da8d65d754093117d4c673a7b725316be4e576e32b0d40c995e6ab1a07b7c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17422245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18b3bb2c3e0a97c9fe052eca67890f691907de7a5b514e88a44e660bb905079b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:06:46 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:06:48 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:06:48 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:06:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:06:51 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:06:51 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:06:52 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:06:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e09dc0459583a6ad3ba0428d5e180b7e3e6ae28360a69e293f03632cec397a0`  
		Last Modified: Sat, 21 Oct 2023 00:07:14 GMT  
		Size: 347.6 KB (347617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4705ff25da68d95a4bd671cbd4cec69369ea788be53bfafb45cdf4a930a725f8`  
		Last Modified: Sat, 21 Oct 2023 00:07:13 GMT  
		Size: 7.5 KB (7504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969c487cd333c7b53a7f57017e0ad77490d3806d9e52259caf9772016e96576d`  
		Last Modified: Sat, 21 Oct 2023 00:07:16 GMT  
		Size: 13.9 MB (13921833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:dd028bb08526d3533680243c94b9464c9c1a6559dccf5dde3b61ec73b9afd002
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17155303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:539aa551acc109f33c6ea5076a1f518af4d0476b517dc698d98c7350e8cb1b1a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:17:55 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:17:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:17:56 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:17:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:17:59 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:17:59 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:18:00 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:18:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee93e167fdbd8e67ec3f4ed8eaf242e5c8022a9845dd4f797448503af15d777c`  
		Last Modified: Sat, 21 Oct 2023 00:18:22 GMT  
		Size: 344.5 KB (344454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2895c0143aa41e87473191f749160d3109330cdb9de0c90a9b0a9e60e8a3a3e`  
		Last Modified: Sat, 21 Oct 2023 00:18:22 GMT  
		Size: 7.5 KB (7508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f015da3d3488ea9171b2970be40718bfa7e31496bae565a9bc2b677e53c09915`  
		Last Modified: Sat, 21 Oct 2023 00:18:25 GMT  
		Size: 13.9 MB (13903436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:d18ec23ab87841ede7ccefc353c20d1554faddf3ac362213c32ae22311136da5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17273763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cbdde935029392921ca3521ef9ebdb6a2b46cd1d4b7a9dabf0b71b00c593572`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:23:28 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:23:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:23:29 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:23:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:23:31 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:23:31 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:23:32 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:23:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461fe4f467fe88a160e176c442825b4bfea8dde13fc2324393a5d81518375e6f`  
		Last Modified: Sat, 21 Oct 2023 00:23:52 GMT  
		Size: 360.6 KB (360623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9335adc9ff07e38d963f0a71a2f7db01b5b5ed8e9d93fba14e584f25ea05c29d`  
		Last Modified: Sat, 21 Oct 2023 00:23:52 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32426666f5ec8621a07038733361be24f83719a812c0cce54e3f41192b31c2d`  
		Last Modified: Sat, 21 Oct 2023 00:23:54 GMT  
		Size: 13.6 MB (13573803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:1cd57ee42a4e84e91731e9182350ab4fd5b26705ec7286c28c5768c549435fd5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.1 MB (17057167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5aa3d5c5c63bea353c483de170ae8690a4f7eb12042cb84dc2bf0d52bf914b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:09:00 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:09:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:09:02 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:09:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:09:05 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:09:05 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:09:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:09:09 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:09:09 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:09:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692440f8f5ba2c6efbf2e74e3301377e3d9a90ae5a7cbd728c771ab306277830`  
		Last Modified: Sat, 21 Oct 2023 00:09:34 GMT  
		Size: 362.2 KB (362183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2886f5cbb210969eea27d97b8a48d88cae7bbe1bdd528a2b2775a8affde3084`  
		Last Modified: Sat, 21 Oct 2023 00:09:33 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdd6a19a7b9d3f4621c5388c53b0a9ea5591e9e72250bc60bcf22ed672632b1`  
		Last Modified: Sat, 21 Oct 2023 00:09:36 GMT  
		Size: 13.3 MB (13340969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:7dc6afd9bb40ff4450e4282bc56431b993d068c5b832c914dd50831189920061
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.8 MB (17822696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be3873facfc56aac0a1a9659efab4cddfc06afe6ac27c54cdd1b6fc9a23f1c1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:05:23 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:05:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:05:24 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:05:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:05:27 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:05:27 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:05:29 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:05:29 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:05:29 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d6d08cebdb83ff91ba335e0c4aec115b17261ed40307aaee6adde8c6763ad6`  
		Last Modified: Sat, 21 Oct 2023 00:06:00 GMT  
		Size: 355.0 KB (354963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58e0c7856c877cacd1d63a86beb12c9be91c4a0950dd85954db6f16a6d93103`  
		Last Modified: Sat, 21 Oct 2023 00:06:00 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69bf19674eec620ff3f87ecb754c60b7c137eb6c8c3763ff795739061593a77`  
		Last Modified: Sat, 21 Oct 2023 00:06:02 GMT  
		Size: 14.2 MB (14245123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.4974; amd64

```console
$ docker pull caddy@sha256:77cb1b0b8315f376e69becef400d33c9d8b2a45548714845a821736158771de2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2047649951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3171dc2f25b4435520d8ba983ebf42f070ddec217b0da7677e309cc4cd51b05`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 03:59:19 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:39:06 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:40:04 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:40:05 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:40:06 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:40:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:40:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:40:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:40:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:40:12 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:40:13 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:41:01 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:41:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c4565a9b36858bc727874537e3c99968438a37e53c13057b0b1a233699d014`  
		Last Modified: Wed, 11 Oct 2023 04:05:44 GMT  
		Size: 472.0 KB (472034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df4a75108d3a33583e7ae61f1a019d4865860820bd89280ba414af94dd3f56e`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9dee9792a7bf7e1225840c56fb692536bee1743eba0a4da2faff34533f1160f`  
		Last Modified: Thu, 12 Oct 2023 01:44:37 GMT  
		Size: 15.3 MB (15296055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41900185a2519f01b8bd860f70936cee271612c4023512694b105826e0e0251`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0f1b69a12cd8550d868156e54168abaa32e1df40ee6eb39bc4e173ce04905e`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca266891343bff15b313846692ba3a41f313d5b228bedde964191332a16dffe`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12539eb7433a69ed67556d91b75b66dfedf0543d3efd7dabe82772437307a6f`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5103f279ed518bcfec88e00183e3222b50c1bc2f0e5b42f043e2198da424de98`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efc1cff2dac4308ce732a395ee215e1497d21f737e42e77917debf070afa8d7`  
		Last Modified: Thu, 12 Oct 2023 01:44:35 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cb50f59d2b11532a330925afb6ebd04d9b4708de8b11ae436e258c3764d741`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd11a311e4c0cf49bb544980f2c999751fc5e2fbe80d37b0f719f837abf8c3f`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ccbee9a6b9058ec933797dc1cfed875ceeb0115ce29ee163cd60a66e9f3b2d`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b486fc8ef055010a59374557443d3b713b9e55c1ccd11b7873f47876758976`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41df430d9a95c6000c922dd021b6cb2af0110dcc661ddc37a190a8cf6cd4bb06`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f243061a2e17d508efa4a424310d9ca158ca0cf0f59bd15cac606ab3e74701`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e709fff7d020a5d7c2d9e9e9a664c87392e9f9a4f4ced9802e64ca268995e23`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2c7aca9b511bc62340e6e8883d5f625bdccb805c4e897b837b68f3c79964b5`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38802c5a2b45b7029b250d88dac8209405146b0968925d1204cf17f7c3e76d98`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 269.1 KB (269086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376d19318a370d0da2ffcc29b47c2810278efa9d22fb39799c48687dfee0a2d9`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.20348.2031; amd64

```console
$ docker pull caddy@sha256:05f529a68927f0acfa7afbc79b7a19541f94430c137612ed344de7a822dcfafb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1875907229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8701a0e5aada270070acddeed89c57e20a5cac8afd88ed58da9557bf01dccb27`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:02:07 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:41:20 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:41:42 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:41:42 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:41:43 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:41:44 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:41:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:41:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:41:50 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:41:52 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:42:04 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:42:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c36616366b0df84f087a09bf19876f3872d839997f2f43e4eb8599861417c06`  
		Last Modified: Wed, 11 Oct 2023 04:06:10 GMT  
		Size: 467.9 KB (467933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db420ca589f10e4f9f5bc9dd6badc855d95c6a598888f2eb77a747eced259557`  
		Last Modified: Thu, 12 Oct 2023 01:45:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b5d7433dab05533d906a290a0f42cf31804c132da65c9fd7d4d2c41a64f519`  
		Last Modified: Thu, 12 Oct 2023 01:45:04 GMT  
		Size: 15.3 MB (15284209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62069fdf38bff9495ef2be05d397a55221536f9eec345734d6acec3a6196324f`  
		Last Modified: Thu, 12 Oct 2023 01:45:00 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e237a4c373c6937b5c51d0a3936152ac2b572fd5a432db3690f4070a7c78327`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73fae1c57e166a2ade87aa32e11980b456658212b296eea0f02ba3ec1c6557b`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000f2101dc464fa43321619c6e65c5b9e62b62755f3b141e69bd31892a253ded`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8536723423849b861a08fa490135f690c287be0144267e38fb3e631fb1bddbd2`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f176ef86531863755c3a315ec662b8da324474ae6097d7365dc18b76d61bde5`  
		Last Modified: Thu, 12 Oct 2023 01:44:58 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3973c168b3a63daa069e3a9870395561709d7b27762ffafb16538c773a16ad29`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5a10fbc59abc7ee7cc04a7ff48cc85983728745e91e8ef5fafee0589ba2193`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf033f8ab12414230e08aaada214c761777b0c784908ad2783ee31f8d330d0c9`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e2af83b2af59d76bd9b735c4e71b9492d9dbc120c042b8134ae0a70008f49`  
		Last Modified: Thu, 12 Oct 2023 01:44:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0355ed819405072f13996095ae7ec7044017bee81808dea9500459620118c20b`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e86117e27425829055f627e6156a4a657d9817cf8d2158f0026752366c9022c`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22fbe71be2fe08164a92f1362959f0a4aba194dcf931945d7bb2ac50e8f6467`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed768b9f807d51e5834f0bc8b2ea4dda09a5139d126f9141cb3db51f781ea541`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359fc3c79eda3ddbb39c46b09a4c68137a693a72f8712182d545c546b726027e`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 289.5 KB (289533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e4b8683a429393010114c6906acced22d65d5167cda2cc55238ae5b9f816c0`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:f1c092da9fcba7a8197cf1065a347d4f0bb67b6dd188985eafaf0a5aec6c9041
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
$ docker pull caddy@sha256:a9c7585fdc50bb28d686b73a9b1f0eb9a3d103efd63c48dc334ccb5f51aa1722
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18474311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70c3913f54e294079c54cc8b651576b08dd4add42a0f4c0bc93d539913ae335d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:11:11 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:11:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:11:12 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:11:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:11:15 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:11:15 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:11:16 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:11:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5433daac73cddf3f03243a31c38d460570073f83e9a8cf64c7f0e3387b85807`  
		Last Modified: Sat, 21 Oct 2023 00:11:36 GMT  
		Size: 350.8 KB (350840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c6b4aafe2c09344f58425bb0fe037a429808edb7b2ba37d79cd35b2775a422`  
		Last Modified: Sat, 21 Oct 2023 00:11:36 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a182bff4e1b33f3d5dd80f809e697793466287c3da7704863c3d0b51d42b5b`  
		Last Modified: Sat, 21 Oct 2023 00:11:39 GMT  
		Size: 14.7 MB (14713998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f43da8d65d754093117d4c673a7b725316be4e576e32b0d40c995e6ab1a07b7c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17422245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18b3bb2c3e0a97c9fe052eca67890f691907de7a5b514e88a44e660bb905079b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:06:46 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:06:48 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:06:48 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:06:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:06:51 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:06:51 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:06:52 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:06:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e09dc0459583a6ad3ba0428d5e180b7e3e6ae28360a69e293f03632cec397a0`  
		Last Modified: Sat, 21 Oct 2023 00:07:14 GMT  
		Size: 347.6 KB (347617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4705ff25da68d95a4bd671cbd4cec69369ea788be53bfafb45cdf4a930a725f8`  
		Last Modified: Sat, 21 Oct 2023 00:07:13 GMT  
		Size: 7.5 KB (7504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969c487cd333c7b53a7f57017e0ad77490d3806d9e52259caf9772016e96576d`  
		Last Modified: Sat, 21 Oct 2023 00:07:16 GMT  
		Size: 13.9 MB (13921833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:dd028bb08526d3533680243c94b9464c9c1a6559dccf5dde3b61ec73b9afd002
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17155303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:539aa551acc109f33c6ea5076a1f518af4d0476b517dc698d98c7350e8cb1b1a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:17:55 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:17:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:17:56 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:17:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:17:59 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:17:59 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:18:00 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:18:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee93e167fdbd8e67ec3f4ed8eaf242e5c8022a9845dd4f797448503af15d777c`  
		Last Modified: Sat, 21 Oct 2023 00:18:22 GMT  
		Size: 344.5 KB (344454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2895c0143aa41e87473191f749160d3109330cdb9de0c90a9b0a9e60e8a3a3e`  
		Last Modified: Sat, 21 Oct 2023 00:18:22 GMT  
		Size: 7.5 KB (7508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f015da3d3488ea9171b2970be40718bfa7e31496bae565a9bc2b677e53c09915`  
		Last Modified: Sat, 21 Oct 2023 00:18:25 GMT  
		Size: 13.9 MB (13903436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:d18ec23ab87841ede7ccefc353c20d1554faddf3ac362213c32ae22311136da5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17273763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cbdde935029392921ca3521ef9ebdb6a2b46cd1d4b7a9dabf0b71b00c593572`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:23:28 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:23:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:23:29 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:23:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:23:31 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:23:31 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:23:32 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:23:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461fe4f467fe88a160e176c442825b4bfea8dde13fc2324393a5d81518375e6f`  
		Last Modified: Sat, 21 Oct 2023 00:23:52 GMT  
		Size: 360.6 KB (360623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9335adc9ff07e38d963f0a71a2f7db01b5b5ed8e9d93fba14e584f25ea05c29d`  
		Last Modified: Sat, 21 Oct 2023 00:23:52 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32426666f5ec8621a07038733361be24f83719a812c0cce54e3f41192b31c2d`  
		Last Modified: Sat, 21 Oct 2023 00:23:54 GMT  
		Size: 13.6 MB (13573803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:1cd57ee42a4e84e91731e9182350ab4fd5b26705ec7286c28c5768c549435fd5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.1 MB (17057167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5aa3d5c5c63bea353c483de170ae8690a4f7eb12042cb84dc2bf0d52bf914b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:09:00 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:09:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:09:02 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:09:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:09:05 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:09:05 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:09:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:09:09 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:09:09 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:09:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692440f8f5ba2c6efbf2e74e3301377e3d9a90ae5a7cbd728c771ab306277830`  
		Last Modified: Sat, 21 Oct 2023 00:09:34 GMT  
		Size: 362.2 KB (362183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2886f5cbb210969eea27d97b8a48d88cae7bbe1bdd528a2b2775a8affde3084`  
		Last Modified: Sat, 21 Oct 2023 00:09:33 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdd6a19a7b9d3f4621c5388c53b0a9ea5591e9e72250bc60bcf22ed672632b1`  
		Last Modified: Sat, 21 Oct 2023 00:09:36 GMT  
		Size: 13.3 MB (13340969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:7dc6afd9bb40ff4450e4282bc56431b993d068c5b832c914dd50831189920061
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.8 MB (17822696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be3873facfc56aac0a1a9659efab4cddfc06afe6ac27c54cdd1b6fc9a23f1c1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:05:23 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:05:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:05:24 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:05:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:05:27 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:05:27 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:05:29 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:05:29 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:05:29 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d6d08cebdb83ff91ba335e0c4aec115b17261ed40307aaee6adde8c6763ad6`  
		Last Modified: Sat, 21 Oct 2023 00:06:00 GMT  
		Size: 355.0 KB (354963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58e0c7856c877cacd1d63a86beb12c9be91c4a0950dd85954db6f16a6d93103`  
		Last Modified: Sat, 21 Oct 2023 00:06:00 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69bf19674eec620ff3f87ecb754c60b7c137eb6c8c3763ff795739061593a77`  
		Last Modified: Sat, 21 Oct 2023 00:06:02 GMT  
		Size: 14.2 MB (14245123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:d039cffaec2ce64db9cae84dc789bb36c8d3d09e6ff70f3a40c4f405a89deed8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4974; amd64
	-	windows version 10.0.20348.2031; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:d1f6d3dcfec129b4d0e23b6743f576807352958232a7ac6c17ee36f785fe5c58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76972374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e113a57232410dd987d12708b35062e6a269825fa7b4d03aef42c00acc93dce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:54:30 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:54:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:20:11 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:20:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 19:20:22 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:20:22 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:20:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:20:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:20:23 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:11:20 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:11:20 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:11:20 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:11:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:11:21 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:11:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:11:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:11:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc37b24bb09971feb8bf4882e861bce9db0c985a16a900adb0dc9de3f854243b`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 284.7 KB (284690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a4303e95078c253686dcc16d7717644af63809efcbd753c0a999c9aad3fe72`  
		Last Modified: Tue, 10 Oct 2023 19:26:17 GMT  
		Size: 67.0 MB (67012876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359925be0f358b952dc8be63647139c5aab0fff94f7a070d88cb51dd258f80e5`  
		Last Modified: Tue, 10 Oct 2023 19:26:06 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958092cb44d28ddde181d193284001b1146b33a1cf19624e9683fc8f31551043`  
		Last Modified: Sat, 21 Oct 2023 00:11:52 GMT  
		Size: 5.0 MB (4970044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85cdb072dd78dcf6a7b04409cf7c8dc1fddddf912b601b15c6dc94adb2df10b`  
		Last Modified: Sat, 21 Oct 2023 00:11:51 GMT  
		Size: 1.3 MB (1302237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32749367842b0c8b40e7f61a315ff21b4d42211b5399e648beb75d86acb29c4c`  
		Last Modified: Sat, 21 Oct 2023 00:11:51 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:15f0db6d62062758441d2d22fd178c42299cf148c5097ffe10468153ff40c6b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75413855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:509cf858d9f3ffa4a94fe988705864c41bd510f34ade4ece0d2ede4cda23599f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:55:22 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:55:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 18:49:21 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 18:49:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 18:49:42 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 18:49:42 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 18:49:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 18:49:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 18:49:43 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:06:57 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:06:57 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:06:58 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:06:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:06:58 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:06:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:06:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:06:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3da3b9e7a12f6bb6b7f56e9240c2c92ce8c9f5fd5ef3b3063b9a93d454919e`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 284.9 KB (284887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbbb7b34bc324d050e49d3dd31294bdde5d6ecda33decf9afe31c11165b138a`  
		Last Modified: Tue, 10 Oct 2023 18:55:32 GMT  
		Size: 65.8 MB (65770135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c022f45a9fb1e7649eb4a663acd4ed6437363b4fc6e56f6af3e5f457a5d06ee8`  
		Last Modified: Tue, 10 Oct 2023 18:55:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12bec1760d3cf2773adbb14bd47431e46e130a914a46535c9a70de28e4b363b`  
		Last Modified: Sat, 21 Oct 2023 00:07:30 GMT  
		Size: 5.0 MB (4964316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888b304960048015ef929fcb0ffab750c1ba463aaf1d419272f2233e67195d56`  
		Last Modified: Sat, 21 Oct 2023 00:07:30 GMT  
		Size: 1.2 MB (1248665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00237a85b25c3b9ee3968fe9e98da8f378a4a70ccc746a6524820916085348ef`  
		Last Modified: Sat, 21 Oct 2023 00:07:29 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9275f10d0ef0db0999dc5ed6b19c068a941f59a05d69fad4b3cb07c3f0b14a7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74714658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b10f4fd814dc9e97d1147715baacffedd007b23ec081f4c100520df02050e6c9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:07:30 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 15:58:50 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:58:50 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 15:59:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 15:59:08 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 15:59:08 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 15:59:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:59:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 15:59:09 GMT
WORKDIR /go
# Wed, 01 Nov 2023 21:17:21 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 21:17:22 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 21:17:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 21:17:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 21:17:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8457acc181d300b4231b44e12aa0bf4a99ced5d51c5dfdc14eb899a341d5b855`  
		Last Modified: Sat, 21 Oct 2023 01:07:42 GMT  
		Size: 284.1 KB (284074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05626b790821d279bd9aea8466a1a79307764cbc389c51ab081a4b98c7657dc2`  
		Last Modified: Wed, 01 Nov 2023 16:06:11 GMT  
		Size: 65.8 MB (65772806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2dba3cbff62191bbc046c664eead34e3af26adfa5ecdbacf0ba6e73b9cbe51`  
		Last Modified: Wed, 01 Nov 2023 16:05:56 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357de4175525102c1d6c8d4fc605461ca1b1791b2a3b6c55c73e3ef6266159ad`  
		Last Modified: Wed, 01 Nov 2023 21:17:50 GMT  
		Size: 4.5 MB (4511226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59aa4bdeb70fa8c96a09911a5e79184a493cb38488e04d22007af9f9164e4f44`  
		Last Modified: Wed, 01 Nov 2023 21:17:50 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7b450bb18e60383a1dd8c51f37de16c5782ba7eba9e2737540247f3a4394c8`  
		Last Modified: Wed, 01 Nov 2023 21:17:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:76d3844fa9c17929397bb168745241a1f8fa36bf63c437d9d255fe217ec6a87c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73995976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6b4383d952151327974f3f21fa7be1e862f9a67c4ee08a264948e4372890be6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 02:41:07 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 15:36:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:36:13 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 15:36:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 15:36:23 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 15:36:23 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 15:36:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:36:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 15:36:24 GMT
WORKDIR /go
# Wed, 01 Nov 2023 19:56:22 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 19:56:22 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 19:56:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 19:56:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 19:56:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74bf0db6f91dfe1899e8204affb86f8c505a5643bdcb83b085888c86e0c7411`  
		Last Modified: Sat, 21 Oct 2023 02:41:18 GMT  
		Size: 286.3 KB (286297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd442d12e388d3f44ee4325caf9e959ca82d4064c8b1b38321da75a84a6ccbd`  
		Last Modified: Wed, 01 Nov 2023 15:41:04 GMT  
		Size: 64.1 MB (64110459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0297817440f5024a6c0e27f7906a375aa91aea5aaf191caa3f1762426e60e9c2`  
		Last Modified: Wed, 01 Nov 2023 15:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9fb63180b1c62b2cfd436428dc31a25bc97989024e217b9d8e508e82b0b287`  
		Last Modified: Wed, 01 Nov 2023 19:56:42 GMT  
		Size: 5.1 MB (5068382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0ee6df11f2e2e143f36f30697c4b309c4560fa062faa2fcb3a1c22db91257e`  
		Last Modified: Wed, 01 Nov 2023 19:56:42 GMT  
		Size: 1.2 MB (1198448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15b8268dd8cba7445da5d02c68c6787ce774d7ecc7dba9fa3f2775a88884d64`  
		Last Modified: Wed, 01 Nov 2023 19:56:41 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:ed1e2679ee802b3a2c8f7b42d4828ecc9ba50b5a029e3d14bbc54fa2a0fc5444
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74214117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2041e14adf1ce1c2b331135049ec2871be632eb2a7130142af035fa662cb1e19`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:13:11 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:13:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:17:44 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:18:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 19:18:14 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:18:14 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:18:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:18:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:18:17 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:09:16 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:09:17 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:09:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:09:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:09:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc67971d1767eae5019ffeaf8f893e6d81dbba50bde347da0c0433c56e3f2a3`  
		Last Modified: Thu, 28 Sep 2023 22:18:17 GMT  
		Size: 286.7 KB (286659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1caf7fa003bdf7c7611eb2e33a11db077a0f632b70d28f5b73096bf051f25aeb`  
		Last Modified: Tue, 10 Oct 2023 19:28:09 GMT  
		Size: 64.1 MB (64125245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9573c5aef56335266ce720d0812f9a0156f628fbd01ba4a6462be56d8742dc8a`  
		Last Modified: Tue, 10 Oct 2023 19:27:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40b483d55ec27555b481cb0fad97faf6e8d1686165905df945c86967ec0ac96`  
		Last Modified: Sat, 21 Oct 2023 00:09:50 GMT  
		Size: 5.3 MB (5268969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966ad11dd0f3a17ae3666a37f54fd9d6265bc0e18133314a565abf1039e90a1f`  
		Last Modified: Sat, 21 Oct 2023 00:09:50 GMT  
		Size: 1.2 MB (1186175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e18b62f88891e2a1b8f7a5e8a66e6ee69c9f42fe03945d66da418c55d339a9`  
		Last Modified: Sat, 21 Oct 2023 00:09:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:02d085e00e424e29b1a4c45b6358c9ac90629ed72540af87be474238770f3217
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76112263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fa19320a45d01205e0025f17edf0aa856b433bd25ee512a7877ec407bdf0a3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:44:44 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 12:29:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 12:29:18 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 12:29:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 12:29:51 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 12:29:52 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 12:29:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 12:29:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 12:29:54 GMT
WORKDIR /go
# Wed, 01 Nov 2023 16:51:53 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 16:51:55 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 16:51:56 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 16:51:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 16:51:57 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 16:51:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 16:52:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 16:52:01 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f15a4d38dd3d4f044868149900a763ac233f1aef33fe18019f45149b6bd02c`  
		Last Modified: Sat, 21 Oct 2023 00:45:00 GMT  
		Size: 285.1 KB (285095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23831500ce8c52e3d80c9eab9eb44d36e8daf00224a75f36d961186e47851ae8`  
		Last Modified: Wed, 01 Nov 2023 12:38:38 GMT  
		Size: 66.2 MB (66234435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92c933a1dfb2cbb65a33ccba713aabb9ff92ce6a0286e12af67e54c51be8a44`  
		Last Modified: Wed, 01 Nov 2023 12:38:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368a8f32c470e61e32632b0c78836e09dc1d70ab0e9a48e1c2bef1d23de82f7d`  
		Last Modified: Wed, 01 Nov 2023 16:52:34 GMT  
		Size: 5.1 MB (5114679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b61d54a31e32a9c971c8d7ea514537dababa89a4e60ce97eca5bdcf4e8d007`  
		Last Modified: Wed, 01 Nov 2023 16:52:33 GMT  
		Size: 1.3 MB (1262390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147c37f0535cd57e5355158d43aa5608a1430f56aa08ef1b4eb9cea12976a728`  
		Last Modified: Wed, 01 Nov 2023 16:52:33 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.4974; amd64

```console
$ docker pull caddy@sha256:951876270030a4a5404a8bab425d35b64f90babc594bb65c261cc05eab33ed79
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2128478401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:883908294a37d78f29e796d389d42c83a12c68a6c0f1113bba3bdd9290db5b05`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 02:23:09 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Oct 2023 02:23:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Oct 2023 02:23:11 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Oct 2023 02:23:12 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Oct 2023 02:24:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:24:31 GMT
ENV GOPATH=C:\go
# Wed, 11 Oct 2023 02:25:33 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Oct 2023 02:25:34 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 11 Oct 2023 02:28:30 GMT
RUN $url = 'https://dl.google.com/go/go1.21.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '27c8daf157493f288d42a6f38debc6a2cb391f6543139eba9152fceca0be2a10'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:28:31 GMT
WORKDIR C:\go
# Wed, 11 Oct 2023 04:03:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:03:14 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 12 Oct 2023 01:42:14 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:42:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 12 Oct 2023 01:43:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 12 Oct 2023 01:43:13 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fded5ce3c59d7e8d637a5536d6eed085ff6b6a323f42c1df76a7be6e9970ee`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a72a6b595ab9f8f71a34a065e75e609b20ea5e026f901820fce6d3c9134939`  
		Last Modified: Wed, 11 Oct 2023 02:46:39 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2574f8b7fb0ec5a8c39ee40a8008f0d24c398380247bf7140be1abdede5542b`  
		Last Modified: Wed, 11 Oct 2023 02:46:40 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951c53676fe729ebf5d3c07215d91afa952e6190715f79a7952f4c3aa121231e`  
		Last Modified: Wed, 11 Oct 2023 02:46:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a382bb149b70b82f9c2f58ebf6a2672dc4c64460017836d73a5a23b7379ea095`  
		Last Modified: Wed, 11 Oct 2023 02:46:44 GMT  
		Size: 25.6 MB (25557568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608a2584f4b3b8f3038fa41c0719005822ab967d85d1231843bd729a7b3d2d60`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1058e02ad62f976d823e3035f0578b2868eb09f28986153342a52014cc5c3810`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 284.8 KB (284754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fce039c31b2e60b62a0ede9974b6574519f2e47e1d8f4e09c7a1f30763aee95`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65449f183261f9bbdb731d41f5e6fca94f3e547e8d996133e418773400cfcfe`  
		Last Modified: Wed, 11 Oct 2023 02:46:59 GMT  
		Size: 69.3 MB (69345382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394e07c2ad53e950c47ffb647836822197dc5f8ebe082eaa045854e2b25bafc7`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993f5e59c63ef5be894fc498ab0e165faa3129d35a8a8f5173f12c6a4232f588`  
		Last Modified: Wed, 11 Oct 2023 04:06:31 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c675831130735b443a544dff1b9c188928f34947a5342350ef04eadc0d1ab27`  
		Last Modified: Wed, 11 Oct 2023 04:06:28 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69fe7c1d1f5383a4421f2a0e7284e17db440ee5b7be9f487ce9048f76970e7b6`  
		Last Modified: Thu, 12 Oct 2023 01:45:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee998763c3cef90b11adda3322e66e1a89d89409d1ed29dd73a4101fb657e29`  
		Last Modified: Thu, 12 Oct 2023 01:45:21 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196a81b981d5dc89b19acce594b87914fc5bc4777e42b1322ca9b9d4c4b4f179`  
		Last Modified: Thu, 12 Oct 2023 01:45:22 GMT  
		Size: 1.7 MB (1682335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3ad6e4e7b1be08f8a79e4d77328648deded93f9ef0d4a1e8202ce4c3a21c67`  
		Last Modified: Thu, 12 Oct 2023 01:45:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.20348.2031; amd64

```console
$ docker pull caddy@sha256:04b6c1b2519c8d35d65976c53b4523d7074d53c7b98fa5b29b83c837e021b493
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1956648108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6c3e402a7640df51573fae3237803e1e5fabce3d4c88849d9513c716654d474`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 02:19:41 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Oct 2023 02:19:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Oct 2023 02:19:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Oct 2023 02:19:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Oct 2023 02:20:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:20:18 GMT
ENV GOPATH=C:\go
# Wed, 11 Oct 2023 02:20:42 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Oct 2023 02:20:42 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 11 Oct 2023 02:22:59 GMT
RUN $url = 'https://dl.google.com/go/go1.21.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '27c8daf157493f288d42a6f38debc6a2cb391f6543139eba9152fceca0be2a10'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:23:01 GMT
WORKDIR C:\go
# Wed, 11 Oct 2023 04:04:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:04:42 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 12 Oct 2023 01:43:30 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:43:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 12 Oct 2023 01:43:51 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 12 Oct 2023 01:43:52 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60407a49ce6121c65fa6399c333c5227a09518414fd987c460ea29cb441ac5a`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe632e8cddda4e5f347720b87b8b3868e2e2969048761e3b0a40799d33f5f7a`  
		Last Modified: Wed, 11 Oct 2023 02:45:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4384696fc834e9658e7b3e5d1ceb1f8b362db85865daf29521b3c75c6999c046`  
		Last Modified: Wed, 11 Oct 2023 02:45:04 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c794ea611ef69f54d577f90b68e165e40a17e43b6d1d08f59951a38e084ea5fb`  
		Last Modified: Wed, 11 Oct 2023 02:45:03 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c74dc2d701da2bfabc4d44e6a4e6b92912515e2ca1fb053ffcc6b0d5cae2972`  
		Last Modified: Wed, 11 Oct 2023 02:45:08 GMT  
		Size: 25.5 MB (25531724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91612399ba7df8de0a05ad078c3817548f0a3b44516b76565e14a96ea62452e9`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7439c7c4353d2432c780827e4926910b19e84fe436d58e0a8129de2f631bd2b8`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 264.4 KB (264384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b0eaedd98e739ace4b7934261c71292195e461adcc977d02e57604d4a42ee8`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f46e84d4d007a200b1d6e7cb5b48db90116cdeb8bd3ec3964a08191875973e2`  
		Last Modified: Wed, 11 Oct 2023 02:45:25 GMT  
		Size: 69.3 MB (69325670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f59bab6d84ca44bbb60474dcf59c9af4f0f15edbdd64249b0eeaf968aff211f`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.6 KB (1556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f449f4d34d707dbde9cbb245c154c0b2e1d1a2c55d172501f8d7da576866f76f`  
		Last Modified: Wed, 11 Oct 2023 04:06:49 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a2edf76facdd17af03954b607484f7f7b36164a30634d19dd96b7320feb6b5`  
		Last Modified: Wed, 11 Oct 2023 04:06:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802c3686d509915fea71538d2c40c7a48c71719fab6144cb4497b6118b276ab9`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99cb183ed6cdad781eaba7bd1b4cb443befd9042c8a59450ee41f0245dd0ece4`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec33434b55fade6bcd7f3f0dfc10c981de93dc44bbae2b8702fdb6418a37a65b`  
		Last Modified: Thu, 12 Oct 2023 01:45:38 GMT  
		Size: 1.7 MB (1664788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0833369ef8236fcf99aba2d1fa48788db07662d0a9885a8429d435bf9f2227b2`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:0b6ab47c59512267b3021fcb39af41d2896fd78718a39fa127cc8f2a4795638e
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
$ docker pull caddy@sha256:d1f6d3dcfec129b4d0e23b6743f576807352958232a7ac6c17ee36f785fe5c58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76972374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e113a57232410dd987d12708b35062e6a269825fa7b4d03aef42c00acc93dce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:54:30 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:54:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:20:11 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:20:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 19:20:22 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:20:22 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:20:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:20:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:20:23 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:11:20 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:11:20 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:11:20 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:11:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:11:21 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:11:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:11:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:11:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc37b24bb09971feb8bf4882e861bce9db0c985a16a900adb0dc9de3f854243b`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 284.7 KB (284690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a4303e95078c253686dcc16d7717644af63809efcbd753c0a999c9aad3fe72`  
		Last Modified: Tue, 10 Oct 2023 19:26:17 GMT  
		Size: 67.0 MB (67012876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359925be0f358b952dc8be63647139c5aab0fff94f7a070d88cb51dd258f80e5`  
		Last Modified: Tue, 10 Oct 2023 19:26:06 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958092cb44d28ddde181d193284001b1146b33a1cf19624e9683fc8f31551043`  
		Last Modified: Sat, 21 Oct 2023 00:11:52 GMT  
		Size: 5.0 MB (4970044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85cdb072dd78dcf6a7b04409cf7c8dc1fddddf912b601b15c6dc94adb2df10b`  
		Last Modified: Sat, 21 Oct 2023 00:11:51 GMT  
		Size: 1.3 MB (1302237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32749367842b0c8b40e7f61a315ff21b4d42211b5399e648beb75d86acb29c4c`  
		Last Modified: Sat, 21 Oct 2023 00:11:51 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:15f0db6d62062758441d2d22fd178c42299cf148c5097ffe10468153ff40c6b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75413855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:509cf858d9f3ffa4a94fe988705864c41bd510f34ade4ece0d2ede4cda23599f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:55:22 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:55:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 18:49:21 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 18:49:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 18:49:42 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 18:49:42 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 18:49:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 18:49:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 18:49:43 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:06:57 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:06:57 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:06:58 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:06:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:06:58 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:06:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:06:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:06:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3da3b9e7a12f6bb6b7f56e9240c2c92ce8c9f5fd5ef3b3063b9a93d454919e`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 284.9 KB (284887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbbb7b34bc324d050e49d3dd31294bdde5d6ecda33decf9afe31c11165b138a`  
		Last Modified: Tue, 10 Oct 2023 18:55:32 GMT  
		Size: 65.8 MB (65770135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c022f45a9fb1e7649eb4a663acd4ed6437363b4fc6e56f6af3e5f457a5d06ee8`  
		Last Modified: Tue, 10 Oct 2023 18:55:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12bec1760d3cf2773adbb14bd47431e46e130a914a46535c9a70de28e4b363b`  
		Last Modified: Sat, 21 Oct 2023 00:07:30 GMT  
		Size: 5.0 MB (4964316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888b304960048015ef929fcb0ffab750c1ba463aaf1d419272f2233e67195d56`  
		Last Modified: Sat, 21 Oct 2023 00:07:30 GMT  
		Size: 1.2 MB (1248665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00237a85b25c3b9ee3968fe9e98da8f378a4a70ccc746a6524820916085348ef`  
		Last Modified: Sat, 21 Oct 2023 00:07:29 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9275f10d0ef0db0999dc5ed6b19c068a941f59a05d69fad4b3cb07c3f0b14a7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74714658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b10f4fd814dc9e97d1147715baacffedd007b23ec081f4c100520df02050e6c9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:07:30 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 15:58:50 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:58:50 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 15:59:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 15:59:08 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 15:59:08 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 15:59:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:59:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 15:59:09 GMT
WORKDIR /go
# Wed, 01 Nov 2023 21:17:21 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 21:17:22 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 21:17:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 21:17:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 21:17:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8457acc181d300b4231b44e12aa0bf4a99ced5d51c5dfdc14eb899a341d5b855`  
		Last Modified: Sat, 21 Oct 2023 01:07:42 GMT  
		Size: 284.1 KB (284074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05626b790821d279bd9aea8466a1a79307764cbc389c51ab081a4b98c7657dc2`  
		Last Modified: Wed, 01 Nov 2023 16:06:11 GMT  
		Size: 65.8 MB (65772806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2dba3cbff62191bbc046c664eead34e3af26adfa5ecdbacf0ba6e73b9cbe51`  
		Last Modified: Wed, 01 Nov 2023 16:05:56 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357de4175525102c1d6c8d4fc605461ca1b1791b2a3b6c55c73e3ef6266159ad`  
		Last Modified: Wed, 01 Nov 2023 21:17:50 GMT  
		Size: 4.5 MB (4511226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59aa4bdeb70fa8c96a09911a5e79184a493cb38488e04d22007af9f9164e4f44`  
		Last Modified: Wed, 01 Nov 2023 21:17:50 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7b450bb18e60383a1dd8c51f37de16c5782ba7eba9e2737540247f3a4394c8`  
		Last Modified: Wed, 01 Nov 2023 21:17:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:76d3844fa9c17929397bb168745241a1f8fa36bf63c437d9d255fe217ec6a87c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73995976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6b4383d952151327974f3f21fa7be1e862f9a67c4ee08a264948e4372890be6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 02:41:07 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 15:36:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:36:13 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 15:36:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 15:36:23 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 15:36:23 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 15:36:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:36:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 15:36:24 GMT
WORKDIR /go
# Wed, 01 Nov 2023 19:56:22 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 19:56:22 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 19:56:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 19:56:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 19:56:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74bf0db6f91dfe1899e8204affb86f8c505a5643bdcb83b085888c86e0c7411`  
		Last Modified: Sat, 21 Oct 2023 02:41:18 GMT  
		Size: 286.3 KB (286297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd442d12e388d3f44ee4325caf9e959ca82d4064c8b1b38321da75a84a6ccbd`  
		Last Modified: Wed, 01 Nov 2023 15:41:04 GMT  
		Size: 64.1 MB (64110459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0297817440f5024a6c0e27f7906a375aa91aea5aaf191caa3f1762426e60e9c2`  
		Last Modified: Wed, 01 Nov 2023 15:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9fb63180b1c62b2cfd436428dc31a25bc97989024e217b9d8e508e82b0b287`  
		Last Modified: Wed, 01 Nov 2023 19:56:42 GMT  
		Size: 5.1 MB (5068382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0ee6df11f2e2e143f36f30697c4b309c4560fa062faa2fcb3a1c22db91257e`  
		Last Modified: Wed, 01 Nov 2023 19:56:42 GMT  
		Size: 1.2 MB (1198448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15b8268dd8cba7445da5d02c68c6787ce774d7ecc7dba9fa3f2775a88884d64`  
		Last Modified: Wed, 01 Nov 2023 19:56:41 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:ed1e2679ee802b3a2c8f7b42d4828ecc9ba50b5a029e3d14bbc54fa2a0fc5444
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74214117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2041e14adf1ce1c2b331135049ec2871be632eb2a7130142af035fa662cb1e19`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:13:11 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:13:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:17:44 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:18:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 19:18:14 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:18:14 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:18:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:18:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:18:17 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:09:16 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:09:17 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:09:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:09:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:09:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc67971d1767eae5019ffeaf8f893e6d81dbba50bde347da0c0433c56e3f2a3`  
		Last Modified: Thu, 28 Sep 2023 22:18:17 GMT  
		Size: 286.7 KB (286659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1caf7fa003bdf7c7611eb2e33a11db077a0f632b70d28f5b73096bf051f25aeb`  
		Last Modified: Tue, 10 Oct 2023 19:28:09 GMT  
		Size: 64.1 MB (64125245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9573c5aef56335266ce720d0812f9a0156f628fbd01ba4a6462be56d8742dc8a`  
		Last Modified: Tue, 10 Oct 2023 19:27:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40b483d55ec27555b481cb0fad97faf6e8d1686165905df945c86967ec0ac96`  
		Last Modified: Sat, 21 Oct 2023 00:09:50 GMT  
		Size: 5.3 MB (5268969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966ad11dd0f3a17ae3666a37f54fd9d6265bc0e18133314a565abf1039e90a1f`  
		Last Modified: Sat, 21 Oct 2023 00:09:50 GMT  
		Size: 1.2 MB (1186175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e18b62f88891e2a1b8f7a5e8a66e6ee69c9f42fe03945d66da418c55d339a9`  
		Last Modified: Sat, 21 Oct 2023 00:09:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:02d085e00e424e29b1a4c45b6358c9ac90629ed72540af87be474238770f3217
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76112263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fa19320a45d01205e0025f17edf0aa856b433bd25ee512a7877ec407bdf0a3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:44:44 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 12:29:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 12:29:18 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 12:29:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 12:29:51 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 12:29:52 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 12:29:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 12:29:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 12:29:54 GMT
WORKDIR /go
# Wed, 01 Nov 2023 16:51:53 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 16:51:55 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 16:51:56 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 16:51:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 16:51:57 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 16:51:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 16:52:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 16:52:01 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f15a4d38dd3d4f044868149900a763ac233f1aef33fe18019f45149b6bd02c`  
		Last Modified: Sat, 21 Oct 2023 00:45:00 GMT  
		Size: 285.1 KB (285095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23831500ce8c52e3d80c9eab9eb44d36e8daf00224a75f36d961186e47851ae8`  
		Last Modified: Wed, 01 Nov 2023 12:38:38 GMT  
		Size: 66.2 MB (66234435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92c933a1dfb2cbb65a33ccba713aabb9ff92ce6a0286e12af67e54c51be8a44`  
		Last Modified: Wed, 01 Nov 2023 12:38:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368a8f32c470e61e32632b0c78836e09dc1d70ab0e9a48e1c2bef1d23de82f7d`  
		Last Modified: Wed, 01 Nov 2023 16:52:34 GMT  
		Size: 5.1 MB (5114679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b61d54a31e32a9c971c8d7ea514537dababa89a4e60ce97eca5bdcf4e8d007`  
		Last Modified: Wed, 01 Nov 2023 16:52:33 GMT  
		Size: 1.3 MB (1262390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147c37f0535cd57e5355158d43aa5608a1430f56aa08ef1b4eb9cea12976a728`  
		Last Modified: Wed, 01 Nov 2023 16:52:33 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:c0740b75861440c921e23bec00c2ce3e14bda7ca7967b2aec7855352ea96cd0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull caddy@sha256:951876270030a4a5404a8bab425d35b64f90babc594bb65c261cc05eab33ed79
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2128478401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:883908294a37d78f29e796d389d42c83a12c68a6c0f1113bba3bdd9290db5b05`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 02:23:09 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Oct 2023 02:23:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Oct 2023 02:23:11 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Oct 2023 02:23:12 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Oct 2023 02:24:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:24:31 GMT
ENV GOPATH=C:\go
# Wed, 11 Oct 2023 02:25:33 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Oct 2023 02:25:34 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 11 Oct 2023 02:28:30 GMT
RUN $url = 'https://dl.google.com/go/go1.21.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '27c8daf157493f288d42a6f38debc6a2cb391f6543139eba9152fceca0be2a10'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:28:31 GMT
WORKDIR C:\go
# Wed, 11 Oct 2023 04:03:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:03:14 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 12 Oct 2023 01:42:14 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:42:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 12 Oct 2023 01:43:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 12 Oct 2023 01:43:13 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fded5ce3c59d7e8d637a5536d6eed085ff6b6a323f42c1df76a7be6e9970ee`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a72a6b595ab9f8f71a34a065e75e609b20ea5e026f901820fce6d3c9134939`  
		Last Modified: Wed, 11 Oct 2023 02:46:39 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2574f8b7fb0ec5a8c39ee40a8008f0d24c398380247bf7140be1abdede5542b`  
		Last Modified: Wed, 11 Oct 2023 02:46:40 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951c53676fe729ebf5d3c07215d91afa952e6190715f79a7952f4c3aa121231e`  
		Last Modified: Wed, 11 Oct 2023 02:46:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a382bb149b70b82f9c2f58ebf6a2672dc4c64460017836d73a5a23b7379ea095`  
		Last Modified: Wed, 11 Oct 2023 02:46:44 GMT  
		Size: 25.6 MB (25557568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608a2584f4b3b8f3038fa41c0719005822ab967d85d1231843bd729a7b3d2d60`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1058e02ad62f976d823e3035f0578b2868eb09f28986153342a52014cc5c3810`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 284.8 KB (284754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fce039c31b2e60b62a0ede9974b6574519f2e47e1d8f4e09c7a1f30763aee95`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65449f183261f9bbdb731d41f5e6fca94f3e547e8d996133e418773400cfcfe`  
		Last Modified: Wed, 11 Oct 2023 02:46:59 GMT  
		Size: 69.3 MB (69345382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394e07c2ad53e950c47ffb647836822197dc5f8ebe082eaa045854e2b25bafc7`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993f5e59c63ef5be894fc498ab0e165faa3129d35a8a8f5173f12c6a4232f588`  
		Last Modified: Wed, 11 Oct 2023 04:06:31 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c675831130735b443a544dff1b9c188928f34947a5342350ef04eadc0d1ab27`  
		Last Modified: Wed, 11 Oct 2023 04:06:28 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69fe7c1d1f5383a4421f2a0e7284e17db440ee5b7be9f487ce9048f76970e7b6`  
		Last Modified: Thu, 12 Oct 2023 01:45:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee998763c3cef90b11adda3322e66e1a89d89409d1ed29dd73a4101fb657e29`  
		Last Modified: Thu, 12 Oct 2023 01:45:21 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196a81b981d5dc89b19acce594b87914fc5bc4777e42b1322ca9b9d4c4b4f179`  
		Last Modified: Thu, 12 Oct 2023 01:45:22 GMT  
		Size: 1.7 MB (1682335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3ad6e4e7b1be08f8a79e4d77328648deded93f9ef0d4a1e8202ce4c3a21c67`  
		Last Modified: Thu, 12 Oct 2023 01:45:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:7a4eaeb7416d6a4b442d55eab7e8c7824e36a07baef33353084b943d46b6b7b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `caddy:2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull caddy@sha256:04b6c1b2519c8d35d65976c53b4523d7074d53c7b98fa5b29b83c837e021b493
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1956648108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6c3e402a7640df51573fae3237803e1e5fabce3d4c88849d9513c716654d474`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 02:19:41 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Oct 2023 02:19:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Oct 2023 02:19:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Oct 2023 02:19:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Oct 2023 02:20:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:20:18 GMT
ENV GOPATH=C:\go
# Wed, 11 Oct 2023 02:20:42 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Oct 2023 02:20:42 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 11 Oct 2023 02:22:59 GMT
RUN $url = 'https://dl.google.com/go/go1.21.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '27c8daf157493f288d42a6f38debc6a2cb391f6543139eba9152fceca0be2a10'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:23:01 GMT
WORKDIR C:\go
# Wed, 11 Oct 2023 04:04:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:04:42 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 12 Oct 2023 01:43:30 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:43:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 12 Oct 2023 01:43:51 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 12 Oct 2023 01:43:52 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60407a49ce6121c65fa6399c333c5227a09518414fd987c460ea29cb441ac5a`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe632e8cddda4e5f347720b87b8b3868e2e2969048761e3b0a40799d33f5f7a`  
		Last Modified: Wed, 11 Oct 2023 02:45:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4384696fc834e9658e7b3e5d1ceb1f8b362db85865daf29521b3c75c6999c046`  
		Last Modified: Wed, 11 Oct 2023 02:45:04 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c794ea611ef69f54d577f90b68e165e40a17e43b6d1d08f59951a38e084ea5fb`  
		Last Modified: Wed, 11 Oct 2023 02:45:03 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c74dc2d701da2bfabc4d44e6a4e6b92912515e2ca1fb053ffcc6b0d5cae2972`  
		Last Modified: Wed, 11 Oct 2023 02:45:08 GMT  
		Size: 25.5 MB (25531724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91612399ba7df8de0a05ad078c3817548f0a3b44516b76565e14a96ea62452e9`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7439c7c4353d2432c780827e4926910b19e84fe436d58e0a8129de2f631bd2b8`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 264.4 KB (264384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b0eaedd98e739ace4b7934261c71292195e461adcc977d02e57604d4a42ee8`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f46e84d4d007a200b1d6e7cb5b48db90116cdeb8bd3ec3964a08191875973e2`  
		Last Modified: Wed, 11 Oct 2023 02:45:25 GMT  
		Size: 69.3 MB (69325670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f59bab6d84ca44bbb60474dcf59c9af4f0f15edbdd64249b0eeaf968aff211f`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.6 KB (1556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f449f4d34d707dbde9cbb245c154c0b2e1d1a2c55d172501f8d7da576866f76f`  
		Last Modified: Wed, 11 Oct 2023 04:06:49 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a2edf76facdd17af03954b607484f7f7b36164a30634d19dd96b7320feb6b5`  
		Last Modified: Wed, 11 Oct 2023 04:06:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802c3686d509915fea71538d2c40c7a48c71719fab6144cb4497b6118b276ab9`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99cb183ed6cdad781eaba7bd1b4cb443befd9042c8a59450ee41f0245dd0ece4`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec33434b55fade6bcd7f3f0dfc10c981de93dc44bbae2b8702fdb6418a37a65b`  
		Last Modified: Thu, 12 Oct 2023 01:45:38 GMT  
		Size: 1.7 MB (1664788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0833369ef8236fcf99aba2d1fa48788db07662d0a9885a8429d435bf9f2227b2`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:b859825f1b8093a4b961d02fb945e63f5180c5e07e56ce7495384835c016c47d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4974; amd64
	-	windows version 10.0.20348.2031; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.4974; amd64

```console
$ docker pull caddy@sha256:77cb1b0b8315f376e69becef400d33c9d8b2a45548714845a821736158771de2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2047649951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3171dc2f25b4435520d8ba983ebf42f070ddec217b0da7677e309cc4cd51b05`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 03:59:19 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:39:06 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:40:04 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:40:05 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:40:06 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:40:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:40:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:40:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:40:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:40:12 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:40:13 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:41:01 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:41:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c4565a9b36858bc727874537e3c99968438a37e53c13057b0b1a233699d014`  
		Last Modified: Wed, 11 Oct 2023 04:05:44 GMT  
		Size: 472.0 KB (472034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df4a75108d3a33583e7ae61f1a019d4865860820bd89280ba414af94dd3f56e`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9dee9792a7bf7e1225840c56fb692536bee1743eba0a4da2faff34533f1160f`  
		Last Modified: Thu, 12 Oct 2023 01:44:37 GMT  
		Size: 15.3 MB (15296055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41900185a2519f01b8bd860f70936cee271612c4023512694b105826e0e0251`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0f1b69a12cd8550d868156e54168abaa32e1df40ee6eb39bc4e173ce04905e`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca266891343bff15b313846692ba3a41f313d5b228bedde964191332a16dffe`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12539eb7433a69ed67556d91b75b66dfedf0543d3efd7dabe82772437307a6f`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5103f279ed518bcfec88e00183e3222b50c1bc2f0e5b42f043e2198da424de98`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efc1cff2dac4308ce732a395ee215e1497d21f737e42e77917debf070afa8d7`  
		Last Modified: Thu, 12 Oct 2023 01:44:35 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cb50f59d2b11532a330925afb6ebd04d9b4708de8b11ae436e258c3764d741`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd11a311e4c0cf49bb544980f2c999751fc5e2fbe80d37b0f719f837abf8c3f`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ccbee9a6b9058ec933797dc1cfed875ceeb0115ce29ee163cd60a66e9f3b2d`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b486fc8ef055010a59374557443d3b713b9e55c1ccd11b7873f47876758976`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41df430d9a95c6000c922dd021b6cb2af0110dcc661ddc37a190a8cf6cd4bb06`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f243061a2e17d508efa4a424310d9ca158ca0cf0f59bd15cac606ab3e74701`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e709fff7d020a5d7c2d9e9e9a664c87392e9f9a4f4ced9802e64ca268995e23`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2c7aca9b511bc62340e6e8883d5f625bdccb805c4e897b837b68f3c79964b5`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38802c5a2b45b7029b250d88dac8209405146b0968925d1204cf17f7c3e76d98`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 269.1 KB (269086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376d19318a370d0da2ffcc29b47c2810278efa9d22fb39799c48687dfee0a2d9`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.20348.2031; amd64

```console
$ docker pull caddy@sha256:05f529a68927f0acfa7afbc79b7a19541f94430c137612ed344de7a822dcfafb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1875907229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8701a0e5aada270070acddeed89c57e20a5cac8afd88ed58da9557bf01dccb27`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:02:07 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:41:20 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:41:42 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:41:42 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:41:43 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:41:44 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:41:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:41:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:41:50 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:41:52 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:42:04 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:42:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c36616366b0df84f087a09bf19876f3872d839997f2f43e4eb8599861417c06`  
		Last Modified: Wed, 11 Oct 2023 04:06:10 GMT  
		Size: 467.9 KB (467933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db420ca589f10e4f9f5bc9dd6badc855d95c6a598888f2eb77a747eced259557`  
		Last Modified: Thu, 12 Oct 2023 01:45:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b5d7433dab05533d906a290a0f42cf31804c132da65c9fd7d4d2c41a64f519`  
		Last Modified: Thu, 12 Oct 2023 01:45:04 GMT  
		Size: 15.3 MB (15284209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62069fdf38bff9495ef2be05d397a55221536f9eec345734d6acec3a6196324f`  
		Last Modified: Thu, 12 Oct 2023 01:45:00 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e237a4c373c6937b5c51d0a3936152ac2b572fd5a432db3690f4070a7c78327`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73fae1c57e166a2ade87aa32e11980b456658212b296eea0f02ba3ec1c6557b`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000f2101dc464fa43321619c6e65c5b9e62b62755f3b141e69bd31892a253ded`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8536723423849b861a08fa490135f690c287be0144267e38fb3e631fb1bddbd2`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f176ef86531863755c3a315ec662b8da324474ae6097d7365dc18b76d61bde5`  
		Last Modified: Thu, 12 Oct 2023 01:44:58 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3973c168b3a63daa069e3a9870395561709d7b27762ffafb16538c773a16ad29`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5a10fbc59abc7ee7cc04a7ff48cc85983728745e91e8ef5fafee0589ba2193`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf033f8ab12414230e08aaada214c761777b0c784908ad2783ee31f8d330d0c9`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e2af83b2af59d76bd9b735c4e71b9492d9dbc120c042b8134ae0a70008f49`  
		Last Modified: Thu, 12 Oct 2023 01:44:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0355ed819405072f13996095ae7ec7044017bee81808dea9500459620118c20b`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e86117e27425829055f627e6156a4a657d9817cf8d2158f0026752366c9022c`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22fbe71be2fe08164a92f1362959f0a4aba194dcf931945d7bb2ac50e8f6467`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed768b9f807d51e5834f0bc8b2ea4dda09a5139d126f9141cb3db51f781ea541`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359fc3c79eda3ddbb39c46b09a4c68137a693a72f8712182d545c546b726027e`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 289.5 KB (289533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e4b8683a429393010114c6906acced22d65d5167cda2cc55238ae5b9f816c0`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:8169d134dfa19ddbba9eeeb7210c5227c2a61f00906c340474aab1250aba47f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull caddy@sha256:77cb1b0b8315f376e69becef400d33c9d8b2a45548714845a821736158771de2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2047649951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3171dc2f25b4435520d8ba983ebf42f070ddec217b0da7677e309cc4cd51b05`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 03:59:19 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:39:06 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:40:04 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:40:05 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:40:06 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:40:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:40:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:40:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:40:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:40:12 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:40:13 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:41:01 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:41:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c4565a9b36858bc727874537e3c99968438a37e53c13057b0b1a233699d014`  
		Last Modified: Wed, 11 Oct 2023 04:05:44 GMT  
		Size: 472.0 KB (472034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df4a75108d3a33583e7ae61f1a019d4865860820bd89280ba414af94dd3f56e`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9dee9792a7bf7e1225840c56fb692536bee1743eba0a4da2faff34533f1160f`  
		Last Modified: Thu, 12 Oct 2023 01:44:37 GMT  
		Size: 15.3 MB (15296055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41900185a2519f01b8bd860f70936cee271612c4023512694b105826e0e0251`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0f1b69a12cd8550d868156e54168abaa32e1df40ee6eb39bc4e173ce04905e`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca266891343bff15b313846692ba3a41f313d5b228bedde964191332a16dffe`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12539eb7433a69ed67556d91b75b66dfedf0543d3efd7dabe82772437307a6f`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5103f279ed518bcfec88e00183e3222b50c1bc2f0e5b42f043e2198da424de98`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efc1cff2dac4308ce732a395ee215e1497d21f737e42e77917debf070afa8d7`  
		Last Modified: Thu, 12 Oct 2023 01:44:35 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cb50f59d2b11532a330925afb6ebd04d9b4708de8b11ae436e258c3764d741`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd11a311e4c0cf49bb544980f2c999751fc5e2fbe80d37b0f719f837abf8c3f`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ccbee9a6b9058ec933797dc1cfed875ceeb0115ce29ee163cd60a66e9f3b2d`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b486fc8ef055010a59374557443d3b713b9e55c1ccd11b7873f47876758976`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41df430d9a95c6000c922dd021b6cb2af0110dcc661ddc37a190a8cf6cd4bb06`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f243061a2e17d508efa4a424310d9ca158ca0cf0f59bd15cac606ab3e74701`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e709fff7d020a5d7c2d9e9e9a664c87392e9f9a4f4ced9802e64ca268995e23`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2c7aca9b511bc62340e6e8883d5f625bdccb805c4e897b837b68f3c79964b5`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38802c5a2b45b7029b250d88dac8209405146b0968925d1204cf17f7c3e76d98`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 269.1 KB (269086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376d19318a370d0da2ffcc29b47c2810278efa9d22fb39799c48687dfee0a2d9`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:278d32be7fb2f9a5e3f48ea6a672747dbb4ad6256e4802aff4a1e11a67e2e518
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `caddy:2-windowsservercore-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull caddy@sha256:05f529a68927f0acfa7afbc79b7a19541f94430c137612ed344de7a822dcfafb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1875907229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8701a0e5aada270070acddeed89c57e20a5cac8afd88ed58da9557bf01dccb27`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:02:07 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:41:20 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:41:42 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:41:42 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:41:43 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:41:44 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:41:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:41:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:41:50 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:41:52 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:42:04 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:42:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c36616366b0df84f087a09bf19876f3872d839997f2f43e4eb8599861417c06`  
		Last Modified: Wed, 11 Oct 2023 04:06:10 GMT  
		Size: 467.9 KB (467933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db420ca589f10e4f9f5bc9dd6badc855d95c6a598888f2eb77a747eced259557`  
		Last Modified: Thu, 12 Oct 2023 01:45:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b5d7433dab05533d906a290a0f42cf31804c132da65c9fd7d4d2c41a64f519`  
		Last Modified: Thu, 12 Oct 2023 01:45:04 GMT  
		Size: 15.3 MB (15284209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62069fdf38bff9495ef2be05d397a55221536f9eec345734d6acec3a6196324f`  
		Last Modified: Thu, 12 Oct 2023 01:45:00 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e237a4c373c6937b5c51d0a3936152ac2b572fd5a432db3690f4070a7c78327`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73fae1c57e166a2ade87aa32e11980b456658212b296eea0f02ba3ec1c6557b`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000f2101dc464fa43321619c6e65c5b9e62b62755f3b141e69bd31892a253ded`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8536723423849b861a08fa490135f690c287be0144267e38fb3e631fb1bddbd2`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f176ef86531863755c3a315ec662b8da324474ae6097d7365dc18b76d61bde5`  
		Last Modified: Thu, 12 Oct 2023 01:44:58 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3973c168b3a63daa069e3a9870395561709d7b27762ffafb16538c773a16ad29`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5a10fbc59abc7ee7cc04a7ff48cc85983728745e91e8ef5fafee0589ba2193`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf033f8ab12414230e08aaada214c761777b0c784908ad2783ee31f8d330d0c9`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e2af83b2af59d76bd9b735c4e71b9492d9dbc120c042b8134ae0a70008f49`  
		Last Modified: Thu, 12 Oct 2023 01:44:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0355ed819405072f13996095ae7ec7044017bee81808dea9500459620118c20b`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e86117e27425829055f627e6156a4a657d9817cf8d2158f0026752366c9022c`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22fbe71be2fe08164a92f1362959f0a4aba194dcf931945d7bb2ac50e8f6467`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed768b9f807d51e5834f0bc8b2ea4dda09a5139d126f9141cb3db51f781ea541`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359fc3c79eda3ddbb39c46b09a4c68137a693a72f8712182d545c546b726027e`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 289.5 KB (289533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e4b8683a429393010114c6906acced22d65d5167cda2cc55238ae5b9f816c0`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7`

```console
$ docker pull caddy@sha256:325f81ca0328db0737503a53f43717fce79ea0c574e83f8e586c8d350cadf34b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4974; amd64
	-	windows version 10.0.20348.2031; amd64

### `caddy:2.7` - linux; amd64

```console
$ docker pull caddy@sha256:a9c7585fdc50bb28d686b73a9b1f0eb9a3d103efd63c48dc334ccb5f51aa1722
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18474311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70c3913f54e294079c54cc8b651576b08dd4add42a0f4c0bc93d539913ae335d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:11:11 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:11:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:11:12 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:11:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:11:15 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:11:15 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:11:16 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:11:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5433daac73cddf3f03243a31c38d460570073f83e9a8cf64c7f0e3387b85807`  
		Last Modified: Sat, 21 Oct 2023 00:11:36 GMT  
		Size: 350.8 KB (350840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c6b4aafe2c09344f58425bb0fe037a429808edb7b2ba37d79cd35b2775a422`  
		Last Modified: Sat, 21 Oct 2023 00:11:36 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a182bff4e1b33f3d5dd80f809e697793466287c3da7704863c3d0b51d42b5b`  
		Last Modified: Sat, 21 Oct 2023 00:11:39 GMT  
		Size: 14.7 MB (14713998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f43da8d65d754093117d4c673a7b725316be4e576e32b0d40c995e6ab1a07b7c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17422245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18b3bb2c3e0a97c9fe052eca67890f691907de7a5b514e88a44e660bb905079b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:06:46 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:06:48 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:06:48 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:06:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:06:51 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:06:51 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:06:52 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:06:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e09dc0459583a6ad3ba0428d5e180b7e3e6ae28360a69e293f03632cec397a0`  
		Last Modified: Sat, 21 Oct 2023 00:07:14 GMT  
		Size: 347.6 KB (347617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4705ff25da68d95a4bd671cbd4cec69369ea788be53bfafb45cdf4a930a725f8`  
		Last Modified: Sat, 21 Oct 2023 00:07:13 GMT  
		Size: 7.5 KB (7504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969c487cd333c7b53a7f57017e0ad77490d3806d9e52259caf9772016e96576d`  
		Last Modified: Sat, 21 Oct 2023 00:07:16 GMT  
		Size: 13.9 MB (13921833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - linux; arm variant v7

```console
$ docker pull caddy@sha256:dd028bb08526d3533680243c94b9464c9c1a6559dccf5dde3b61ec73b9afd002
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17155303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:539aa551acc109f33c6ea5076a1f518af4d0476b517dc698d98c7350e8cb1b1a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:17:55 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:17:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:17:56 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:17:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:17:59 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:17:59 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:18:00 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:18:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee93e167fdbd8e67ec3f4ed8eaf242e5c8022a9845dd4f797448503af15d777c`  
		Last Modified: Sat, 21 Oct 2023 00:18:22 GMT  
		Size: 344.5 KB (344454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2895c0143aa41e87473191f749160d3109330cdb9de0c90a9b0a9e60e8a3a3e`  
		Last Modified: Sat, 21 Oct 2023 00:18:22 GMT  
		Size: 7.5 KB (7508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f015da3d3488ea9171b2970be40718bfa7e31496bae565a9bc2b677e53c09915`  
		Last Modified: Sat, 21 Oct 2023 00:18:25 GMT  
		Size: 13.9 MB (13903436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:d18ec23ab87841ede7ccefc353c20d1554faddf3ac362213c32ae22311136da5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17273763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cbdde935029392921ca3521ef9ebdb6a2b46cd1d4b7a9dabf0b71b00c593572`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:23:28 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:23:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:23:29 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:23:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:23:31 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:23:31 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:23:32 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:23:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461fe4f467fe88a160e176c442825b4bfea8dde13fc2324393a5d81518375e6f`  
		Last Modified: Sat, 21 Oct 2023 00:23:52 GMT  
		Size: 360.6 KB (360623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9335adc9ff07e38d963f0a71a2f7db01b5b5ed8e9d93fba14e584f25ea05c29d`  
		Last Modified: Sat, 21 Oct 2023 00:23:52 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32426666f5ec8621a07038733361be24f83719a812c0cce54e3f41192b31c2d`  
		Last Modified: Sat, 21 Oct 2023 00:23:54 GMT  
		Size: 13.6 MB (13573803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - linux; ppc64le

```console
$ docker pull caddy@sha256:1cd57ee42a4e84e91731e9182350ab4fd5b26705ec7286c28c5768c549435fd5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.1 MB (17057167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5aa3d5c5c63bea353c483de170ae8690a4f7eb12042cb84dc2bf0d52bf914b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:09:00 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:09:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:09:02 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:09:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:09:05 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:09:05 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:09:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:09:09 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:09:09 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:09:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692440f8f5ba2c6efbf2e74e3301377e3d9a90ae5a7cbd728c771ab306277830`  
		Last Modified: Sat, 21 Oct 2023 00:09:34 GMT  
		Size: 362.2 KB (362183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2886f5cbb210969eea27d97b8a48d88cae7bbe1bdd528a2b2775a8affde3084`  
		Last Modified: Sat, 21 Oct 2023 00:09:33 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdd6a19a7b9d3f4621c5388c53b0a9ea5591e9e72250bc60bcf22ed672632b1`  
		Last Modified: Sat, 21 Oct 2023 00:09:36 GMT  
		Size: 13.3 MB (13340969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - linux; s390x

```console
$ docker pull caddy@sha256:7dc6afd9bb40ff4450e4282bc56431b993d068c5b832c914dd50831189920061
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.8 MB (17822696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be3873facfc56aac0a1a9659efab4cddfc06afe6ac27c54cdd1b6fc9a23f1c1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:05:23 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:05:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:05:24 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:05:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:05:27 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:05:27 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:05:29 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:05:29 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:05:29 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d6d08cebdb83ff91ba335e0c4aec115b17261ed40307aaee6adde8c6763ad6`  
		Last Modified: Sat, 21 Oct 2023 00:06:00 GMT  
		Size: 355.0 KB (354963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58e0c7856c877cacd1d63a86beb12c9be91c4a0950dd85954db6f16a6d93103`  
		Last Modified: Sat, 21 Oct 2023 00:06:00 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69bf19674eec620ff3f87ecb754c60b7c137eb6c8c3763ff795739061593a77`  
		Last Modified: Sat, 21 Oct 2023 00:06:02 GMT  
		Size: 14.2 MB (14245123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - windows version 10.0.17763.4974; amd64

```console
$ docker pull caddy@sha256:77cb1b0b8315f376e69becef400d33c9d8b2a45548714845a821736158771de2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2047649951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3171dc2f25b4435520d8ba983ebf42f070ddec217b0da7677e309cc4cd51b05`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 03:59:19 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:39:06 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:40:04 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:40:05 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:40:06 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:40:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:40:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:40:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:40:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:40:12 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:40:13 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:41:01 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:41:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c4565a9b36858bc727874537e3c99968438a37e53c13057b0b1a233699d014`  
		Last Modified: Wed, 11 Oct 2023 04:05:44 GMT  
		Size: 472.0 KB (472034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df4a75108d3a33583e7ae61f1a019d4865860820bd89280ba414af94dd3f56e`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9dee9792a7bf7e1225840c56fb692536bee1743eba0a4da2faff34533f1160f`  
		Last Modified: Thu, 12 Oct 2023 01:44:37 GMT  
		Size: 15.3 MB (15296055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41900185a2519f01b8bd860f70936cee271612c4023512694b105826e0e0251`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0f1b69a12cd8550d868156e54168abaa32e1df40ee6eb39bc4e173ce04905e`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca266891343bff15b313846692ba3a41f313d5b228bedde964191332a16dffe`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12539eb7433a69ed67556d91b75b66dfedf0543d3efd7dabe82772437307a6f`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5103f279ed518bcfec88e00183e3222b50c1bc2f0e5b42f043e2198da424de98`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efc1cff2dac4308ce732a395ee215e1497d21f737e42e77917debf070afa8d7`  
		Last Modified: Thu, 12 Oct 2023 01:44:35 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cb50f59d2b11532a330925afb6ebd04d9b4708de8b11ae436e258c3764d741`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd11a311e4c0cf49bb544980f2c999751fc5e2fbe80d37b0f719f837abf8c3f`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ccbee9a6b9058ec933797dc1cfed875ceeb0115ce29ee163cd60a66e9f3b2d`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b486fc8ef055010a59374557443d3b713b9e55c1ccd11b7873f47876758976`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41df430d9a95c6000c922dd021b6cb2af0110dcc661ddc37a190a8cf6cd4bb06`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f243061a2e17d508efa4a424310d9ca158ca0cf0f59bd15cac606ab3e74701`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e709fff7d020a5d7c2d9e9e9a664c87392e9f9a4f4ced9802e64ca268995e23`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2c7aca9b511bc62340e6e8883d5f625bdccb805c4e897b837b68f3c79964b5`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38802c5a2b45b7029b250d88dac8209405146b0968925d1204cf17f7c3e76d98`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 269.1 KB (269086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376d19318a370d0da2ffcc29b47c2810278efa9d22fb39799c48687dfee0a2d9`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - windows version 10.0.20348.2031; amd64

```console
$ docker pull caddy@sha256:05f529a68927f0acfa7afbc79b7a19541f94430c137612ed344de7a822dcfafb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1875907229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8701a0e5aada270070acddeed89c57e20a5cac8afd88ed58da9557bf01dccb27`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:02:07 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:41:20 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:41:42 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:41:42 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:41:43 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:41:44 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:41:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:41:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:41:50 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:41:52 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:42:04 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:42:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c36616366b0df84f087a09bf19876f3872d839997f2f43e4eb8599861417c06`  
		Last Modified: Wed, 11 Oct 2023 04:06:10 GMT  
		Size: 467.9 KB (467933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db420ca589f10e4f9f5bc9dd6badc855d95c6a598888f2eb77a747eced259557`  
		Last Modified: Thu, 12 Oct 2023 01:45:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b5d7433dab05533d906a290a0f42cf31804c132da65c9fd7d4d2c41a64f519`  
		Last Modified: Thu, 12 Oct 2023 01:45:04 GMT  
		Size: 15.3 MB (15284209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62069fdf38bff9495ef2be05d397a55221536f9eec345734d6acec3a6196324f`  
		Last Modified: Thu, 12 Oct 2023 01:45:00 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e237a4c373c6937b5c51d0a3936152ac2b572fd5a432db3690f4070a7c78327`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73fae1c57e166a2ade87aa32e11980b456658212b296eea0f02ba3ec1c6557b`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000f2101dc464fa43321619c6e65c5b9e62b62755f3b141e69bd31892a253ded`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8536723423849b861a08fa490135f690c287be0144267e38fb3e631fb1bddbd2`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f176ef86531863755c3a315ec662b8da324474ae6097d7365dc18b76d61bde5`  
		Last Modified: Thu, 12 Oct 2023 01:44:58 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3973c168b3a63daa069e3a9870395561709d7b27762ffafb16538c773a16ad29`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5a10fbc59abc7ee7cc04a7ff48cc85983728745e91e8ef5fafee0589ba2193`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf033f8ab12414230e08aaada214c761777b0c784908ad2783ee31f8d330d0c9`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e2af83b2af59d76bd9b735c4e71b9492d9dbc120c042b8134ae0a70008f49`  
		Last Modified: Thu, 12 Oct 2023 01:44:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0355ed819405072f13996095ae7ec7044017bee81808dea9500459620118c20b`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e86117e27425829055f627e6156a4a657d9817cf8d2158f0026752366c9022c`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22fbe71be2fe08164a92f1362959f0a4aba194dcf931945d7bb2ac50e8f6467`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed768b9f807d51e5834f0bc8b2ea4dda09a5139d126f9141cb3db51f781ea541`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359fc3c79eda3ddbb39c46b09a4c68137a693a72f8712182d545c546b726027e`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 289.5 KB (289533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e4b8683a429393010114c6906acced22d65d5167cda2cc55238ae5b9f816c0`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-alpine`

```console
$ docker pull caddy@sha256:f1c092da9fcba7a8197cf1065a347d4f0bb67b6dd188985eafaf0a5aec6c9041
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.7-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:a9c7585fdc50bb28d686b73a9b1f0eb9a3d103efd63c48dc334ccb5f51aa1722
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18474311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70c3913f54e294079c54cc8b651576b08dd4add42a0f4c0bc93d539913ae335d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:11:11 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:11:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:11:12 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:11:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:11:15 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:11:15 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:11:16 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:11:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5433daac73cddf3f03243a31c38d460570073f83e9a8cf64c7f0e3387b85807`  
		Last Modified: Sat, 21 Oct 2023 00:11:36 GMT  
		Size: 350.8 KB (350840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c6b4aafe2c09344f58425bb0fe037a429808edb7b2ba37d79cd35b2775a422`  
		Last Modified: Sat, 21 Oct 2023 00:11:36 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a182bff4e1b33f3d5dd80f809e697793466287c3da7704863c3d0b51d42b5b`  
		Last Modified: Sat, 21 Oct 2023 00:11:39 GMT  
		Size: 14.7 MB (14713998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f43da8d65d754093117d4c673a7b725316be4e576e32b0d40c995e6ab1a07b7c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17422245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18b3bb2c3e0a97c9fe052eca67890f691907de7a5b514e88a44e660bb905079b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:06:46 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:06:48 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:06:48 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:06:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:06:51 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:06:51 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:06:52 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:06:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e09dc0459583a6ad3ba0428d5e180b7e3e6ae28360a69e293f03632cec397a0`  
		Last Modified: Sat, 21 Oct 2023 00:07:14 GMT  
		Size: 347.6 KB (347617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4705ff25da68d95a4bd671cbd4cec69369ea788be53bfafb45cdf4a930a725f8`  
		Last Modified: Sat, 21 Oct 2023 00:07:13 GMT  
		Size: 7.5 KB (7504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969c487cd333c7b53a7f57017e0ad77490d3806d9e52259caf9772016e96576d`  
		Last Modified: Sat, 21 Oct 2023 00:07:16 GMT  
		Size: 13.9 MB (13921833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:dd028bb08526d3533680243c94b9464c9c1a6559dccf5dde3b61ec73b9afd002
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17155303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:539aa551acc109f33c6ea5076a1f518af4d0476b517dc698d98c7350e8cb1b1a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:17:55 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:17:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:17:56 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:17:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:17:59 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:17:59 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:18:00 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:18:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee93e167fdbd8e67ec3f4ed8eaf242e5c8022a9845dd4f797448503af15d777c`  
		Last Modified: Sat, 21 Oct 2023 00:18:22 GMT  
		Size: 344.5 KB (344454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2895c0143aa41e87473191f749160d3109330cdb9de0c90a9b0a9e60e8a3a3e`  
		Last Modified: Sat, 21 Oct 2023 00:18:22 GMT  
		Size: 7.5 KB (7508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f015da3d3488ea9171b2970be40718bfa7e31496bae565a9bc2b677e53c09915`  
		Last Modified: Sat, 21 Oct 2023 00:18:25 GMT  
		Size: 13.9 MB (13903436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:d18ec23ab87841ede7ccefc353c20d1554faddf3ac362213c32ae22311136da5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17273763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cbdde935029392921ca3521ef9ebdb6a2b46cd1d4b7a9dabf0b71b00c593572`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:23:28 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:23:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:23:29 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:23:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:23:31 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:23:31 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:23:32 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:23:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461fe4f467fe88a160e176c442825b4bfea8dde13fc2324393a5d81518375e6f`  
		Last Modified: Sat, 21 Oct 2023 00:23:52 GMT  
		Size: 360.6 KB (360623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9335adc9ff07e38d963f0a71a2f7db01b5b5ed8e9d93fba14e584f25ea05c29d`  
		Last Modified: Sat, 21 Oct 2023 00:23:52 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32426666f5ec8621a07038733361be24f83719a812c0cce54e3f41192b31c2d`  
		Last Modified: Sat, 21 Oct 2023 00:23:54 GMT  
		Size: 13.6 MB (13573803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:1cd57ee42a4e84e91731e9182350ab4fd5b26705ec7286c28c5768c549435fd5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.1 MB (17057167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5aa3d5c5c63bea353c483de170ae8690a4f7eb12042cb84dc2bf0d52bf914b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:09:00 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:09:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:09:02 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:09:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:09:05 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:09:05 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:09:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:09:09 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:09:09 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:09:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692440f8f5ba2c6efbf2e74e3301377e3d9a90ae5a7cbd728c771ab306277830`  
		Last Modified: Sat, 21 Oct 2023 00:09:34 GMT  
		Size: 362.2 KB (362183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2886f5cbb210969eea27d97b8a48d88cae7bbe1bdd528a2b2775a8affde3084`  
		Last Modified: Sat, 21 Oct 2023 00:09:33 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdd6a19a7b9d3f4621c5388c53b0a9ea5591e9e72250bc60bcf22ed672632b1`  
		Last Modified: Sat, 21 Oct 2023 00:09:36 GMT  
		Size: 13.3 MB (13340969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:7dc6afd9bb40ff4450e4282bc56431b993d068c5b832c914dd50831189920061
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.8 MB (17822696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be3873facfc56aac0a1a9659efab4cddfc06afe6ac27c54cdd1b6fc9a23f1c1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:05:23 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:05:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:05:24 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:05:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:05:27 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:05:27 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:05:29 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:05:29 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:05:29 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d6d08cebdb83ff91ba335e0c4aec115b17261ed40307aaee6adde8c6763ad6`  
		Last Modified: Sat, 21 Oct 2023 00:06:00 GMT  
		Size: 355.0 KB (354963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58e0c7856c877cacd1d63a86beb12c9be91c4a0950dd85954db6f16a6d93103`  
		Last Modified: Sat, 21 Oct 2023 00:06:00 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69bf19674eec620ff3f87ecb754c60b7c137eb6c8c3763ff795739061593a77`  
		Last Modified: Sat, 21 Oct 2023 00:06:02 GMT  
		Size: 14.2 MB (14245123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-builder`

```console
$ docker pull caddy@sha256:d039cffaec2ce64db9cae84dc789bb36c8d3d09e6ff70f3a40c4f405a89deed8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4974; amd64
	-	windows version 10.0.20348.2031; amd64

### `caddy:2.7-builder` - linux; amd64

```console
$ docker pull caddy@sha256:d1f6d3dcfec129b4d0e23b6743f576807352958232a7ac6c17ee36f785fe5c58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76972374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e113a57232410dd987d12708b35062e6a269825fa7b4d03aef42c00acc93dce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:54:30 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:54:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:20:11 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:20:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 19:20:22 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:20:22 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:20:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:20:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:20:23 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:11:20 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:11:20 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:11:20 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:11:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:11:21 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:11:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:11:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:11:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc37b24bb09971feb8bf4882e861bce9db0c985a16a900adb0dc9de3f854243b`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 284.7 KB (284690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a4303e95078c253686dcc16d7717644af63809efcbd753c0a999c9aad3fe72`  
		Last Modified: Tue, 10 Oct 2023 19:26:17 GMT  
		Size: 67.0 MB (67012876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359925be0f358b952dc8be63647139c5aab0fff94f7a070d88cb51dd258f80e5`  
		Last Modified: Tue, 10 Oct 2023 19:26:06 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958092cb44d28ddde181d193284001b1146b33a1cf19624e9683fc8f31551043`  
		Last Modified: Sat, 21 Oct 2023 00:11:52 GMT  
		Size: 5.0 MB (4970044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85cdb072dd78dcf6a7b04409cf7c8dc1fddddf912b601b15c6dc94adb2df10b`  
		Last Modified: Sat, 21 Oct 2023 00:11:51 GMT  
		Size: 1.3 MB (1302237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32749367842b0c8b40e7f61a315ff21b4d42211b5399e648beb75d86acb29c4c`  
		Last Modified: Sat, 21 Oct 2023 00:11:51 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:15f0db6d62062758441d2d22fd178c42299cf148c5097ffe10468153ff40c6b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75413855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:509cf858d9f3ffa4a94fe988705864c41bd510f34ade4ece0d2ede4cda23599f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:55:22 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:55:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 18:49:21 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 18:49:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 18:49:42 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 18:49:42 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 18:49:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 18:49:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 18:49:43 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:06:57 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:06:57 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:06:58 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:06:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:06:58 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:06:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:06:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:06:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3da3b9e7a12f6bb6b7f56e9240c2c92ce8c9f5fd5ef3b3063b9a93d454919e`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 284.9 KB (284887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbbb7b34bc324d050e49d3dd31294bdde5d6ecda33decf9afe31c11165b138a`  
		Last Modified: Tue, 10 Oct 2023 18:55:32 GMT  
		Size: 65.8 MB (65770135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c022f45a9fb1e7649eb4a663acd4ed6437363b4fc6e56f6af3e5f457a5d06ee8`  
		Last Modified: Tue, 10 Oct 2023 18:55:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12bec1760d3cf2773adbb14bd47431e46e130a914a46535c9a70de28e4b363b`  
		Last Modified: Sat, 21 Oct 2023 00:07:30 GMT  
		Size: 5.0 MB (4964316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888b304960048015ef929fcb0ffab750c1ba463aaf1d419272f2233e67195d56`  
		Last Modified: Sat, 21 Oct 2023 00:07:30 GMT  
		Size: 1.2 MB (1248665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00237a85b25c3b9ee3968fe9e98da8f378a4a70ccc746a6524820916085348ef`  
		Last Modified: Sat, 21 Oct 2023 00:07:29 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9275f10d0ef0db0999dc5ed6b19c068a941f59a05d69fad4b3cb07c3f0b14a7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74714658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b10f4fd814dc9e97d1147715baacffedd007b23ec081f4c100520df02050e6c9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:07:30 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 15:58:50 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:58:50 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 15:59:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 15:59:08 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 15:59:08 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 15:59:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:59:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 15:59:09 GMT
WORKDIR /go
# Wed, 01 Nov 2023 21:17:21 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 21:17:22 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 21:17:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 21:17:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 21:17:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8457acc181d300b4231b44e12aa0bf4a99ced5d51c5dfdc14eb899a341d5b855`  
		Last Modified: Sat, 21 Oct 2023 01:07:42 GMT  
		Size: 284.1 KB (284074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05626b790821d279bd9aea8466a1a79307764cbc389c51ab081a4b98c7657dc2`  
		Last Modified: Wed, 01 Nov 2023 16:06:11 GMT  
		Size: 65.8 MB (65772806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2dba3cbff62191bbc046c664eead34e3af26adfa5ecdbacf0ba6e73b9cbe51`  
		Last Modified: Wed, 01 Nov 2023 16:05:56 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357de4175525102c1d6c8d4fc605461ca1b1791b2a3b6c55c73e3ef6266159ad`  
		Last Modified: Wed, 01 Nov 2023 21:17:50 GMT  
		Size: 4.5 MB (4511226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59aa4bdeb70fa8c96a09911a5e79184a493cb38488e04d22007af9f9164e4f44`  
		Last Modified: Wed, 01 Nov 2023 21:17:50 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7b450bb18e60383a1dd8c51f37de16c5782ba7eba9e2737540247f3a4394c8`  
		Last Modified: Wed, 01 Nov 2023 21:17:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:76d3844fa9c17929397bb168745241a1f8fa36bf63c437d9d255fe217ec6a87c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73995976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6b4383d952151327974f3f21fa7be1e862f9a67c4ee08a264948e4372890be6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 02:41:07 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 15:36:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:36:13 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 15:36:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 15:36:23 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 15:36:23 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 15:36:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:36:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 15:36:24 GMT
WORKDIR /go
# Wed, 01 Nov 2023 19:56:22 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 19:56:22 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 19:56:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 19:56:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 19:56:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74bf0db6f91dfe1899e8204affb86f8c505a5643bdcb83b085888c86e0c7411`  
		Last Modified: Sat, 21 Oct 2023 02:41:18 GMT  
		Size: 286.3 KB (286297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd442d12e388d3f44ee4325caf9e959ca82d4064c8b1b38321da75a84a6ccbd`  
		Last Modified: Wed, 01 Nov 2023 15:41:04 GMT  
		Size: 64.1 MB (64110459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0297817440f5024a6c0e27f7906a375aa91aea5aaf191caa3f1762426e60e9c2`  
		Last Modified: Wed, 01 Nov 2023 15:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9fb63180b1c62b2cfd436428dc31a25bc97989024e217b9d8e508e82b0b287`  
		Last Modified: Wed, 01 Nov 2023 19:56:42 GMT  
		Size: 5.1 MB (5068382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0ee6df11f2e2e143f36f30697c4b309c4560fa062faa2fcb3a1c22db91257e`  
		Last Modified: Wed, 01 Nov 2023 19:56:42 GMT  
		Size: 1.2 MB (1198448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15b8268dd8cba7445da5d02c68c6787ce774d7ecc7dba9fa3f2775a88884d64`  
		Last Modified: Wed, 01 Nov 2023 19:56:41 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:ed1e2679ee802b3a2c8f7b42d4828ecc9ba50b5a029e3d14bbc54fa2a0fc5444
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74214117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2041e14adf1ce1c2b331135049ec2871be632eb2a7130142af035fa662cb1e19`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:13:11 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:13:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:17:44 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:18:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 19:18:14 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:18:14 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:18:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:18:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:18:17 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:09:16 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:09:17 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:09:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:09:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:09:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc67971d1767eae5019ffeaf8f893e6d81dbba50bde347da0c0433c56e3f2a3`  
		Last Modified: Thu, 28 Sep 2023 22:18:17 GMT  
		Size: 286.7 KB (286659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1caf7fa003bdf7c7611eb2e33a11db077a0f632b70d28f5b73096bf051f25aeb`  
		Last Modified: Tue, 10 Oct 2023 19:28:09 GMT  
		Size: 64.1 MB (64125245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9573c5aef56335266ce720d0812f9a0156f628fbd01ba4a6462be56d8742dc8a`  
		Last Modified: Tue, 10 Oct 2023 19:27:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40b483d55ec27555b481cb0fad97faf6e8d1686165905df945c86967ec0ac96`  
		Last Modified: Sat, 21 Oct 2023 00:09:50 GMT  
		Size: 5.3 MB (5268969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966ad11dd0f3a17ae3666a37f54fd9d6265bc0e18133314a565abf1039e90a1f`  
		Last Modified: Sat, 21 Oct 2023 00:09:50 GMT  
		Size: 1.2 MB (1186175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e18b62f88891e2a1b8f7a5e8a66e6ee69c9f42fe03945d66da418c55d339a9`  
		Last Modified: Sat, 21 Oct 2023 00:09:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; s390x

```console
$ docker pull caddy@sha256:02d085e00e424e29b1a4c45b6358c9ac90629ed72540af87be474238770f3217
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76112263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fa19320a45d01205e0025f17edf0aa856b433bd25ee512a7877ec407bdf0a3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:44:44 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 12:29:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 12:29:18 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 12:29:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 12:29:51 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 12:29:52 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 12:29:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 12:29:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 12:29:54 GMT
WORKDIR /go
# Wed, 01 Nov 2023 16:51:53 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 16:51:55 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 16:51:56 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 16:51:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 16:51:57 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 16:51:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 16:52:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 16:52:01 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f15a4d38dd3d4f044868149900a763ac233f1aef33fe18019f45149b6bd02c`  
		Last Modified: Sat, 21 Oct 2023 00:45:00 GMT  
		Size: 285.1 KB (285095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23831500ce8c52e3d80c9eab9eb44d36e8daf00224a75f36d961186e47851ae8`  
		Last Modified: Wed, 01 Nov 2023 12:38:38 GMT  
		Size: 66.2 MB (66234435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92c933a1dfb2cbb65a33ccba713aabb9ff92ce6a0286e12af67e54c51be8a44`  
		Last Modified: Wed, 01 Nov 2023 12:38:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368a8f32c470e61e32632b0c78836e09dc1d70ab0e9a48e1c2bef1d23de82f7d`  
		Last Modified: Wed, 01 Nov 2023 16:52:34 GMT  
		Size: 5.1 MB (5114679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b61d54a31e32a9c971c8d7ea514537dababa89a4e60ce97eca5bdcf4e8d007`  
		Last Modified: Wed, 01 Nov 2023 16:52:33 GMT  
		Size: 1.3 MB (1262390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147c37f0535cd57e5355158d43aa5608a1430f56aa08ef1b4eb9cea12976a728`  
		Last Modified: Wed, 01 Nov 2023 16:52:33 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - windows version 10.0.17763.4974; amd64

```console
$ docker pull caddy@sha256:951876270030a4a5404a8bab425d35b64f90babc594bb65c261cc05eab33ed79
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2128478401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:883908294a37d78f29e796d389d42c83a12c68a6c0f1113bba3bdd9290db5b05`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 02:23:09 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Oct 2023 02:23:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Oct 2023 02:23:11 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Oct 2023 02:23:12 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Oct 2023 02:24:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:24:31 GMT
ENV GOPATH=C:\go
# Wed, 11 Oct 2023 02:25:33 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Oct 2023 02:25:34 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 11 Oct 2023 02:28:30 GMT
RUN $url = 'https://dl.google.com/go/go1.21.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '27c8daf157493f288d42a6f38debc6a2cb391f6543139eba9152fceca0be2a10'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:28:31 GMT
WORKDIR C:\go
# Wed, 11 Oct 2023 04:03:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:03:14 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 12 Oct 2023 01:42:14 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:42:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 12 Oct 2023 01:43:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 12 Oct 2023 01:43:13 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fded5ce3c59d7e8d637a5536d6eed085ff6b6a323f42c1df76a7be6e9970ee`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a72a6b595ab9f8f71a34a065e75e609b20ea5e026f901820fce6d3c9134939`  
		Last Modified: Wed, 11 Oct 2023 02:46:39 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2574f8b7fb0ec5a8c39ee40a8008f0d24c398380247bf7140be1abdede5542b`  
		Last Modified: Wed, 11 Oct 2023 02:46:40 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951c53676fe729ebf5d3c07215d91afa952e6190715f79a7952f4c3aa121231e`  
		Last Modified: Wed, 11 Oct 2023 02:46:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a382bb149b70b82f9c2f58ebf6a2672dc4c64460017836d73a5a23b7379ea095`  
		Last Modified: Wed, 11 Oct 2023 02:46:44 GMT  
		Size: 25.6 MB (25557568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608a2584f4b3b8f3038fa41c0719005822ab967d85d1231843bd729a7b3d2d60`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1058e02ad62f976d823e3035f0578b2868eb09f28986153342a52014cc5c3810`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 284.8 KB (284754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fce039c31b2e60b62a0ede9974b6574519f2e47e1d8f4e09c7a1f30763aee95`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65449f183261f9bbdb731d41f5e6fca94f3e547e8d996133e418773400cfcfe`  
		Last Modified: Wed, 11 Oct 2023 02:46:59 GMT  
		Size: 69.3 MB (69345382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394e07c2ad53e950c47ffb647836822197dc5f8ebe082eaa045854e2b25bafc7`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993f5e59c63ef5be894fc498ab0e165faa3129d35a8a8f5173f12c6a4232f588`  
		Last Modified: Wed, 11 Oct 2023 04:06:31 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c675831130735b443a544dff1b9c188928f34947a5342350ef04eadc0d1ab27`  
		Last Modified: Wed, 11 Oct 2023 04:06:28 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69fe7c1d1f5383a4421f2a0e7284e17db440ee5b7be9f487ce9048f76970e7b6`  
		Last Modified: Thu, 12 Oct 2023 01:45:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee998763c3cef90b11adda3322e66e1a89d89409d1ed29dd73a4101fb657e29`  
		Last Modified: Thu, 12 Oct 2023 01:45:21 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196a81b981d5dc89b19acce594b87914fc5bc4777e42b1322ca9b9d4c4b4f179`  
		Last Modified: Thu, 12 Oct 2023 01:45:22 GMT  
		Size: 1.7 MB (1682335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3ad6e4e7b1be08f8a79e4d77328648deded93f9ef0d4a1e8202ce4c3a21c67`  
		Last Modified: Thu, 12 Oct 2023 01:45:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - windows version 10.0.20348.2031; amd64

```console
$ docker pull caddy@sha256:04b6c1b2519c8d35d65976c53b4523d7074d53c7b98fa5b29b83c837e021b493
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1956648108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6c3e402a7640df51573fae3237803e1e5fabce3d4c88849d9513c716654d474`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 02:19:41 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Oct 2023 02:19:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Oct 2023 02:19:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Oct 2023 02:19:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Oct 2023 02:20:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:20:18 GMT
ENV GOPATH=C:\go
# Wed, 11 Oct 2023 02:20:42 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Oct 2023 02:20:42 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 11 Oct 2023 02:22:59 GMT
RUN $url = 'https://dl.google.com/go/go1.21.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '27c8daf157493f288d42a6f38debc6a2cb391f6543139eba9152fceca0be2a10'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:23:01 GMT
WORKDIR C:\go
# Wed, 11 Oct 2023 04:04:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:04:42 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 12 Oct 2023 01:43:30 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:43:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 12 Oct 2023 01:43:51 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 12 Oct 2023 01:43:52 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60407a49ce6121c65fa6399c333c5227a09518414fd987c460ea29cb441ac5a`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe632e8cddda4e5f347720b87b8b3868e2e2969048761e3b0a40799d33f5f7a`  
		Last Modified: Wed, 11 Oct 2023 02:45:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4384696fc834e9658e7b3e5d1ceb1f8b362db85865daf29521b3c75c6999c046`  
		Last Modified: Wed, 11 Oct 2023 02:45:04 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c794ea611ef69f54d577f90b68e165e40a17e43b6d1d08f59951a38e084ea5fb`  
		Last Modified: Wed, 11 Oct 2023 02:45:03 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c74dc2d701da2bfabc4d44e6a4e6b92912515e2ca1fb053ffcc6b0d5cae2972`  
		Last Modified: Wed, 11 Oct 2023 02:45:08 GMT  
		Size: 25.5 MB (25531724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91612399ba7df8de0a05ad078c3817548f0a3b44516b76565e14a96ea62452e9`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7439c7c4353d2432c780827e4926910b19e84fe436d58e0a8129de2f631bd2b8`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 264.4 KB (264384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b0eaedd98e739ace4b7934261c71292195e461adcc977d02e57604d4a42ee8`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f46e84d4d007a200b1d6e7cb5b48db90116cdeb8bd3ec3964a08191875973e2`  
		Last Modified: Wed, 11 Oct 2023 02:45:25 GMT  
		Size: 69.3 MB (69325670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f59bab6d84ca44bbb60474dcf59c9af4f0f15edbdd64249b0eeaf968aff211f`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.6 KB (1556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f449f4d34d707dbde9cbb245c154c0b2e1d1a2c55d172501f8d7da576866f76f`  
		Last Modified: Wed, 11 Oct 2023 04:06:49 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a2edf76facdd17af03954b607484f7f7b36164a30634d19dd96b7320feb6b5`  
		Last Modified: Wed, 11 Oct 2023 04:06:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802c3686d509915fea71538d2c40c7a48c71719fab6144cb4497b6118b276ab9`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99cb183ed6cdad781eaba7bd1b4cb443befd9042c8a59450ee41f0245dd0ece4`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec33434b55fade6bcd7f3f0dfc10c981de93dc44bbae2b8702fdb6418a37a65b`  
		Last Modified: Thu, 12 Oct 2023 01:45:38 GMT  
		Size: 1.7 MB (1664788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0833369ef8236fcf99aba2d1fa48788db07662d0a9885a8429d435bf9f2227b2`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-builder-alpine`

```console
$ docker pull caddy@sha256:0b6ab47c59512267b3021fcb39af41d2896fd78718a39fa127cc8f2a4795638e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.7-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:d1f6d3dcfec129b4d0e23b6743f576807352958232a7ac6c17ee36f785fe5c58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76972374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e113a57232410dd987d12708b35062e6a269825fa7b4d03aef42c00acc93dce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:54:30 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:54:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:20:11 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:20:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 19:20:22 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:20:22 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:20:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:20:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:20:23 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:11:20 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:11:20 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:11:20 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:11:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:11:21 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:11:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:11:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:11:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc37b24bb09971feb8bf4882e861bce9db0c985a16a900adb0dc9de3f854243b`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 284.7 KB (284690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a4303e95078c253686dcc16d7717644af63809efcbd753c0a999c9aad3fe72`  
		Last Modified: Tue, 10 Oct 2023 19:26:17 GMT  
		Size: 67.0 MB (67012876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359925be0f358b952dc8be63647139c5aab0fff94f7a070d88cb51dd258f80e5`  
		Last Modified: Tue, 10 Oct 2023 19:26:06 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958092cb44d28ddde181d193284001b1146b33a1cf19624e9683fc8f31551043`  
		Last Modified: Sat, 21 Oct 2023 00:11:52 GMT  
		Size: 5.0 MB (4970044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85cdb072dd78dcf6a7b04409cf7c8dc1fddddf912b601b15c6dc94adb2df10b`  
		Last Modified: Sat, 21 Oct 2023 00:11:51 GMT  
		Size: 1.3 MB (1302237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32749367842b0c8b40e7f61a315ff21b4d42211b5399e648beb75d86acb29c4c`  
		Last Modified: Sat, 21 Oct 2023 00:11:51 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:15f0db6d62062758441d2d22fd178c42299cf148c5097ffe10468153ff40c6b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75413855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:509cf858d9f3ffa4a94fe988705864c41bd510f34ade4ece0d2ede4cda23599f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:55:22 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:55:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 18:49:21 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 18:49:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 18:49:42 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 18:49:42 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 18:49:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 18:49:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 18:49:43 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:06:57 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:06:57 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:06:58 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:06:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:06:58 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:06:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:06:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:06:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3da3b9e7a12f6bb6b7f56e9240c2c92ce8c9f5fd5ef3b3063b9a93d454919e`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 284.9 KB (284887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbbb7b34bc324d050e49d3dd31294bdde5d6ecda33decf9afe31c11165b138a`  
		Last Modified: Tue, 10 Oct 2023 18:55:32 GMT  
		Size: 65.8 MB (65770135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c022f45a9fb1e7649eb4a663acd4ed6437363b4fc6e56f6af3e5f457a5d06ee8`  
		Last Modified: Tue, 10 Oct 2023 18:55:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12bec1760d3cf2773adbb14bd47431e46e130a914a46535c9a70de28e4b363b`  
		Last Modified: Sat, 21 Oct 2023 00:07:30 GMT  
		Size: 5.0 MB (4964316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888b304960048015ef929fcb0ffab750c1ba463aaf1d419272f2233e67195d56`  
		Last Modified: Sat, 21 Oct 2023 00:07:30 GMT  
		Size: 1.2 MB (1248665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00237a85b25c3b9ee3968fe9e98da8f378a4a70ccc746a6524820916085348ef`  
		Last Modified: Sat, 21 Oct 2023 00:07:29 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9275f10d0ef0db0999dc5ed6b19c068a941f59a05d69fad4b3cb07c3f0b14a7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74714658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b10f4fd814dc9e97d1147715baacffedd007b23ec081f4c100520df02050e6c9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:07:30 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 15:58:50 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:58:50 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 15:59:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 15:59:08 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 15:59:08 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 15:59:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:59:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 15:59:09 GMT
WORKDIR /go
# Wed, 01 Nov 2023 21:17:21 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 21:17:22 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 21:17:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 21:17:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 21:17:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8457acc181d300b4231b44e12aa0bf4a99ced5d51c5dfdc14eb899a341d5b855`  
		Last Modified: Sat, 21 Oct 2023 01:07:42 GMT  
		Size: 284.1 KB (284074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05626b790821d279bd9aea8466a1a79307764cbc389c51ab081a4b98c7657dc2`  
		Last Modified: Wed, 01 Nov 2023 16:06:11 GMT  
		Size: 65.8 MB (65772806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2dba3cbff62191bbc046c664eead34e3af26adfa5ecdbacf0ba6e73b9cbe51`  
		Last Modified: Wed, 01 Nov 2023 16:05:56 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357de4175525102c1d6c8d4fc605461ca1b1791b2a3b6c55c73e3ef6266159ad`  
		Last Modified: Wed, 01 Nov 2023 21:17:50 GMT  
		Size: 4.5 MB (4511226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59aa4bdeb70fa8c96a09911a5e79184a493cb38488e04d22007af9f9164e4f44`  
		Last Modified: Wed, 01 Nov 2023 21:17:50 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7b450bb18e60383a1dd8c51f37de16c5782ba7eba9e2737540247f3a4394c8`  
		Last Modified: Wed, 01 Nov 2023 21:17:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:76d3844fa9c17929397bb168745241a1f8fa36bf63c437d9d255fe217ec6a87c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73995976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6b4383d952151327974f3f21fa7be1e862f9a67c4ee08a264948e4372890be6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 02:41:07 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 15:36:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:36:13 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 15:36:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 15:36:23 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 15:36:23 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 15:36:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:36:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 15:36:24 GMT
WORKDIR /go
# Wed, 01 Nov 2023 19:56:22 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 19:56:22 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 19:56:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 19:56:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 19:56:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74bf0db6f91dfe1899e8204affb86f8c505a5643bdcb83b085888c86e0c7411`  
		Last Modified: Sat, 21 Oct 2023 02:41:18 GMT  
		Size: 286.3 KB (286297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd442d12e388d3f44ee4325caf9e959ca82d4064c8b1b38321da75a84a6ccbd`  
		Last Modified: Wed, 01 Nov 2023 15:41:04 GMT  
		Size: 64.1 MB (64110459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0297817440f5024a6c0e27f7906a375aa91aea5aaf191caa3f1762426e60e9c2`  
		Last Modified: Wed, 01 Nov 2023 15:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9fb63180b1c62b2cfd436428dc31a25bc97989024e217b9d8e508e82b0b287`  
		Last Modified: Wed, 01 Nov 2023 19:56:42 GMT  
		Size: 5.1 MB (5068382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0ee6df11f2e2e143f36f30697c4b309c4560fa062faa2fcb3a1c22db91257e`  
		Last Modified: Wed, 01 Nov 2023 19:56:42 GMT  
		Size: 1.2 MB (1198448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15b8268dd8cba7445da5d02c68c6787ce774d7ecc7dba9fa3f2775a88884d64`  
		Last Modified: Wed, 01 Nov 2023 19:56:41 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:ed1e2679ee802b3a2c8f7b42d4828ecc9ba50b5a029e3d14bbc54fa2a0fc5444
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74214117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2041e14adf1ce1c2b331135049ec2871be632eb2a7130142af035fa662cb1e19`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:13:11 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:13:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:17:44 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:18:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 19:18:14 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:18:14 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:18:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:18:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:18:17 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:09:16 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:09:17 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:09:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:09:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:09:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc67971d1767eae5019ffeaf8f893e6d81dbba50bde347da0c0433c56e3f2a3`  
		Last Modified: Thu, 28 Sep 2023 22:18:17 GMT  
		Size: 286.7 KB (286659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1caf7fa003bdf7c7611eb2e33a11db077a0f632b70d28f5b73096bf051f25aeb`  
		Last Modified: Tue, 10 Oct 2023 19:28:09 GMT  
		Size: 64.1 MB (64125245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9573c5aef56335266ce720d0812f9a0156f628fbd01ba4a6462be56d8742dc8a`  
		Last Modified: Tue, 10 Oct 2023 19:27:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40b483d55ec27555b481cb0fad97faf6e8d1686165905df945c86967ec0ac96`  
		Last Modified: Sat, 21 Oct 2023 00:09:50 GMT  
		Size: 5.3 MB (5268969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966ad11dd0f3a17ae3666a37f54fd9d6265bc0e18133314a565abf1039e90a1f`  
		Last Modified: Sat, 21 Oct 2023 00:09:50 GMT  
		Size: 1.2 MB (1186175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e18b62f88891e2a1b8f7a5e8a66e6ee69c9f42fe03945d66da418c55d339a9`  
		Last Modified: Sat, 21 Oct 2023 00:09:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:02d085e00e424e29b1a4c45b6358c9ac90629ed72540af87be474238770f3217
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76112263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fa19320a45d01205e0025f17edf0aa856b433bd25ee512a7877ec407bdf0a3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:44:44 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 12:29:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 12:29:18 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 12:29:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 12:29:51 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 12:29:52 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 12:29:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 12:29:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 12:29:54 GMT
WORKDIR /go
# Wed, 01 Nov 2023 16:51:53 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 16:51:55 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 16:51:56 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 16:51:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 16:51:57 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 16:51:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 16:52:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 16:52:01 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f15a4d38dd3d4f044868149900a763ac233f1aef33fe18019f45149b6bd02c`  
		Last Modified: Sat, 21 Oct 2023 00:45:00 GMT  
		Size: 285.1 KB (285095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23831500ce8c52e3d80c9eab9eb44d36e8daf00224a75f36d961186e47851ae8`  
		Last Modified: Wed, 01 Nov 2023 12:38:38 GMT  
		Size: 66.2 MB (66234435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92c933a1dfb2cbb65a33ccba713aabb9ff92ce6a0286e12af67e54c51be8a44`  
		Last Modified: Wed, 01 Nov 2023 12:38:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368a8f32c470e61e32632b0c78836e09dc1d70ab0e9a48e1c2bef1d23de82f7d`  
		Last Modified: Wed, 01 Nov 2023 16:52:34 GMT  
		Size: 5.1 MB (5114679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b61d54a31e32a9c971c8d7ea514537dababa89a4e60ce97eca5bdcf4e8d007`  
		Last Modified: Wed, 01 Nov 2023 16:52:33 GMT  
		Size: 1.3 MB (1262390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147c37f0535cd57e5355158d43aa5608a1430f56aa08ef1b4eb9cea12976a728`  
		Last Modified: Wed, 01 Nov 2023 16:52:33 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:c0740b75861440c921e23bec00c2ce3e14bda7ca7967b2aec7855352ea96cd0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `caddy:2.7-builder-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull caddy@sha256:951876270030a4a5404a8bab425d35b64f90babc594bb65c261cc05eab33ed79
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2128478401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:883908294a37d78f29e796d389d42c83a12c68a6c0f1113bba3bdd9290db5b05`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 02:23:09 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Oct 2023 02:23:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Oct 2023 02:23:11 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Oct 2023 02:23:12 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Oct 2023 02:24:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:24:31 GMT
ENV GOPATH=C:\go
# Wed, 11 Oct 2023 02:25:33 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Oct 2023 02:25:34 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 11 Oct 2023 02:28:30 GMT
RUN $url = 'https://dl.google.com/go/go1.21.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '27c8daf157493f288d42a6f38debc6a2cb391f6543139eba9152fceca0be2a10'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:28:31 GMT
WORKDIR C:\go
# Wed, 11 Oct 2023 04:03:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:03:14 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 12 Oct 2023 01:42:14 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:42:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 12 Oct 2023 01:43:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 12 Oct 2023 01:43:13 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fded5ce3c59d7e8d637a5536d6eed085ff6b6a323f42c1df76a7be6e9970ee`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a72a6b595ab9f8f71a34a065e75e609b20ea5e026f901820fce6d3c9134939`  
		Last Modified: Wed, 11 Oct 2023 02:46:39 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2574f8b7fb0ec5a8c39ee40a8008f0d24c398380247bf7140be1abdede5542b`  
		Last Modified: Wed, 11 Oct 2023 02:46:40 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951c53676fe729ebf5d3c07215d91afa952e6190715f79a7952f4c3aa121231e`  
		Last Modified: Wed, 11 Oct 2023 02:46:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a382bb149b70b82f9c2f58ebf6a2672dc4c64460017836d73a5a23b7379ea095`  
		Last Modified: Wed, 11 Oct 2023 02:46:44 GMT  
		Size: 25.6 MB (25557568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608a2584f4b3b8f3038fa41c0719005822ab967d85d1231843bd729a7b3d2d60`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1058e02ad62f976d823e3035f0578b2868eb09f28986153342a52014cc5c3810`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 284.8 KB (284754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fce039c31b2e60b62a0ede9974b6574519f2e47e1d8f4e09c7a1f30763aee95`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65449f183261f9bbdb731d41f5e6fca94f3e547e8d996133e418773400cfcfe`  
		Last Modified: Wed, 11 Oct 2023 02:46:59 GMT  
		Size: 69.3 MB (69345382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394e07c2ad53e950c47ffb647836822197dc5f8ebe082eaa045854e2b25bafc7`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993f5e59c63ef5be894fc498ab0e165faa3129d35a8a8f5173f12c6a4232f588`  
		Last Modified: Wed, 11 Oct 2023 04:06:31 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c675831130735b443a544dff1b9c188928f34947a5342350ef04eadc0d1ab27`  
		Last Modified: Wed, 11 Oct 2023 04:06:28 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69fe7c1d1f5383a4421f2a0e7284e17db440ee5b7be9f487ce9048f76970e7b6`  
		Last Modified: Thu, 12 Oct 2023 01:45:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee998763c3cef90b11adda3322e66e1a89d89409d1ed29dd73a4101fb657e29`  
		Last Modified: Thu, 12 Oct 2023 01:45:21 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196a81b981d5dc89b19acce594b87914fc5bc4777e42b1322ca9b9d4c4b4f179`  
		Last Modified: Thu, 12 Oct 2023 01:45:22 GMT  
		Size: 1.7 MB (1682335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3ad6e4e7b1be08f8a79e4d77328648deded93f9ef0d4a1e8202ce4c3a21c67`  
		Last Modified: Thu, 12 Oct 2023 01:45:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:7a4eaeb7416d6a4b442d55eab7e8c7824e36a07baef33353084b943d46b6b7b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `caddy:2.7-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull caddy@sha256:04b6c1b2519c8d35d65976c53b4523d7074d53c7b98fa5b29b83c837e021b493
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1956648108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6c3e402a7640df51573fae3237803e1e5fabce3d4c88849d9513c716654d474`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 02:19:41 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Oct 2023 02:19:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Oct 2023 02:19:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Oct 2023 02:19:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Oct 2023 02:20:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:20:18 GMT
ENV GOPATH=C:\go
# Wed, 11 Oct 2023 02:20:42 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Oct 2023 02:20:42 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 11 Oct 2023 02:22:59 GMT
RUN $url = 'https://dl.google.com/go/go1.21.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '27c8daf157493f288d42a6f38debc6a2cb391f6543139eba9152fceca0be2a10'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:23:01 GMT
WORKDIR C:\go
# Wed, 11 Oct 2023 04:04:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:04:42 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 12 Oct 2023 01:43:30 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:43:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 12 Oct 2023 01:43:51 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 12 Oct 2023 01:43:52 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60407a49ce6121c65fa6399c333c5227a09518414fd987c460ea29cb441ac5a`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe632e8cddda4e5f347720b87b8b3868e2e2969048761e3b0a40799d33f5f7a`  
		Last Modified: Wed, 11 Oct 2023 02:45:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4384696fc834e9658e7b3e5d1ceb1f8b362db85865daf29521b3c75c6999c046`  
		Last Modified: Wed, 11 Oct 2023 02:45:04 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c794ea611ef69f54d577f90b68e165e40a17e43b6d1d08f59951a38e084ea5fb`  
		Last Modified: Wed, 11 Oct 2023 02:45:03 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c74dc2d701da2bfabc4d44e6a4e6b92912515e2ca1fb053ffcc6b0d5cae2972`  
		Last Modified: Wed, 11 Oct 2023 02:45:08 GMT  
		Size: 25.5 MB (25531724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91612399ba7df8de0a05ad078c3817548f0a3b44516b76565e14a96ea62452e9`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7439c7c4353d2432c780827e4926910b19e84fe436d58e0a8129de2f631bd2b8`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 264.4 KB (264384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b0eaedd98e739ace4b7934261c71292195e461adcc977d02e57604d4a42ee8`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f46e84d4d007a200b1d6e7cb5b48db90116cdeb8bd3ec3964a08191875973e2`  
		Last Modified: Wed, 11 Oct 2023 02:45:25 GMT  
		Size: 69.3 MB (69325670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f59bab6d84ca44bbb60474dcf59c9af4f0f15edbdd64249b0eeaf968aff211f`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.6 KB (1556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f449f4d34d707dbde9cbb245c154c0b2e1d1a2c55d172501f8d7da576866f76f`  
		Last Modified: Wed, 11 Oct 2023 04:06:49 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a2edf76facdd17af03954b607484f7f7b36164a30634d19dd96b7320feb6b5`  
		Last Modified: Wed, 11 Oct 2023 04:06:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802c3686d509915fea71538d2c40c7a48c71719fab6144cb4497b6118b276ab9`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99cb183ed6cdad781eaba7bd1b4cb443befd9042c8a59450ee41f0245dd0ece4`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec33434b55fade6bcd7f3f0dfc10c981de93dc44bbae2b8702fdb6418a37a65b`  
		Last Modified: Thu, 12 Oct 2023 01:45:38 GMT  
		Size: 1.7 MB (1664788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0833369ef8236fcf99aba2d1fa48788db07662d0a9885a8429d435bf9f2227b2`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-windowsservercore`

```console
$ docker pull caddy@sha256:b859825f1b8093a4b961d02fb945e63f5180c5e07e56ce7495384835c016c47d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4974; amd64
	-	windows version 10.0.20348.2031; amd64

### `caddy:2.7-windowsservercore` - windows version 10.0.17763.4974; amd64

```console
$ docker pull caddy@sha256:77cb1b0b8315f376e69becef400d33c9d8b2a45548714845a821736158771de2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2047649951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3171dc2f25b4435520d8ba983ebf42f070ddec217b0da7677e309cc4cd51b05`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 03:59:19 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:39:06 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:40:04 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:40:05 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:40:06 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:40:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:40:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:40:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:40:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:40:12 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:40:13 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:41:01 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:41:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c4565a9b36858bc727874537e3c99968438a37e53c13057b0b1a233699d014`  
		Last Modified: Wed, 11 Oct 2023 04:05:44 GMT  
		Size: 472.0 KB (472034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df4a75108d3a33583e7ae61f1a019d4865860820bd89280ba414af94dd3f56e`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9dee9792a7bf7e1225840c56fb692536bee1743eba0a4da2faff34533f1160f`  
		Last Modified: Thu, 12 Oct 2023 01:44:37 GMT  
		Size: 15.3 MB (15296055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41900185a2519f01b8bd860f70936cee271612c4023512694b105826e0e0251`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0f1b69a12cd8550d868156e54168abaa32e1df40ee6eb39bc4e173ce04905e`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca266891343bff15b313846692ba3a41f313d5b228bedde964191332a16dffe`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12539eb7433a69ed67556d91b75b66dfedf0543d3efd7dabe82772437307a6f`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5103f279ed518bcfec88e00183e3222b50c1bc2f0e5b42f043e2198da424de98`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efc1cff2dac4308ce732a395ee215e1497d21f737e42e77917debf070afa8d7`  
		Last Modified: Thu, 12 Oct 2023 01:44:35 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cb50f59d2b11532a330925afb6ebd04d9b4708de8b11ae436e258c3764d741`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd11a311e4c0cf49bb544980f2c999751fc5e2fbe80d37b0f719f837abf8c3f`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ccbee9a6b9058ec933797dc1cfed875ceeb0115ce29ee163cd60a66e9f3b2d`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b486fc8ef055010a59374557443d3b713b9e55c1ccd11b7873f47876758976`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41df430d9a95c6000c922dd021b6cb2af0110dcc661ddc37a190a8cf6cd4bb06`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f243061a2e17d508efa4a424310d9ca158ca0cf0f59bd15cac606ab3e74701`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e709fff7d020a5d7c2d9e9e9a664c87392e9f9a4f4ced9802e64ca268995e23`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2c7aca9b511bc62340e6e8883d5f625bdccb805c4e897b837b68f3c79964b5`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38802c5a2b45b7029b250d88dac8209405146b0968925d1204cf17f7c3e76d98`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 269.1 KB (269086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376d19318a370d0da2ffcc29b47c2810278efa9d22fb39799c48687dfee0a2d9`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-windowsservercore` - windows version 10.0.20348.2031; amd64

```console
$ docker pull caddy@sha256:05f529a68927f0acfa7afbc79b7a19541f94430c137612ed344de7a822dcfafb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1875907229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8701a0e5aada270070acddeed89c57e20a5cac8afd88ed58da9557bf01dccb27`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:02:07 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:41:20 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:41:42 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:41:42 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:41:43 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:41:44 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:41:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:41:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:41:50 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:41:52 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:42:04 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:42:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c36616366b0df84f087a09bf19876f3872d839997f2f43e4eb8599861417c06`  
		Last Modified: Wed, 11 Oct 2023 04:06:10 GMT  
		Size: 467.9 KB (467933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db420ca589f10e4f9f5bc9dd6badc855d95c6a598888f2eb77a747eced259557`  
		Last Modified: Thu, 12 Oct 2023 01:45:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b5d7433dab05533d906a290a0f42cf31804c132da65c9fd7d4d2c41a64f519`  
		Last Modified: Thu, 12 Oct 2023 01:45:04 GMT  
		Size: 15.3 MB (15284209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62069fdf38bff9495ef2be05d397a55221536f9eec345734d6acec3a6196324f`  
		Last Modified: Thu, 12 Oct 2023 01:45:00 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e237a4c373c6937b5c51d0a3936152ac2b572fd5a432db3690f4070a7c78327`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73fae1c57e166a2ade87aa32e11980b456658212b296eea0f02ba3ec1c6557b`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000f2101dc464fa43321619c6e65c5b9e62b62755f3b141e69bd31892a253ded`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8536723423849b861a08fa490135f690c287be0144267e38fb3e631fb1bddbd2`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f176ef86531863755c3a315ec662b8da324474ae6097d7365dc18b76d61bde5`  
		Last Modified: Thu, 12 Oct 2023 01:44:58 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3973c168b3a63daa069e3a9870395561709d7b27762ffafb16538c773a16ad29`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5a10fbc59abc7ee7cc04a7ff48cc85983728745e91e8ef5fafee0589ba2193`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf033f8ab12414230e08aaada214c761777b0c784908ad2783ee31f8d330d0c9`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e2af83b2af59d76bd9b735c4e71b9492d9dbc120c042b8134ae0a70008f49`  
		Last Modified: Thu, 12 Oct 2023 01:44:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0355ed819405072f13996095ae7ec7044017bee81808dea9500459620118c20b`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e86117e27425829055f627e6156a4a657d9817cf8d2158f0026752366c9022c`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22fbe71be2fe08164a92f1362959f0a4aba194dcf931945d7bb2ac50e8f6467`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed768b9f807d51e5834f0bc8b2ea4dda09a5139d126f9141cb3db51f781ea541`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359fc3c79eda3ddbb39c46b09a4c68137a693a72f8712182d545c546b726027e`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 289.5 KB (289533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e4b8683a429393010114c6906acced22d65d5167cda2cc55238ae5b9f816c0`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-windowsservercore-1809`

```console
$ docker pull caddy@sha256:8169d134dfa19ddbba9eeeb7210c5227c2a61f00906c340474aab1250aba47f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `caddy:2.7-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull caddy@sha256:77cb1b0b8315f376e69becef400d33c9d8b2a45548714845a821736158771de2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2047649951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3171dc2f25b4435520d8ba983ebf42f070ddec217b0da7677e309cc4cd51b05`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 03:59:19 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:39:06 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:40:04 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:40:05 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:40:06 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:40:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:40:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:40:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:40:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:40:12 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:40:13 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:41:01 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:41:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c4565a9b36858bc727874537e3c99968438a37e53c13057b0b1a233699d014`  
		Last Modified: Wed, 11 Oct 2023 04:05:44 GMT  
		Size: 472.0 KB (472034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df4a75108d3a33583e7ae61f1a019d4865860820bd89280ba414af94dd3f56e`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9dee9792a7bf7e1225840c56fb692536bee1743eba0a4da2faff34533f1160f`  
		Last Modified: Thu, 12 Oct 2023 01:44:37 GMT  
		Size: 15.3 MB (15296055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41900185a2519f01b8bd860f70936cee271612c4023512694b105826e0e0251`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0f1b69a12cd8550d868156e54168abaa32e1df40ee6eb39bc4e173ce04905e`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca266891343bff15b313846692ba3a41f313d5b228bedde964191332a16dffe`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12539eb7433a69ed67556d91b75b66dfedf0543d3efd7dabe82772437307a6f`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5103f279ed518bcfec88e00183e3222b50c1bc2f0e5b42f043e2198da424de98`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efc1cff2dac4308ce732a395ee215e1497d21f737e42e77917debf070afa8d7`  
		Last Modified: Thu, 12 Oct 2023 01:44:35 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cb50f59d2b11532a330925afb6ebd04d9b4708de8b11ae436e258c3764d741`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd11a311e4c0cf49bb544980f2c999751fc5e2fbe80d37b0f719f837abf8c3f`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ccbee9a6b9058ec933797dc1cfed875ceeb0115ce29ee163cd60a66e9f3b2d`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b486fc8ef055010a59374557443d3b713b9e55c1ccd11b7873f47876758976`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41df430d9a95c6000c922dd021b6cb2af0110dcc661ddc37a190a8cf6cd4bb06`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f243061a2e17d508efa4a424310d9ca158ca0cf0f59bd15cac606ab3e74701`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e709fff7d020a5d7c2d9e9e9a664c87392e9f9a4f4ced9802e64ca268995e23`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2c7aca9b511bc62340e6e8883d5f625bdccb805c4e897b837b68f3c79964b5`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38802c5a2b45b7029b250d88dac8209405146b0968925d1204cf17f7c3e76d98`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 269.1 KB (269086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376d19318a370d0da2ffcc29b47c2810278efa9d22fb39799c48687dfee0a2d9`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:278d32be7fb2f9a5e3f48ea6a672747dbb4ad6256e4802aff4a1e11a67e2e518
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `caddy:2.7-windowsservercore-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull caddy@sha256:05f529a68927f0acfa7afbc79b7a19541f94430c137612ed344de7a822dcfafb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1875907229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8701a0e5aada270070acddeed89c57e20a5cac8afd88ed58da9557bf01dccb27`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:02:07 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:41:20 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:41:42 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:41:42 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:41:43 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:41:44 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:41:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:41:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:41:50 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:41:52 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:42:04 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:42:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c36616366b0df84f087a09bf19876f3872d839997f2f43e4eb8599861417c06`  
		Last Modified: Wed, 11 Oct 2023 04:06:10 GMT  
		Size: 467.9 KB (467933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db420ca589f10e4f9f5bc9dd6badc855d95c6a598888f2eb77a747eced259557`  
		Last Modified: Thu, 12 Oct 2023 01:45:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b5d7433dab05533d906a290a0f42cf31804c132da65c9fd7d4d2c41a64f519`  
		Last Modified: Thu, 12 Oct 2023 01:45:04 GMT  
		Size: 15.3 MB (15284209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62069fdf38bff9495ef2be05d397a55221536f9eec345734d6acec3a6196324f`  
		Last Modified: Thu, 12 Oct 2023 01:45:00 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e237a4c373c6937b5c51d0a3936152ac2b572fd5a432db3690f4070a7c78327`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73fae1c57e166a2ade87aa32e11980b456658212b296eea0f02ba3ec1c6557b`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000f2101dc464fa43321619c6e65c5b9e62b62755f3b141e69bd31892a253ded`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8536723423849b861a08fa490135f690c287be0144267e38fb3e631fb1bddbd2`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f176ef86531863755c3a315ec662b8da324474ae6097d7365dc18b76d61bde5`  
		Last Modified: Thu, 12 Oct 2023 01:44:58 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3973c168b3a63daa069e3a9870395561709d7b27762ffafb16538c773a16ad29`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5a10fbc59abc7ee7cc04a7ff48cc85983728745e91e8ef5fafee0589ba2193`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf033f8ab12414230e08aaada214c761777b0c784908ad2783ee31f8d330d0c9`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e2af83b2af59d76bd9b735c4e71b9492d9dbc120c042b8134ae0a70008f49`  
		Last Modified: Thu, 12 Oct 2023 01:44:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0355ed819405072f13996095ae7ec7044017bee81808dea9500459620118c20b`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e86117e27425829055f627e6156a4a657d9817cf8d2158f0026752366c9022c`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22fbe71be2fe08164a92f1362959f0a4aba194dcf931945d7bb2ac50e8f6467`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed768b9f807d51e5834f0bc8b2ea4dda09a5139d126f9141cb3db51f781ea541`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359fc3c79eda3ddbb39c46b09a4c68137a693a72f8712182d545c546b726027e`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 289.5 KB (289533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e4b8683a429393010114c6906acced22d65d5167cda2cc55238ae5b9f816c0`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.5`

```console
$ docker pull caddy@sha256:325f81ca0328db0737503a53f43717fce79ea0c574e83f8e586c8d350cadf34b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4974; amd64
	-	windows version 10.0.20348.2031; amd64

### `caddy:2.7.5` - linux; amd64

```console
$ docker pull caddy@sha256:a9c7585fdc50bb28d686b73a9b1f0eb9a3d103efd63c48dc334ccb5f51aa1722
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18474311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70c3913f54e294079c54cc8b651576b08dd4add42a0f4c0bc93d539913ae335d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:11:11 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:11:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:11:12 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:11:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:11:15 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:11:15 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:11:16 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:11:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5433daac73cddf3f03243a31c38d460570073f83e9a8cf64c7f0e3387b85807`  
		Last Modified: Sat, 21 Oct 2023 00:11:36 GMT  
		Size: 350.8 KB (350840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c6b4aafe2c09344f58425bb0fe037a429808edb7b2ba37d79cd35b2775a422`  
		Last Modified: Sat, 21 Oct 2023 00:11:36 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a182bff4e1b33f3d5dd80f809e697793466287c3da7704863c3d0b51d42b5b`  
		Last Modified: Sat, 21 Oct 2023 00:11:39 GMT  
		Size: 14.7 MB (14713998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f43da8d65d754093117d4c673a7b725316be4e576e32b0d40c995e6ab1a07b7c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17422245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18b3bb2c3e0a97c9fe052eca67890f691907de7a5b514e88a44e660bb905079b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:06:46 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:06:48 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:06:48 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:06:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:06:51 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:06:51 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:06:52 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:06:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e09dc0459583a6ad3ba0428d5e180b7e3e6ae28360a69e293f03632cec397a0`  
		Last Modified: Sat, 21 Oct 2023 00:07:14 GMT  
		Size: 347.6 KB (347617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4705ff25da68d95a4bd671cbd4cec69369ea788be53bfafb45cdf4a930a725f8`  
		Last Modified: Sat, 21 Oct 2023 00:07:13 GMT  
		Size: 7.5 KB (7504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969c487cd333c7b53a7f57017e0ad77490d3806d9e52259caf9772016e96576d`  
		Last Modified: Sat, 21 Oct 2023 00:07:16 GMT  
		Size: 13.9 MB (13921833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5` - linux; arm variant v7

```console
$ docker pull caddy@sha256:dd028bb08526d3533680243c94b9464c9c1a6559dccf5dde3b61ec73b9afd002
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17155303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:539aa551acc109f33c6ea5076a1f518af4d0476b517dc698d98c7350e8cb1b1a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:17:55 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:17:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:17:56 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:17:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:17:59 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:17:59 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:18:00 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:18:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee93e167fdbd8e67ec3f4ed8eaf242e5c8022a9845dd4f797448503af15d777c`  
		Last Modified: Sat, 21 Oct 2023 00:18:22 GMT  
		Size: 344.5 KB (344454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2895c0143aa41e87473191f749160d3109330cdb9de0c90a9b0a9e60e8a3a3e`  
		Last Modified: Sat, 21 Oct 2023 00:18:22 GMT  
		Size: 7.5 KB (7508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f015da3d3488ea9171b2970be40718bfa7e31496bae565a9bc2b677e53c09915`  
		Last Modified: Sat, 21 Oct 2023 00:18:25 GMT  
		Size: 13.9 MB (13903436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:d18ec23ab87841ede7ccefc353c20d1554faddf3ac362213c32ae22311136da5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17273763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cbdde935029392921ca3521ef9ebdb6a2b46cd1d4b7a9dabf0b71b00c593572`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:23:28 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:23:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:23:29 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:23:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:23:31 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:23:31 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:23:32 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:23:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461fe4f467fe88a160e176c442825b4bfea8dde13fc2324393a5d81518375e6f`  
		Last Modified: Sat, 21 Oct 2023 00:23:52 GMT  
		Size: 360.6 KB (360623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9335adc9ff07e38d963f0a71a2f7db01b5b5ed8e9d93fba14e584f25ea05c29d`  
		Last Modified: Sat, 21 Oct 2023 00:23:52 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32426666f5ec8621a07038733361be24f83719a812c0cce54e3f41192b31c2d`  
		Last Modified: Sat, 21 Oct 2023 00:23:54 GMT  
		Size: 13.6 MB (13573803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5` - linux; ppc64le

```console
$ docker pull caddy@sha256:1cd57ee42a4e84e91731e9182350ab4fd5b26705ec7286c28c5768c549435fd5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.1 MB (17057167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5aa3d5c5c63bea353c483de170ae8690a4f7eb12042cb84dc2bf0d52bf914b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:09:00 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:09:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:09:02 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:09:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:09:05 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:09:05 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:09:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:09:09 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:09:09 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:09:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692440f8f5ba2c6efbf2e74e3301377e3d9a90ae5a7cbd728c771ab306277830`  
		Last Modified: Sat, 21 Oct 2023 00:09:34 GMT  
		Size: 362.2 KB (362183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2886f5cbb210969eea27d97b8a48d88cae7bbe1bdd528a2b2775a8affde3084`  
		Last Modified: Sat, 21 Oct 2023 00:09:33 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdd6a19a7b9d3f4621c5388c53b0a9ea5591e9e72250bc60bcf22ed672632b1`  
		Last Modified: Sat, 21 Oct 2023 00:09:36 GMT  
		Size: 13.3 MB (13340969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5` - linux; s390x

```console
$ docker pull caddy@sha256:7dc6afd9bb40ff4450e4282bc56431b993d068c5b832c914dd50831189920061
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.8 MB (17822696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be3873facfc56aac0a1a9659efab4cddfc06afe6ac27c54cdd1b6fc9a23f1c1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:05:23 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:05:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:05:24 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:05:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:05:27 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:05:27 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:05:29 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:05:29 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:05:29 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d6d08cebdb83ff91ba335e0c4aec115b17261ed40307aaee6adde8c6763ad6`  
		Last Modified: Sat, 21 Oct 2023 00:06:00 GMT  
		Size: 355.0 KB (354963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58e0c7856c877cacd1d63a86beb12c9be91c4a0950dd85954db6f16a6d93103`  
		Last Modified: Sat, 21 Oct 2023 00:06:00 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69bf19674eec620ff3f87ecb754c60b7c137eb6c8c3763ff795739061593a77`  
		Last Modified: Sat, 21 Oct 2023 00:06:02 GMT  
		Size: 14.2 MB (14245123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5` - windows version 10.0.17763.4974; amd64

```console
$ docker pull caddy@sha256:77cb1b0b8315f376e69becef400d33c9d8b2a45548714845a821736158771de2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2047649951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3171dc2f25b4435520d8ba983ebf42f070ddec217b0da7677e309cc4cd51b05`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 03:59:19 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:39:06 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:40:04 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:40:05 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:40:06 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:40:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:40:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:40:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:40:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:40:12 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:40:13 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:41:01 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:41:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c4565a9b36858bc727874537e3c99968438a37e53c13057b0b1a233699d014`  
		Last Modified: Wed, 11 Oct 2023 04:05:44 GMT  
		Size: 472.0 KB (472034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df4a75108d3a33583e7ae61f1a019d4865860820bd89280ba414af94dd3f56e`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9dee9792a7bf7e1225840c56fb692536bee1743eba0a4da2faff34533f1160f`  
		Last Modified: Thu, 12 Oct 2023 01:44:37 GMT  
		Size: 15.3 MB (15296055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41900185a2519f01b8bd860f70936cee271612c4023512694b105826e0e0251`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0f1b69a12cd8550d868156e54168abaa32e1df40ee6eb39bc4e173ce04905e`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca266891343bff15b313846692ba3a41f313d5b228bedde964191332a16dffe`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12539eb7433a69ed67556d91b75b66dfedf0543d3efd7dabe82772437307a6f`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5103f279ed518bcfec88e00183e3222b50c1bc2f0e5b42f043e2198da424de98`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efc1cff2dac4308ce732a395ee215e1497d21f737e42e77917debf070afa8d7`  
		Last Modified: Thu, 12 Oct 2023 01:44:35 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cb50f59d2b11532a330925afb6ebd04d9b4708de8b11ae436e258c3764d741`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd11a311e4c0cf49bb544980f2c999751fc5e2fbe80d37b0f719f837abf8c3f`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ccbee9a6b9058ec933797dc1cfed875ceeb0115ce29ee163cd60a66e9f3b2d`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b486fc8ef055010a59374557443d3b713b9e55c1ccd11b7873f47876758976`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41df430d9a95c6000c922dd021b6cb2af0110dcc661ddc37a190a8cf6cd4bb06`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f243061a2e17d508efa4a424310d9ca158ca0cf0f59bd15cac606ab3e74701`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e709fff7d020a5d7c2d9e9e9a664c87392e9f9a4f4ced9802e64ca268995e23`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2c7aca9b511bc62340e6e8883d5f625bdccb805c4e897b837b68f3c79964b5`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38802c5a2b45b7029b250d88dac8209405146b0968925d1204cf17f7c3e76d98`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 269.1 KB (269086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376d19318a370d0da2ffcc29b47c2810278efa9d22fb39799c48687dfee0a2d9`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5` - windows version 10.0.20348.2031; amd64

```console
$ docker pull caddy@sha256:05f529a68927f0acfa7afbc79b7a19541f94430c137612ed344de7a822dcfafb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1875907229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8701a0e5aada270070acddeed89c57e20a5cac8afd88ed58da9557bf01dccb27`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:02:07 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:41:20 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:41:42 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:41:42 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:41:43 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:41:44 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:41:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:41:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:41:50 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:41:52 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:42:04 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:42:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c36616366b0df84f087a09bf19876f3872d839997f2f43e4eb8599861417c06`  
		Last Modified: Wed, 11 Oct 2023 04:06:10 GMT  
		Size: 467.9 KB (467933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db420ca589f10e4f9f5bc9dd6badc855d95c6a598888f2eb77a747eced259557`  
		Last Modified: Thu, 12 Oct 2023 01:45:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b5d7433dab05533d906a290a0f42cf31804c132da65c9fd7d4d2c41a64f519`  
		Last Modified: Thu, 12 Oct 2023 01:45:04 GMT  
		Size: 15.3 MB (15284209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62069fdf38bff9495ef2be05d397a55221536f9eec345734d6acec3a6196324f`  
		Last Modified: Thu, 12 Oct 2023 01:45:00 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e237a4c373c6937b5c51d0a3936152ac2b572fd5a432db3690f4070a7c78327`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73fae1c57e166a2ade87aa32e11980b456658212b296eea0f02ba3ec1c6557b`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000f2101dc464fa43321619c6e65c5b9e62b62755f3b141e69bd31892a253ded`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8536723423849b861a08fa490135f690c287be0144267e38fb3e631fb1bddbd2`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f176ef86531863755c3a315ec662b8da324474ae6097d7365dc18b76d61bde5`  
		Last Modified: Thu, 12 Oct 2023 01:44:58 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3973c168b3a63daa069e3a9870395561709d7b27762ffafb16538c773a16ad29`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5a10fbc59abc7ee7cc04a7ff48cc85983728745e91e8ef5fafee0589ba2193`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf033f8ab12414230e08aaada214c761777b0c784908ad2783ee31f8d330d0c9`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e2af83b2af59d76bd9b735c4e71b9492d9dbc120c042b8134ae0a70008f49`  
		Last Modified: Thu, 12 Oct 2023 01:44:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0355ed819405072f13996095ae7ec7044017bee81808dea9500459620118c20b`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e86117e27425829055f627e6156a4a657d9817cf8d2158f0026752366c9022c`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22fbe71be2fe08164a92f1362959f0a4aba194dcf931945d7bb2ac50e8f6467`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed768b9f807d51e5834f0bc8b2ea4dda09a5139d126f9141cb3db51f781ea541`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359fc3c79eda3ddbb39c46b09a4c68137a693a72f8712182d545c546b726027e`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 289.5 KB (289533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e4b8683a429393010114c6906acced22d65d5167cda2cc55238ae5b9f816c0`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.5-alpine`

```console
$ docker pull caddy@sha256:f1c092da9fcba7a8197cf1065a347d4f0bb67b6dd188985eafaf0a5aec6c9041
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.7.5-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:a9c7585fdc50bb28d686b73a9b1f0eb9a3d103efd63c48dc334ccb5f51aa1722
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18474311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70c3913f54e294079c54cc8b651576b08dd4add42a0f4c0bc93d539913ae335d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:11:11 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:11:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:11:12 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:11:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:11:15 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:11:15 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:11:16 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:11:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5433daac73cddf3f03243a31c38d460570073f83e9a8cf64c7f0e3387b85807`  
		Last Modified: Sat, 21 Oct 2023 00:11:36 GMT  
		Size: 350.8 KB (350840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c6b4aafe2c09344f58425bb0fe037a429808edb7b2ba37d79cd35b2775a422`  
		Last Modified: Sat, 21 Oct 2023 00:11:36 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a182bff4e1b33f3d5dd80f809e697793466287c3da7704863c3d0b51d42b5b`  
		Last Modified: Sat, 21 Oct 2023 00:11:39 GMT  
		Size: 14.7 MB (14713998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f43da8d65d754093117d4c673a7b725316be4e576e32b0d40c995e6ab1a07b7c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17422245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18b3bb2c3e0a97c9fe052eca67890f691907de7a5b514e88a44e660bb905079b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:06:46 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:06:48 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:06:48 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:06:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:06:51 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:06:51 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:06:52 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:06:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e09dc0459583a6ad3ba0428d5e180b7e3e6ae28360a69e293f03632cec397a0`  
		Last Modified: Sat, 21 Oct 2023 00:07:14 GMT  
		Size: 347.6 KB (347617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4705ff25da68d95a4bd671cbd4cec69369ea788be53bfafb45cdf4a930a725f8`  
		Last Modified: Sat, 21 Oct 2023 00:07:13 GMT  
		Size: 7.5 KB (7504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969c487cd333c7b53a7f57017e0ad77490d3806d9e52259caf9772016e96576d`  
		Last Modified: Sat, 21 Oct 2023 00:07:16 GMT  
		Size: 13.9 MB (13921833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:dd028bb08526d3533680243c94b9464c9c1a6559dccf5dde3b61ec73b9afd002
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17155303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:539aa551acc109f33c6ea5076a1f518af4d0476b517dc698d98c7350e8cb1b1a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:17:55 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:17:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:17:56 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:17:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:17:59 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:17:59 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:18:00 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:18:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee93e167fdbd8e67ec3f4ed8eaf242e5c8022a9845dd4f797448503af15d777c`  
		Last Modified: Sat, 21 Oct 2023 00:18:22 GMT  
		Size: 344.5 KB (344454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2895c0143aa41e87473191f749160d3109330cdb9de0c90a9b0a9e60e8a3a3e`  
		Last Modified: Sat, 21 Oct 2023 00:18:22 GMT  
		Size: 7.5 KB (7508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f015da3d3488ea9171b2970be40718bfa7e31496bae565a9bc2b677e53c09915`  
		Last Modified: Sat, 21 Oct 2023 00:18:25 GMT  
		Size: 13.9 MB (13903436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:d18ec23ab87841ede7ccefc353c20d1554faddf3ac362213c32ae22311136da5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17273763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cbdde935029392921ca3521ef9ebdb6a2b46cd1d4b7a9dabf0b71b00c593572`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:23:28 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:23:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:23:29 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:23:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:23:31 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:23:31 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:23:32 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:23:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461fe4f467fe88a160e176c442825b4bfea8dde13fc2324393a5d81518375e6f`  
		Last Modified: Sat, 21 Oct 2023 00:23:52 GMT  
		Size: 360.6 KB (360623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9335adc9ff07e38d963f0a71a2f7db01b5b5ed8e9d93fba14e584f25ea05c29d`  
		Last Modified: Sat, 21 Oct 2023 00:23:52 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32426666f5ec8621a07038733361be24f83719a812c0cce54e3f41192b31c2d`  
		Last Modified: Sat, 21 Oct 2023 00:23:54 GMT  
		Size: 13.6 MB (13573803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:1cd57ee42a4e84e91731e9182350ab4fd5b26705ec7286c28c5768c549435fd5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.1 MB (17057167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5aa3d5c5c63bea353c483de170ae8690a4f7eb12042cb84dc2bf0d52bf914b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:09:00 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:09:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:09:02 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:09:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:09:05 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:09:05 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:09:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:09:09 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:09:09 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:09:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692440f8f5ba2c6efbf2e74e3301377e3d9a90ae5a7cbd728c771ab306277830`  
		Last Modified: Sat, 21 Oct 2023 00:09:34 GMT  
		Size: 362.2 KB (362183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2886f5cbb210969eea27d97b8a48d88cae7bbe1bdd528a2b2775a8affde3084`  
		Last Modified: Sat, 21 Oct 2023 00:09:33 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdd6a19a7b9d3f4621c5388c53b0a9ea5591e9e72250bc60bcf22ed672632b1`  
		Last Modified: Sat, 21 Oct 2023 00:09:36 GMT  
		Size: 13.3 MB (13340969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:7dc6afd9bb40ff4450e4282bc56431b993d068c5b832c914dd50831189920061
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.8 MB (17822696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be3873facfc56aac0a1a9659efab4cddfc06afe6ac27c54cdd1b6fc9a23f1c1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:05:23 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:05:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:05:24 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:05:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:05:27 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:05:27 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:05:29 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:05:29 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:05:29 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d6d08cebdb83ff91ba335e0c4aec115b17261ed40307aaee6adde8c6763ad6`  
		Last Modified: Sat, 21 Oct 2023 00:06:00 GMT  
		Size: 355.0 KB (354963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58e0c7856c877cacd1d63a86beb12c9be91c4a0950dd85954db6f16a6d93103`  
		Last Modified: Sat, 21 Oct 2023 00:06:00 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69bf19674eec620ff3f87ecb754c60b7c137eb6c8c3763ff795739061593a77`  
		Last Modified: Sat, 21 Oct 2023 00:06:02 GMT  
		Size: 14.2 MB (14245123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.5-builder`

```console
$ docker pull caddy@sha256:d039cffaec2ce64db9cae84dc789bb36c8d3d09e6ff70f3a40c4f405a89deed8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4974; amd64
	-	windows version 10.0.20348.2031; amd64

### `caddy:2.7.5-builder` - linux; amd64

```console
$ docker pull caddy@sha256:d1f6d3dcfec129b4d0e23b6743f576807352958232a7ac6c17ee36f785fe5c58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76972374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e113a57232410dd987d12708b35062e6a269825fa7b4d03aef42c00acc93dce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:54:30 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:54:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:20:11 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:20:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 19:20:22 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:20:22 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:20:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:20:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:20:23 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:11:20 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:11:20 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:11:20 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:11:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:11:21 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:11:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:11:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:11:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc37b24bb09971feb8bf4882e861bce9db0c985a16a900adb0dc9de3f854243b`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 284.7 KB (284690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a4303e95078c253686dcc16d7717644af63809efcbd753c0a999c9aad3fe72`  
		Last Modified: Tue, 10 Oct 2023 19:26:17 GMT  
		Size: 67.0 MB (67012876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359925be0f358b952dc8be63647139c5aab0fff94f7a070d88cb51dd258f80e5`  
		Last Modified: Tue, 10 Oct 2023 19:26:06 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958092cb44d28ddde181d193284001b1146b33a1cf19624e9683fc8f31551043`  
		Last Modified: Sat, 21 Oct 2023 00:11:52 GMT  
		Size: 5.0 MB (4970044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85cdb072dd78dcf6a7b04409cf7c8dc1fddddf912b601b15c6dc94adb2df10b`  
		Last Modified: Sat, 21 Oct 2023 00:11:51 GMT  
		Size: 1.3 MB (1302237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32749367842b0c8b40e7f61a315ff21b4d42211b5399e648beb75d86acb29c4c`  
		Last Modified: Sat, 21 Oct 2023 00:11:51 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:15f0db6d62062758441d2d22fd178c42299cf148c5097ffe10468153ff40c6b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75413855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:509cf858d9f3ffa4a94fe988705864c41bd510f34ade4ece0d2ede4cda23599f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:55:22 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:55:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 18:49:21 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 18:49:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 18:49:42 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 18:49:42 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 18:49:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 18:49:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 18:49:43 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:06:57 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:06:57 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:06:58 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:06:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:06:58 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:06:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:06:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:06:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3da3b9e7a12f6bb6b7f56e9240c2c92ce8c9f5fd5ef3b3063b9a93d454919e`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 284.9 KB (284887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbbb7b34bc324d050e49d3dd31294bdde5d6ecda33decf9afe31c11165b138a`  
		Last Modified: Tue, 10 Oct 2023 18:55:32 GMT  
		Size: 65.8 MB (65770135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c022f45a9fb1e7649eb4a663acd4ed6437363b4fc6e56f6af3e5f457a5d06ee8`  
		Last Modified: Tue, 10 Oct 2023 18:55:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12bec1760d3cf2773adbb14bd47431e46e130a914a46535c9a70de28e4b363b`  
		Last Modified: Sat, 21 Oct 2023 00:07:30 GMT  
		Size: 5.0 MB (4964316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888b304960048015ef929fcb0ffab750c1ba463aaf1d419272f2233e67195d56`  
		Last Modified: Sat, 21 Oct 2023 00:07:30 GMT  
		Size: 1.2 MB (1248665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00237a85b25c3b9ee3968fe9e98da8f378a4a70ccc746a6524820916085348ef`  
		Last Modified: Sat, 21 Oct 2023 00:07:29 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9275f10d0ef0db0999dc5ed6b19c068a941f59a05d69fad4b3cb07c3f0b14a7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74714658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b10f4fd814dc9e97d1147715baacffedd007b23ec081f4c100520df02050e6c9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:07:30 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 15:58:50 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:58:50 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 15:59:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 15:59:08 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 15:59:08 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 15:59:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:59:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 15:59:09 GMT
WORKDIR /go
# Wed, 01 Nov 2023 21:17:21 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 21:17:22 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 21:17:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 21:17:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 21:17:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8457acc181d300b4231b44e12aa0bf4a99ced5d51c5dfdc14eb899a341d5b855`  
		Last Modified: Sat, 21 Oct 2023 01:07:42 GMT  
		Size: 284.1 KB (284074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05626b790821d279bd9aea8466a1a79307764cbc389c51ab081a4b98c7657dc2`  
		Last Modified: Wed, 01 Nov 2023 16:06:11 GMT  
		Size: 65.8 MB (65772806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2dba3cbff62191bbc046c664eead34e3af26adfa5ecdbacf0ba6e73b9cbe51`  
		Last Modified: Wed, 01 Nov 2023 16:05:56 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357de4175525102c1d6c8d4fc605461ca1b1791b2a3b6c55c73e3ef6266159ad`  
		Last Modified: Wed, 01 Nov 2023 21:17:50 GMT  
		Size: 4.5 MB (4511226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59aa4bdeb70fa8c96a09911a5e79184a493cb38488e04d22007af9f9164e4f44`  
		Last Modified: Wed, 01 Nov 2023 21:17:50 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7b450bb18e60383a1dd8c51f37de16c5782ba7eba9e2737540247f3a4394c8`  
		Last Modified: Wed, 01 Nov 2023 21:17:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:76d3844fa9c17929397bb168745241a1f8fa36bf63c437d9d255fe217ec6a87c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73995976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6b4383d952151327974f3f21fa7be1e862f9a67c4ee08a264948e4372890be6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 02:41:07 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 15:36:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:36:13 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 15:36:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 15:36:23 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 15:36:23 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 15:36:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:36:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 15:36:24 GMT
WORKDIR /go
# Wed, 01 Nov 2023 19:56:22 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 19:56:22 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 19:56:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 19:56:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 19:56:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74bf0db6f91dfe1899e8204affb86f8c505a5643bdcb83b085888c86e0c7411`  
		Last Modified: Sat, 21 Oct 2023 02:41:18 GMT  
		Size: 286.3 KB (286297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd442d12e388d3f44ee4325caf9e959ca82d4064c8b1b38321da75a84a6ccbd`  
		Last Modified: Wed, 01 Nov 2023 15:41:04 GMT  
		Size: 64.1 MB (64110459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0297817440f5024a6c0e27f7906a375aa91aea5aaf191caa3f1762426e60e9c2`  
		Last Modified: Wed, 01 Nov 2023 15:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9fb63180b1c62b2cfd436428dc31a25bc97989024e217b9d8e508e82b0b287`  
		Last Modified: Wed, 01 Nov 2023 19:56:42 GMT  
		Size: 5.1 MB (5068382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0ee6df11f2e2e143f36f30697c4b309c4560fa062faa2fcb3a1c22db91257e`  
		Last Modified: Wed, 01 Nov 2023 19:56:42 GMT  
		Size: 1.2 MB (1198448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15b8268dd8cba7445da5d02c68c6787ce774d7ecc7dba9fa3f2775a88884d64`  
		Last Modified: Wed, 01 Nov 2023 19:56:41 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:ed1e2679ee802b3a2c8f7b42d4828ecc9ba50b5a029e3d14bbc54fa2a0fc5444
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74214117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2041e14adf1ce1c2b331135049ec2871be632eb2a7130142af035fa662cb1e19`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:13:11 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:13:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:17:44 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:18:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 19:18:14 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:18:14 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:18:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:18:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:18:17 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:09:16 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:09:17 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:09:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:09:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:09:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc67971d1767eae5019ffeaf8f893e6d81dbba50bde347da0c0433c56e3f2a3`  
		Last Modified: Thu, 28 Sep 2023 22:18:17 GMT  
		Size: 286.7 KB (286659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1caf7fa003bdf7c7611eb2e33a11db077a0f632b70d28f5b73096bf051f25aeb`  
		Last Modified: Tue, 10 Oct 2023 19:28:09 GMT  
		Size: 64.1 MB (64125245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9573c5aef56335266ce720d0812f9a0156f628fbd01ba4a6462be56d8742dc8a`  
		Last Modified: Tue, 10 Oct 2023 19:27:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40b483d55ec27555b481cb0fad97faf6e8d1686165905df945c86967ec0ac96`  
		Last Modified: Sat, 21 Oct 2023 00:09:50 GMT  
		Size: 5.3 MB (5268969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966ad11dd0f3a17ae3666a37f54fd9d6265bc0e18133314a565abf1039e90a1f`  
		Last Modified: Sat, 21 Oct 2023 00:09:50 GMT  
		Size: 1.2 MB (1186175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e18b62f88891e2a1b8f7a5e8a66e6ee69c9f42fe03945d66da418c55d339a9`  
		Last Modified: Sat, 21 Oct 2023 00:09:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder` - linux; s390x

```console
$ docker pull caddy@sha256:02d085e00e424e29b1a4c45b6358c9ac90629ed72540af87be474238770f3217
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76112263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fa19320a45d01205e0025f17edf0aa856b433bd25ee512a7877ec407bdf0a3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:44:44 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 12:29:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 12:29:18 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 12:29:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 12:29:51 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 12:29:52 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 12:29:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 12:29:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 12:29:54 GMT
WORKDIR /go
# Wed, 01 Nov 2023 16:51:53 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 16:51:55 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 16:51:56 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 16:51:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 16:51:57 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 16:51:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 16:52:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 16:52:01 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f15a4d38dd3d4f044868149900a763ac233f1aef33fe18019f45149b6bd02c`  
		Last Modified: Sat, 21 Oct 2023 00:45:00 GMT  
		Size: 285.1 KB (285095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23831500ce8c52e3d80c9eab9eb44d36e8daf00224a75f36d961186e47851ae8`  
		Last Modified: Wed, 01 Nov 2023 12:38:38 GMT  
		Size: 66.2 MB (66234435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92c933a1dfb2cbb65a33ccba713aabb9ff92ce6a0286e12af67e54c51be8a44`  
		Last Modified: Wed, 01 Nov 2023 12:38:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368a8f32c470e61e32632b0c78836e09dc1d70ab0e9a48e1c2bef1d23de82f7d`  
		Last Modified: Wed, 01 Nov 2023 16:52:34 GMT  
		Size: 5.1 MB (5114679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b61d54a31e32a9c971c8d7ea514537dababa89a4e60ce97eca5bdcf4e8d007`  
		Last Modified: Wed, 01 Nov 2023 16:52:33 GMT  
		Size: 1.3 MB (1262390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147c37f0535cd57e5355158d43aa5608a1430f56aa08ef1b4eb9cea12976a728`  
		Last Modified: Wed, 01 Nov 2023 16:52:33 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder` - windows version 10.0.17763.4974; amd64

```console
$ docker pull caddy@sha256:951876270030a4a5404a8bab425d35b64f90babc594bb65c261cc05eab33ed79
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2128478401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:883908294a37d78f29e796d389d42c83a12c68a6c0f1113bba3bdd9290db5b05`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 02:23:09 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Oct 2023 02:23:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Oct 2023 02:23:11 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Oct 2023 02:23:12 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Oct 2023 02:24:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:24:31 GMT
ENV GOPATH=C:\go
# Wed, 11 Oct 2023 02:25:33 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Oct 2023 02:25:34 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 11 Oct 2023 02:28:30 GMT
RUN $url = 'https://dl.google.com/go/go1.21.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '27c8daf157493f288d42a6f38debc6a2cb391f6543139eba9152fceca0be2a10'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:28:31 GMT
WORKDIR C:\go
# Wed, 11 Oct 2023 04:03:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:03:14 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 12 Oct 2023 01:42:14 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:42:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 12 Oct 2023 01:43:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 12 Oct 2023 01:43:13 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fded5ce3c59d7e8d637a5536d6eed085ff6b6a323f42c1df76a7be6e9970ee`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a72a6b595ab9f8f71a34a065e75e609b20ea5e026f901820fce6d3c9134939`  
		Last Modified: Wed, 11 Oct 2023 02:46:39 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2574f8b7fb0ec5a8c39ee40a8008f0d24c398380247bf7140be1abdede5542b`  
		Last Modified: Wed, 11 Oct 2023 02:46:40 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951c53676fe729ebf5d3c07215d91afa952e6190715f79a7952f4c3aa121231e`  
		Last Modified: Wed, 11 Oct 2023 02:46:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a382bb149b70b82f9c2f58ebf6a2672dc4c64460017836d73a5a23b7379ea095`  
		Last Modified: Wed, 11 Oct 2023 02:46:44 GMT  
		Size: 25.6 MB (25557568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608a2584f4b3b8f3038fa41c0719005822ab967d85d1231843bd729a7b3d2d60`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1058e02ad62f976d823e3035f0578b2868eb09f28986153342a52014cc5c3810`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 284.8 KB (284754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fce039c31b2e60b62a0ede9974b6574519f2e47e1d8f4e09c7a1f30763aee95`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65449f183261f9bbdb731d41f5e6fca94f3e547e8d996133e418773400cfcfe`  
		Last Modified: Wed, 11 Oct 2023 02:46:59 GMT  
		Size: 69.3 MB (69345382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394e07c2ad53e950c47ffb647836822197dc5f8ebe082eaa045854e2b25bafc7`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993f5e59c63ef5be894fc498ab0e165faa3129d35a8a8f5173f12c6a4232f588`  
		Last Modified: Wed, 11 Oct 2023 04:06:31 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c675831130735b443a544dff1b9c188928f34947a5342350ef04eadc0d1ab27`  
		Last Modified: Wed, 11 Oct 2023 04:06:28 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69fe7c1d1f5383a4421f2a0e7284e17db440ee5b7be9f487ce9048f76970e7b6`  
		Last Modified: Thu, 12 Oct 2023 01:45:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee998763c3cef90b11adda3322e66e1a89d89409d1ed29dd73a4101fb657e29`  
		Last Modified: Thu, 12 Oct 2023 01:45:21 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196a81b981d5dc89b19acce594b87914fc5bc4777e42b1322ca9b9d4c4b4f179`  
		Last Modified: Thu, 12 Oct 2023 01:45:22 GMT  
		Size: 1.7 MB (1682335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3ad6e4e7b1be08f8a79e4d77328648deded93f9ef0d4a1e8202ce4c3a21c67`  
		Last Modified: Thu, 12 Oct 2023 01:45:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder` - windows version 10.0.20348.2031; amd64

```console
$ docker pull caddy@sha256:04b6c1b2519c8d35d65976c53b4523d7074d53c7b98fa5b29b83c837e021b493
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1956648108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6c3e402a7640df51573fae3237803e1e5fabce3d4c88849d9513c716654d474`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 02:19:41 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Oct 2023 02:19:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Oct 2023 02:19:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Oct 2023 02:19:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Oct 2023 02:20:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:20:18 GMT
ENV GOPATH=C:\go
# Wed, 11 Oct 2023 02:20:42 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Oct 2023 02:20:42 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 11 Oct 2023 02:22:59 GMT
RUN $url = 'https://dl.google.com/go/go1.21.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '27c8daf157493f288d42a6f38debc6a2cb391f6543139eba9152fceca0be2a10'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:23:01 GMT
WORKDIR C:\go
# Wed, 11 Oct 2023 04:04:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:04:42 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 12 Oct 2023 01:43:30 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:43:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 12 Oct 2023 01:43:51 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 12 Oct 2023 01:43:52 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60407a49ce6121c65fa6399c333c5227a09518414fd987c460ea29cb441ac5a`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe632e8cddda4e5f347720b87b8b3868e2e2969048761e3b0a40799d33f5f7a`  
		Last Modified: Wed, 11 Oct 2023 02:45:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4384696fc834e9658e7b3e5d1ceb1f8b362db85865daf29521b3c75c6999c046`  
		Last Modified: Wed, 11 Oct 2023 02:45:04 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c794ea611ef69f54d577f90b68e165e40a17e43b6d1d08f59951a38e084ea5fb`  
		Last Modified: Wed, 11 Oct 2023 02:45:03 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c74dc2d701da2bfabc4d44e6a4e6b92912515e2ca1fb053ffcc6b0d5cae2972`  
		Last Modified: Wed, 11 Oct 2023 02:45:08 GMT  
		Size: 25.5 MB (25531724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91612399ba7df8de0a05ad078c3817548f0a3b44516b76565e14a96ea62452e9`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7439c7c4353d2432c780827e4926910b19e84fe436d58e0a8129de2f631bd2b8`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 264.4 KB (264384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b0eaedd98e739ace4b7934261c71292195e461adcc977d02e57604d4a42ee8`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f46e84d4d007a200b1d6e7cb5b48db90116cdeb8bd3ec3964a08191875973e2`  
		Last Modified: Wed, 11 Oct 2023 02:45:25 GMT  
		Size: 69.3 MB (69325670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f59bab6d84ca44bbb60474dcf59c9af4f0f15edbdd64249b0eeaf968aff211f`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.6 KB (1556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f449f4d34d707dbde9cbb245c154c0b2e1d1a2c55d172501f8d7da576866f76f`  
		Last Modified: Wed, 11 Oct 2023 04:06:49 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a2edf76facdd17af03954b607484f7f7b36164a30634d19dd96b7320feb6b5`  
		Last Modified: Wed, 11 Oct 2023 04:06:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802c3686d509915fea71538d2c40c7a48c71719fab6144cb4497b6118b276ab9`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99cb183ed6cdad781eaba7bd1b4cb443befd9042c8a59450ee41f0245dd0ece4`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec33434b55fade6bcd7f3f0dfc10c981de93dc44bbae2b8702fdb6418a37a65b`  
		Last Modified: Thu, 12 Oct 2023 01:45:38 GMT  
		Size: 1.7 MB (1664788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0833369ef8236fcf99aba2d1fa48788db07662d0a9885a8429d435bf9f2227b2`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.5-builder-alpine`

```console
$ docker pull caddy@sha256:0b6ab47c59512267b3021fcb39af41d2896fd78718a39fa127cc8f2a4795638e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.7.5-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:d1f6d3dcfec129b4d0e23b6743f576807352958232a7ac6c17ee36f785fe5c58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76972374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e113a57232410dd987d12708b35062e6a269825fa7b4d03aef42c00acc93dce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:54:30 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:54:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:20:11 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:20:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 19:20:22 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:20:22 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:20:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:20:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:20:23 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:11:20 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:11:20 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:11:20 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:11:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:11:21 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:11:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:11:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:11:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc37b24bb09971feb8bf4882e861bce9db0c985a16a900adb0dc9de3f854243b`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 284.7 KB (284690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a4303e95078c253686dcc16d7717644af63809efcbd753c0a999c9aad3fe72`  
		Last Modified: Tue, 10 Oct 2023 19:26:17 GMT  
		Size: 67.0 MB (67012876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359925be0f358b952dc8be63647139c5aab0fff94f7a070d88cb51dd258f80e5`  
		Last Modified: Tue, 10 Oct 2023 19:26:06 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958092cb44d28ddde181d193284001b1146b33a1cf19624e9683fc8f31551043`  
		Last Modified: Sat, 21 Oct 2023 00:11:52 GMT  
		Size: 5.0 MB (4970044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85cdb072dd78dcf6a7b04409cf7c8dc1fddddf912b601b15c6dc94adb2df10b`  
		Last Modified: Sat, 21 Oct 2023 00:11:51 GMT  
		Size: 1.3 MB (1302237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32749367842b0c8b40e7f61a315ff21b4d42211b5399e648beb75d86acb29c4c`  
		Last Modified: Sat, 21 Oct 2023 00:11:51 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:15f0db6d62062758441d2d22fd178c42299cf148c5097ffe10468153ff40c6b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75413855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:509cf858d9f3ffa4a94fe988705864c41bd510f34ade4ece0d2ede4cda23599f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:55:22 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:55:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 18:49:21 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 18:49:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 18:49:42 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 18:49:42 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 18:49:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 18:49:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 18:49:43 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:06:57 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:06:57 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:06:58 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:06:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:06:58 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:06:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:06:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:06:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3da3b9e7a12f6bb6b7f56e9240c2c92ce8c9f5fd5ef3b3063b9a93d454919e`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 284.9 KB (284887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbbb7b34bc324d050e49d3dd31294bdde5d6ecda33decf9afe31c11165b138a`  
		Last Modified: Tue, 10 Oct 2023 18:55:32 GMT  
		Size: 65.8 MB (65770135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c022f45a9fb1e7649eb4a663acd4ed6437363b4fc6e56f6af3e5f457a5d06ee8`  
		Last Modified: Tue, 10 Oct 2023 18:55:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12bec1760d3cf2773adbb14bd47431e46e130a914a46535c9a70de28e4b363b`  
		Last Modified: Sat, 21 Oct 2023 00:07:30 GMT  
		Size: 5.0 MB (4964316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888b304960048015ef929fcb0ffab750c1ba463aaf1d419272f2233e67195d56`  
		Last Modified: Sat, 21 Oct 2023 00:07:30 GMT  
		Size: 1.2 MB (1248665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00237a85b25c3b9ee3968fe9e98da8f378a4a70ccc746a6524820916085348ef`  
		Last Modified: Sat, 21 Oct 2023 00:07:29 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9275f10d0ef0db0999dc5ed6b19c068a941f59a05d69fad4b3cb07c3f0b14a7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74714658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b10f4fd814dc9e97d1147715baacffedd007b23ec081f4c100520df02050e6c9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:07:30 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 15:58:50 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:58:50 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 15:59:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 15:59:08 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 15:59:08 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 15:59:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:59:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 15:59:09 GMT
WORKDIR /go
# Wed, 01 Nov 2023 21:17:21 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 21:17:22 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 21:17:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 21:17:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 21:17:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8457acc181d300b4231b44e12aa0bf4a99ced5d51c5dfdc14eb899a341d5b855`  
		Last Modified: Sat, 21 Oct 2023 01:07:42 GMT  
		Size: 284.1 KB (284074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05626b790821d279bd9aea8466a1a79307764cbc389c51ab081a4b98c7657dc2`  
		Last Modified: Wed, 01 Nov 2023 16:06:11 GMT  
		Size: 65.8 MB (65772806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2dba3cbff62191bbc046c664eead34e3af26adfa5ecdbacf0ba6e73b9cbe51`  
		Last Modified: Wed, 01 Nov 2023 16:05:56 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357de4175525102c1d6c8d4fc605461ca1b1791b2a3b6c55c73e3ef6266159ad`  
		Last Modified: Wed, 01 Nov 2023 21:17:50 GMT  
		Size: 4.5 MB (4511226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59aa4bdeb70fa8c96a09911a5e79184a493cb38488e04d22007af9f9164e4f44`  
		Last Modified: Wed, 01 Nov 2023 21:17:50 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7b450bb18e60383a1dd8c51f37de16c5782ba7eba9e2737540247f3a4394c8`  
		Last Modified: Wed, 01 Nov 2023 21:17:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:76d3844fa9c17929397bb168745241a1f8fa36bf63c437d9d255fe217ec6a87c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73995976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6b4383d952151327974f3f21fa7be1e862f9a67c4ee08a264948e4372890be6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 02:41:07 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 15:36:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:36:13 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 15:36:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 15:36:23 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 15:36:23 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 15:36:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:36:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 15:36:24 GMT
WORKDIR /go
# Wed, 01 Nov 2023 19:56:22 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 19:56:22 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 19:56:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 19:56:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 19:56:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74bf0db6f91dfe1899e8204affb86f8c505a5643bdcb83b085888c86e0c7411`  
		Last Modified: Sat, 21 Oct 2023 02:41:18 GMT  
		Size: 286.3 KB (286297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd442d12e388d3f44ee4325caf9e959ca82d4064c8b1b38321da75a84a6ccbd`  
		Last Modified: Wed, 01 Nov 2023 15:41:04 GMT  
		Size: 64.1 MB (64110459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0297817440f5024a6c0e27f7906a375aa91aea5aaf191caa3f1762426e60e9c2`  
		Last Modified: Wed, 01 Nov 2023 15:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9fb63180b1c62b2cfd436428dc31a25bc97989024e217b9d8e508e82b0b287`  
		Last Modified: Wed, 01 Nov 2023 19:56:42 GMT  
		Size: 5.1 MB (5068382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0ee6df11f2e2e143f36f30697c4b309c4560fa062faa2fcb3a1c22db91257e`  
		Last Modified: Wed, 01 Nov 2023 19:56:42 GMT  
		Size: 1.2 MB (1198448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15b8268dd8cba7445da5d02c68c6787ce774d7ecc7dba9fa3f2775a88884d64`  
		Last Modified: Wed, 01 Nov 2023 19:56:41 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:ed1e2679ee802b3a2c8f7b42d4828ecc9ba50b5a029e3d14bbc54fa2a0fc5444
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74214117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2041e14adf1ce1c2b331135049ec2871be632eb2a7130142af035fa662cb1e19`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:13:11 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:13:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:17:44 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:18:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 19:18:14 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:18:14 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:18:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:18:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:18:17 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:09:16 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:09:17 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:09:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:09:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:09:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc67971d1767eae5019ffeaf8f893e6d81dbba50bde347da0c0433c56e3f2a3`  
		Last Modified: Thu, 28 Sep 2023 22:18:17 GMT  
		Size: 286.7 KB (286659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1caf7fa003bdf7c7611eb2e33a11db077a0f632b70d28f5b73096bf051f25aeb`  
		Last Modified: Tue, 10 Oct 2023 19:28:09 GMT  
		Size: 64.1 MB (64125245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9573c5aef56335266ce720d0812f9a0156f628fbd01ba4a6462be56d8742dc8a`  
		Last Modified: Tue, 10 Oct 2023 19:27:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40b483d55ec27555b481cb0fad97faf6e8d1686165905df945c86967ec0ac96`  
		Last Modified: Sat, 21 Oct 2023 00:09:50 GMT  
		Size: 5.3 MB (5268969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966ad11dd0f3a17ae3666a37f54fd9d6265bc0e18133314a565abf1039e90a1f`  
		Last Modified: Sat, 21 Oct 2023 00:09:50 GMT  
		Size: 1.2 MB (1186175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e18b62f88891e2a1b8f7a5e8a66e6ee69c9f42fe03945d66da418c55d339a9`  
		Last Modified: Sat, 21 Oct 2023 00:09:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:02d085e00e424e29b1a4c45b6358c9ac90629ed72540af87be474238770f3217
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76112263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fa19320a45d01205e0025f17edf0aa856b433bd25ee512a7877ec407bdf0a3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:44:44 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 12:29:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 12:29:18 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 12:29:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 12:29:51 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 12:29:52 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 12:29:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 12:29:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 12:29:54 GMT
WORKDIR /go
# Wed, 01 Nov 2023 16:51:53 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 16:51:55 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 16:51:56 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 16:51:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 16:51:57 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 16:51:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 16:52:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 16:52:01 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f15a4d38dd3d4f044868149900a763ac233f1aef33fe18019f45149b6bd02c`  
		Last Modified: Sat, 21 Oct 2023 00:45:00 GMT  
		Size: 285.1 KB (285095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23831500ce8c52e3d80c9eab9eb44d36e8daf00224a75f36d961186e47851ae8`  
		Last Modified: Wed, 01 Nov 2023 12:38:38 GMT  
		Size: 66.2 MB (66234435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92c933a1dfb2cbb65a33ccba713aabb9ff92ce6a0286e12af67e54c51be8a44`  
		Last Modified: Wed, 01 Nov 2023 12:38:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368a8f32c470e61e32632b0c78836e09dc1d70ab0e9a48e1c2bef1d23de82f7d`  
		Last Modified: Wed, 01 Nov 2023 16:52:34 GMT  
		Size: 5.1 MB (5114679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b61d54a31e32a9c971c8d7ea514537dababa89a4e60ce97eca5bdcf4e8d007`  
		Last Modified: Wed, 01 Nov 2023 16:52:33 GMT  
		Size: 1.3 MB (1262390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147c37f0535cd57e5355158d43aa5608a1430f56aa08ef1b4eb9cea12976a728`  
		Last Modified: Wed, 01 Nov 2023 16:52:33 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.5-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:c0740b75861440c921e23bec00c2ce3e14bda7ca7967b2aec7855352ea96cd0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `caddy:2.7.5-builder-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull caddy@sha256:951876270030a4a5404a8bab425d35b64f90babc594bb65c261cc05eab33ed79
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2128478401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:883908294a37d78f29e796d389d42c83a12c68a6c0f1113bba3bdd9290db5b05`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 02:23:09 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Oct 2023 02:23:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Oct 2023 02:23:11 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Oct 2023 02:23:12 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Oct 2023 02:24:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:24:31 GMT
ENV GOPATH=C:\go
# Wed, 11 Oct 2023 02:25:33 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Oct 2023 02:25:34 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 11 Oct 2023 02:28:30 GMT
RUN $url = 'https://dl.google.com/go/go1.21.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '27c8daf157493f288d42a6f38debc6a2cb391f6543139eba9152fceca0be2a10'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:28:31 GMT
WORKDIR C:\go
# Wed, 11 Oct 2023 04:03:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:03:14 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 12 Oct 2023 01:42:14 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:42:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 12 Oct 2023 01:43:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 12 Oct 2023 01:43:13 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fded5ce3c59d7e8d637a5536d6eed085ff6b6a323f42c1df76a7be6e9970ee`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a72a6b595ab9f8f71a34a065e75e609b20ea5e026f901820fce6d3c9134939`  
		Last Modified: Wed, 11 Oct 2023 02:46:39 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2574f8b7fb0ec5a8c39ee40a8008f0d24c398380247bf7140be1abdede5542b`  
		Last Modified: Wed, 11 Oct 2023 02:46:40 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951c53676fe729ebf5d3c07215d91afa952e6190715f79a7952f4c3aa121231e`  
		Last Modified: Wed, 11 Oct 2023 02:46:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a382bb149b70b82f9c2f58ebf6a2672dc4c64460017836d73a5a23b7379ea095`  
		Last Modified: Wed, 11 Oct 2023 02:46:44 GMT  
		Size: 25.6 MB (25557568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608a2584f4b3b8f3038fa41c0719005822ab967d85d1231843bd729a7b3d2d60`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1058e02ad62f976d823e3035f0578b2868eb09f28986153342a52014cc5c3810`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 284.8 KB (284754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fce039c31b2e60b62a0ede9974b6574519f2e47e1d8f4e09c7a1f30763aee95`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65449f183261f9bbdb731d41f5e6fca94f3e547e8d996133e418773400cfcfe`  
		Last Modified: Wed, 11 Oct 2023 02:46:59 GMT  
		Size: 69.3 MB (69345382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394e07c2ad53e950c47ffb647836822197dc5f8ebe082eaa045854e2b25bafc7`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993f5e59c63ef5be894fc498ab0e165faa3129d35a8a8f5173f12c6a4232f588`  
		Last Modified: Wed, 11 Oct 2023 04:06:31 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c675831130735b443a544dff1b9c188928f34947a5342350ef04eadc0d1ab27`  
		Last Modified: Wed, 11 Oct 2023 04:06:28 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69fe7c1d1f5383a4421f2a0e7284e17db440ee5b7be9f487ce9048f76970e7b6`  
		Last Modified: Thu, 12 Oct 2023 01:45:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee998763c3cef90b11adda3322e66e1a89d89409d1ed29dd73a4101fb657e29`  
		Last Modified: Thu, 12 Oct 2023 01:45:21 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196a81b981d5dc89b19acce594b87914fc5bc4777e42b1322ca9b9d4c4b4f179`  
		Last Modified: Thu, 12 Oct 2023 01:45:22 GMT  
		Size: 1.7 MB (1682335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3ad6e4e7b1be08f8a79e4d77328648deded93f9ef0d4a1e8202ce4c3a21c67`  
		Last Modified: Thu, 12 Oct 2023 01:45:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.5-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:7a4eaeb7416d6a4b442d55eab7e8c7824e36a07baef33353084b943d46b6b7b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `caddy:2.7.5-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull caddy@sha256:04b6c1b2519c8d35d65976c53b4523d7074d53c7b98fa5b29b83c837e021b493
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1956648108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6c3e402a7640df51573fae3237803e1e5fabce3d4c88849d9513c716654d474`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 02:19:41 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Oct 2023 02:19:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Oct 2023 02:19:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Oct 2023 02:19:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Oct 2023 02:20:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:20:18 GMT
ENV GOPATH=C:\go
# Wed, 11 Oct 2023 02:20:42 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Oct 2023 02:20:42 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 11 Oct 2023 02:22:59 GMT
RUN $url = 'https://dl.google.com/go/go1.21.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '27c8daf157493f288d42a6f38debc6a2cb391f6543139eba9152fceca0be2a10'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:23:01 GMT
WORKDIR C:\go
# Wed, 11 Oct 2023 04:04:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:04:42 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 12 Oct 2023 01:43:30 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:43:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 12 Oct 2023 01:43:51 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 12 Oct 2023 01:43:52 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60407a49ce6121c65fa6399c333c5227a09518414fd987c460ea29cb441ac5a`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe632e8cddda4e5f347720b87b8b3868e2e2969048761e3b0a40799d33f5f7a`  
		Last Modified: Wed, 11 Oct 2023 02:45:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4384696fc834e9658e7b3e5d1ceb1f8b362db85865daf29521b3c75c6999c046`  
		Last Modified: Wed, 11 Oct 2023 02:45:04 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c794ea611ef69f54d577f90b68e165e40a17e43b6d1d08f59951a38e084ea5fb`  
		Last Modified: Wed, 11 Oct 2023 02:45:03 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c74dc2d701da2bfabc4d44e6a4e6b92912515e2ca1fb053ffcc6b0d5cae2972`  
		Last Modified: Wed, 11 Oct 2023 02:45:08 GMT  
		Size: 25.5 MB (25531724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91612399ba7df8de0a05ad078c3817548f0a3b44516b76565e14a96ea62452e9`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7439c7c4353d2432c780827e4926910b19e84fe436d58e0a8129de2f631bd2b8`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 264.4 KB (264384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b0eaedd98e739ace4b7934261c71292195e461adcc977d02e57604d4a42ee8`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f46e84d4d007a200b1d6e7cb5b48db90116cdeb8bd3ec3964a08191875973e2`  
		Last Modified: Wed, 11 Oct 2023 02:45:25 GMT  
		Size: 69.3 MB (69325670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f59bab6d84ca44bbb60474dcf59c9af4f0f15edbdd64249b0eeaf968aff211f`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.6 KB (1556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f449f4d34d707dbde9cbb245c154c0b2e1d1a2c55d172501f8d7da576866f76f`  
		Last Modified: Wed, 11 Oct 2023 04:06:49 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a2edf76facdd17af03954b607484f7f7b36164a30634d19dd96b7320feb6b5`  
		Last Modified: Wed, 11 Oct 2023 04:06:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802c3686d509915fea71538d2c40c7a48c71719fab6144cb4497b6118b276ab9`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99cb183ed6cdad781eaba7bd1b4cb443befd9042c8a59450ee41f0245dd0ece4`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec33434b55fade6bcd7f3f0dfc10c981de93dc44bbae2b8702fdb6418a37a65b`  
		Last Modified: Thu, 12 Oct 2023 01:45:38 GMT  
		Size: 1.7 MB (1664788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0833369ef8236fcf99aba2d1fa48788db07662d0a9885a8429d435bf9f2227b2`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.5-windowsservercore`

```console
$ docker pull caddy@sha256:b859825f1b8093a4b961d02fb945e63f5180c5e07e56ce7495384835c016c47d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4974; amd64
	-	windows version 10.0.20348.2031; amd64

### `caddy:2.7.5-windowsservercore` - windows version 10.0.17763.4974; amd64

```console
$ docker pull caddy@sha256:77cb1b0b8315f376e69becef400d33c9d8b2a45548714845a821736158771de2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2047649951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3171dc2f25b4435520d8ba983ebf42f070ddec217b0da7677e309cc4cd51b05`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 03:59:19 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:39:06 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:40:04 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:40:05 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:40:06 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:40:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:40:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:40:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:40:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:40:12 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:40:13 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:41:01 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:41:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c4565a9b36858bc727874537e3c99968438a37e53c13057b0b1a233699d014`  
		Last Modified: Wed, 11 Oct 2023 04:05:44 GMT  
		Size: 472.0 KB (472034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df4a75108d3a33583e7ae61f1a019d4865860820bd89280ba414af94dd3f56e`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9dee9792a7bf7e1225840c56fb692536bee1743eba0a4da2faff34533f1160f`  
		Last Modified: Thu, 12 Oct 2023 01:44:37 GMT  
		Size: 15.3 MB (15296055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41900185a2519f01b8bd860f70936cee271612c4023512694b105826e0e0251`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0f1b69a12cd8550d868156e54168abaa32e1df40ee6eb39bc4e173ce04905e`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca266891343bff15b313846692ba3a41f313d5b228bedde964191332a16dffe`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12539eb7433a69ed67556d91b75b66dfedf0543d3efd7dabe82772437307a6f`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5103f279ed518bcfec88e00183e3222b50c1bc2f0e5b42f043e2198da424de98`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efc1cff2dac4308ce732a395ee215e1497d21f737e42e77917debf070afa8d7`  
		Last Modified: Thu, 12 Oct 2023 01:44:35 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cb50f59d2b11532a330925afb6ebd04d9b4708de8b11ae436e258c3764d741`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd11a311e4c0cf49bb544980f2c999751fc5e2fbe80d37b0f719f837abf8c3f`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ccbee9a6b9058ec933797dc1cfed875ceeb0115ce29ee163cd60a66e9f3b2d`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b486fc8ef055010a59374557443d3b713b9e55c1ccd11b7873f47876758976`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41df430d9a95c6000c922dd021b6cb2af0110dcc661ddc37a190a8cf6cd4bb06`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f243061a2e17d508efa4a424310d9ca158ca0cf0f59bd15cac606ab3e74701`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e709fff7d020a5d7c2d9e9e9a664c87392e9f9a4f4ced9802e64ca268995e23`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2c7aca9b511bc62340e6e8883d5f625bdccb805c4e897b837b68f3c79964b5`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38802c5a2b45b7029b250d88dac8209405146b0968925d1204cf17f7c3e76d98`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 269.1 KB (269086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376d19318a370d0da2ffcc29b47c2810278efa9d22fb39799c48687dfee0a2d9`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-windowsservercore` - windows version 10.0.20348.2031; amd64

```console
$ docker pull caddy@sha256:05f529a68927f0acfa7afbc79b7a19541f94430c137612ed344de7a822dcfafb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1875907229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8701a0e5aada270070acddeed89c57e20a5cac8afd88ed58da9557bf01dccb27`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:02:07 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:41:20 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:41:42 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:41:42 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:41:43 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:41:44 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:41:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:41:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:41:50 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:41:52 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:42:04 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:42:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c36616366b0df84f087a09bf19876f3872d839997f2f43e4eb8599861417c06`  
		Last Modified: Wed, 11 Oct 2023 04:06:10 GMT  
		Size: 467.9 KB (467933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db420ca589f10e4f9f5bc9dd6badc855d95c6a598888f2eb77a747eced259557`  
		Last Modified: Thu, 12 Oct 2023 01:45:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b5d7433dab05533d906a290a0f42cf31804c132da65c9fd7d4d2c41a64f519`  
		Last Modified: Thu, 12 Oct 2023 01:45:04 GMT  
		Size: 15.3 MB (15284209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62069fdf38bff9495ef2be05d397a55221536f9eec345734d6acec3a6196324f`  
		Last Modified: Thu, 12 Oct 2023 01:45:00 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e237a4c373c6937b5c51d0a3936152ac2b572fd5a432db3690f4070a7c78327`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73fae1c57e166a2ade87aa32e11980b456658212b296eea0f02ba3ec1c6557b`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000f2101dc464fa43321619c6e65c5b9e62b62755f3b141e69bd31892a253ded`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8536723423849b861a08fa490135f690c287be0144267e38fb3e631fb1bddbd2`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f176ef86531863755c3a315ec662b8da324474ae6097d7365dc18b76d61bde5`  
		Last Modified: Thu, 12 Oct 2023 01:44:58 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3973c168b3a63daa069e3a9870395561709d7b27762ffafb16538c773a16ad29`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5a10fbc59abc7ee7cc04a7ff48cc85983728745e91e8ef5fafee0589ba2193`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf033f8ab12414230e08aaada214c761777b0c784908ad2783ee31f8d330d0c9`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e2af83b2af59d76bd9b735c4e71b9492d9dbc120c042b8134ae0a70008f49`  
		Last Modified: Thu, 12 Oct 2023 01:44:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0355ed819405072f13996095ae7ec7044017bee81808dea9500459620118c20b`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e86117e27425829055f627e6156a4a657d9817cf8d2158f0026752366c9022c`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22fbe71be2fe08164a92f1362959f0a4aba194dcf931945d7bb2ac50e8f6467`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed768b9f807d51e5834f0bc8b2ea4dda09a5139d126f9141cb3db51f781ea541`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359fc3c79eda3ddbb39c46b09a4c68137a693a72f8712182d545c546b726027e`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 289.5 KB (289533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e4b8683a429393010114c6906acced22d65d5167cda2cc55238ae5b9f816c0`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.5-windowsservercore-1809`

```console
$ docker pull caddy@sha256:8169d134dfa19ddbba9eeeb7210c5227c2a61f00906c340474aab1250aba47f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `caddy:2.7.5-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull caddy@sha256:77cb1b0b8315f376e69becef400d33c9d8b2a45548714845a821736158771de2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2047649951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3171dc2f25b4435520d8ba983ebf42f070ddec217b0da7677e309cc4cd51b05`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 03:59:19 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:39:06 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:40:04 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:40:05 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:40:06 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:40:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:40:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:40:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:40:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:40:12 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:40:13 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:41:01 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:41:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c4565a9b36858bc727874537e3c99968438a37e53c13057b0b1a233699d014`  
		Last Modified: Wed, 11 Oct 2023 04:05:44 GMT  
		Size: 472.0 KB (472034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df4a75108d3a33583e7ae61f1a019d4865860820bd89280ba414af94dd3f56e`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9dee9792a7bf7e1225840c56fb692536bee1743eba0a4da2faff34533f1160f`  
		Last Modified: Thu, 12 Oct 2023 01:44:37 GMT  
		Size: 15.3 MB (15296055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41900185a2519f01b8bd860f70936cee271612c4023512694b105826e0e0251`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0f1b69a12cd8550d868156e54168abaa32e1df40ee6eb39bc4e173ce04905e`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca266891343bff15b313846692ba3a41f313d5b228bedde964191332a16dffe`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12539eb7433a69ed67556d91b75b66dfedf0543d3efd7dabe82772437307a6f`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5103f279ed518bcfec88e00183e3222b50c1bc2f0e5b42f043e2198da424de98`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efc1cff2dac4308ce732a395ee215e1497d21f737e42e77917debf070afa8d7`  
		Last Modified: Thu, 12 Oct 2023 01:44:35 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cb50f59d2b11532a330925afb6ebd04d9b4708de8b11ae436e258c3764d741`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd11a311e4c0cf49bb544980f2c999751fc5e2fbe80d37b0f719f837abf8c3f`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ccbee9a6b9058ec933797dc1cfed875ceeb0115ce29ee163cd60a66e9f3b2d`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b486fc8ef055010a59374557443d3b713b9e55c1ccd11b7873f47876758976`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41df430d9a95c6000c922dd021b6cb2af0110dcc661ddc37a190a8cf6cd4bb06`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f243061a2e17d508efa4a424310d9ca158ca0cf0f59bd15cac606ab3e74701`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e709fff7d020a5d7c2d9e9e9a664c87392e9f9a4f4ced9802e64ca268995e23`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2c7aca9b511bc62340e6e8883d5f625bdccb805c4e897b837b68f3c79964b5`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38802c5a2b45b7029b250d88dac8209405146b0968925d1204cf17f7c3e76d98`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 269.1 KB (269086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376d19318a370d0da2ffcc29b47c2810278efa9d22fb39799c48687dfee0a2d9`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.5-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:278d32be7fb2f9a5e3f48ea6a672747dbb4ad6256e4802aff4a1e11a67e2e518
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `caddy:2.7.5-windowsservercore-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull caddy@sha256:05f529a68927f0acfa7afbc79b7a19541f94430c137612ed344de7a822dcfafb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1875907229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8701a0e5aada270070acddeed89c57e20a5cac8afd88ed58da9557bf01dccb27`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:02:07 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:41:20 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:41:42 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:41:42 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:41:43 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:41:44 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:41:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:41:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:41:50 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:41:52 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:42:04 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:42:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c36616366b0df84f087a09bf19876f3872d839997f2f43e4eb8599861417c06`  
		Last Modified: Wed, 11 Oct 2023 04:06:10 GMT  
		Size: 467.9 KB (467933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db420ca589f10e4f9f5bc9dd6badc855d95c6a598888f2eb77a747eced259557`  
		Last Modified: Thu, 12 Oct 2023 01:45:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b5d7433dab05533d906a290a0f42cf31804c132da65c9fd7d4d2c41a64f519`  
		Last Modified: Thu, 12 Oct 2023 01:45:04 GMT  
		Size: 15.3 MB (15284209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62069fdf38bff9495ef2be05d397a55221536f9eec345734d6acec3a6196324f`  
		Last Modified: Thu, 12 Oct 2023 01:45:00 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e237a4c373c6937b5c51d0a3936152ac2b572fd5a432db3690f4070a7c78327`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73fae1c57e166a2ade87aa32e11980b456658212b296eea0f02ba3ec1c6557b`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000f2101dc464fa43321619c6e65c5b9e62b62755f3b141e69bd31892a253ded`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8536723423849b861a08fa490135f690c287be0144267e38fb3e631fb1bddbd2`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f176ef86531863755c3a315ec662b8da324474ae6097d7365dc18b76d61bde5`  
		Last Modified: Thu, 12 Oct 2023 01:44:58 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3973c168b3a63daa069e3a9870395561709d7b27762ffafb16538c773a16ad29`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5a10fbc59abc7ee7cc04a7ff48cc85983728745e91e8ef5fafee0589ba2193`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf033f8ab12414230e08aaada214c761777b0c784908ad2783ee31f8d330d0c9`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e2af83b2af59d76bd9b735c4e71b9492d9dbc120c042b8134ae0a70008f49`  
		Last Modified: Thu, 12 Oct 2023 01:44:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0355ed819405072f13996095ae7ec7044017bee81808dea9500459620118c20b`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e86117e27425829055f627e6156a4a657d9817cf8d2158f0026752366c9022c`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22fbe71be2fe08164a92f1362959f0a4aba194dcf931945d7bb2ac50e8f6467`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed768b9f807d51e5834f0bc8b2ea4dda09a5139d126f9141cb3db51f781ea541`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359fc3c79eda3ddbb39c46b09a4c68137a693a72f8712182d545c546b726027e`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 289.5 KB (289533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e4b8683a429393010114c6906acced22d65d5167cda2cc55238ae5b9f816c0`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:f1c092da9fcba7a8197cf1065a347d4f0bb67b6dd188985eafaf0a5aec6c9041
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
$ docker pull caddy@sha256:a9c7585fdc50bb28d686b73a9b1f0eb9a3d103efd63c48dc334ccb5f51aa1722
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18474311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70c3913f54e294079c54cc8b651576b08dd4add42a0f4c0bc93d539913ae335d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:11:11 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:11:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:11:12 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:11:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:11:15 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:11:15 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:11:16 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:11:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5433daac73cddf3f03243a31c38d460570073f83e9a8cf64c7f0e3387b85807`  
		Last Modified: Sat, 21 Oct 2023 00:11:36 GMT  
		Size: 350.8 KB (350840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c6b4aafe2c09344f58425bb0fe037a429808edb7b2ba37d79cd35b2775a422`  
		Last Modified: Sat, 21 Oct 2023 00:11:36 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a182bff4e1b33f3d5dd80f809e697793466287c3da7704863c3d0b51d42b5b`  
		Last Modified: Sat, 21 Oct 2023 00:11:39 GMT  
		Size: 14.7 MB (14713998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f43da8d65d754093117d4c673a7b725316be4e576e32b0d40c995e6ab1a07b7c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17422245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18b3bb2c3e0a97c9fe052eca67890f691907de7a5b514e88a44e660bb905079b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:06:46 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:06:48 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:06:48 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:06:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:06:51 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:06:51 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:06:52 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:06:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e09dc0459583a6ad3ba0428d5e180b7e3e6ae28360a69e293f03632cec397a0`  
		Last Modified: Sat, 21 Oct 2023 00:07:14 GMT  
		Size: 347.6 KB (347617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4705ff25da68d95a4bd671cbd4cec69369ea788be53bfafb45cdf4a930a725f8`  
		Last Modified: Sat, 21 Oct 2023 00:07:13 GMT  
		Size: 7.5 KB (7504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969c487cd333c7b53a7f57017e0ad77490d3806d9e52259caf9772016e96576d`  
		Last Modified: Sat, 21 Oct 2023 00:07:16 GMT  
		Size: 13.9 MB (13921833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:dd028bb08526d3533680243c94b9464c9c1a6559dccf5dde3b61ec73b9afd002
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17155303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:539aa551acc109f33c6ea5076a1f518af4d0476b517dc698d98c7350e8cb1b1a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:17:55 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:17:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:17:56 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:17:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:17:59 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:17:59 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:18:00 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:18:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee93e167fdbd8e67ec3f4ed8eaf242e5c8022a9845dd4f797448503af15d777c`  
		Last Modified: Sat, 21 Oct 2023 00:18:22 GMT  
		Size: 344.5 KB (344454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2895c0143aa41e87473191f749160d3109330cdb9de0c90a9b0a9e60e8a3a3e`  
		Last Modified: Sat, 21 Oct 2023 00:18:22 GMT  
		Size: 7.5 KB (7508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f015da3d3488ea9171b2970be40718bfa7e31496bae565a9bc2b677e53c09915`  
		Last Modified: Sat, 21 Oct 2023 00:18:25 GMT  
		Size: 13.9 MB (13903436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:d18ec23ab87841ede7ccefc353c20d1554faddf3ac362213c32ae22311136da5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17273763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cbdde935029392921ca3521ef9ebdb6a2b46cd1d4b7a9dabf0b71b00c593572`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:23:28 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:23:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:23:29 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:23:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:23:31 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:23:31 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:23:32 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:23:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461fe4f467fe88a160e176c442825b4bfea8dde13fc2324393a5d81518375e6f`  
		Last Modified: Sat, 21 Oct 2023 00:23:52 GMT  
		Size: 360.6 KB (360623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9335adc9ff07e38d963f0a71a2f7db01b5b5ed8e9d93fba14e584f25ea05c29d`  
		Last Modified: Sat, 21 Oct 2023 00:23:52 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32426666f5ec8621a07038733361be24f83719a812c0cce54e3f41192b31c2d`  
		Last Modified: Sat, 21 Oct 2023 00:23:54 GMT  
		Size: 13.6 MB (13573803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:1cd57ee42a4e84e91731e9182350ab4fd5b26705ec7286c28c5768c549435fd5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.1 MB (17057167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5aa3d5c5c63bea353c483de170ae8690a4f7eb12042cb84dc2bf0d52bf914b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:09:00 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:09:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:09:02 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:09:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:09:05 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:09:05 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:09:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:09:09 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:09:09 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:09:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692440f8f5ba2c6efbf2e74e3301377e3d9a90ae5a7cbd728c771ab306277830`  
		Last Modified: Sat, 21 Oct 2023 00:09:34 GMT  
		Size: 362.2 KB (362183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2886f5cbb210969eea27d97b8a48d88cae7bbe1bdd528a2b2775a8affde3084`  
		Last Modified: Sat, 21 Oct 2023 00:09:33 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdd6a19a7b9d3f4621c5388c53b0a9ea5591e9e72250bc60bcf22ed672632b1`  
		Last Modified: Sat, 21 Oct 2023 00:09:36 GMT  
		Size: 13.3 MB (13340969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:7dc6afd9bb40ff4450e4282bc56431b993d068c5b832c914dd50831189920061
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.8 MB (17822696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be3873facfc56aac0a1a9659efab4cddfc06afe6ac27c54cdd1b6fc9a23f1c1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:05:23 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:05:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:05:24 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:05:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:05:27 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:05:27 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:05:29 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:05:29 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:05:29 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d6d08cebdb83ff91ba335e0c4aec115b17261ed40307aaee6adde8c6763ad6`  
		Last Modified: Sat, 21 Oct 2023 00:06:00 GMT  
		Size: 355.0 KB (354963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58e0c7856c877cacd1d63a86beb12c9be91c4a0950dd85954db6f16a6d93103`  
		Last Modified: Sat, 21 Oct 2023 00:06:00 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69bf19674eec620ff3f87ecb754c60b7c137eb6c8c3763ff795739061593a77`  
		Last Modified: Sat, 21 Oct 2023 00:06:02 GMT  
		Size: 14.2 MB (14245123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:d039cffaec2ce64db9cae84dc789bb36c8d3d09e6ff70f3a40c4f405a89deed8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4974; amd64
	-	windows version 10.0.20348.2031; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:d1f6d3dcfec129b4d0e23b6743f576807352958232a7ac6c17ee36f785fe5c58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76972374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e113a57232410dd987d12708b35062e6a269825fa7b4d03aef42c00acc93dce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:54:30 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:54:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:20:11 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:20:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 19:20:22 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:20:22 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:20:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:20:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:20:23 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:11:20 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:11:20 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:11:20 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:11:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:11:21 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:11:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:11:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:11:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc37b24bb09971feb8bf4882e861bce9db0c985a16a900adb0dc9de3f854243b`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 284.7 KB (284690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a4303e95078c253686dcc16d7717644af63809efcbd753c0a999c9aad3fe72`  
		Last Modified: Tue, 10 Oct 2023 19:26:17 GMT  
		Size: 67.0 MB (67012876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359925be0f358b952dc8be63647139c5aab0fff94f7a070d88cb51dd258f80e5`  
		Last Modified: Tue, 10 Oct 2023 19:26:06 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958092cb44d28ddde181d193284001b1146b33a1cf19624e9683fc8f31551043`  
		Last Modified: Sat, 21 Oct 2023 00:11:52 GMT  
		Size: 5.0 MB (4970044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85cdb072dd78dcf6a7b04409cf7c8dc1fddddf912b601b15c6dc94adb2df10b`  
		Last Modified: Sat, 21 Oct 2023 00:11:51 GMT  
		Size: 1.3 MB (1302237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32749367842b0c8b40e7f61a315ff21b4d42211b5399e648beb75d86acb29c4c`  
		Last Modified: Sat, 21 Oct 2023 00:11:51 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:15f0db6d62062758441d2d22fd178c42299cf148c5097ffe10468153ff40c6b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75413855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:509cf858d9f3ffa4a94fe988705864c41bd510f34ade4ece0d2ede4cda23599f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:55:22 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:55:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 18:49:21 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 18:49:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 18:49:42 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 18:49:42 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 18:49:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 18:49:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 18:49:43 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:06:57 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:06:57 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:06:58 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:06:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:06:58 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:06:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:06:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:06:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3da3b9e7a12f6bb6b7f56e9240c2c92ce8c9f5fd5ef3b3063b9a93d454919e`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 284.9 KB (284887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbbb7b34bc324d050e49d3dd31294bdde5d6ecda33decf9afe31c11165b138a`  
		Last Modified: Tue, 10 Oct 2023 18:55:32 GMT  
		Size: 65.8 MB (65770135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c022f45a9fb1e7649eb4a663acd4ed6437363b4fc6e56f6af3e5f457a5d06ee8`  
		Last Modified: Tue, 10 Oct 2023 18:55:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12bec1760d3cf2773adbb14bd47431e46e130a914a46535c9a70de28e4b363b`  
		Last Modified: Sat, 21 Oct 2023 00:07:30 GMT  
		Size: 5.0 MB (4964316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888b304960048015ef929fcb0ffab750c1ba463aaf1d419272f2233e67195d56`  
		Last Modified: Sat, 21 Oct 2023 00:07:30 GMT  
		Size: 1.2 MB (1248665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00237a85b25c3b9ee3968fe9e98da8f378a4a70ccc746a6524820916085348ef`  
		Last Modified: Sat, 21 Oct 2023 00:07:29 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9275f10d0ef0db0999dc5ed6b19c068a941f59a05d69fad4b3cb07c3f0b14a7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74714658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b10f4fd814dc9e97d1147715baacffedd007b23ec081f4c100520df02050e6c9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:07:30 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 15:58:50 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:58:50 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 15:59:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 15:59:08 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 15:59:08 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 15:59:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:59:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 15:59:09 GMT
WORKDIR /go
# Wed, 01 Nov 2023 21:17:21 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 21:17:22 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 21:17:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 21:17:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 21:17:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8457acc181d300b4231b44e12aa0bf4a99ced5d51c5dfdc14eb899a341d5b855`  
		Last Modified: Sat, 21 Oct 2023 01:07:42 GMT  
		Size: 284.1 KB (284074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05626b790821d279bd9aea8466a1a79307764cbc389c51ab081a4b98c7657dc2`  
		Last Modified: Wed, 01 Nov 2023 16:06:11 GMT  
		Size: 65.8 MB (65772806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2dba3cbff62191bbc046c664eead34e3af26adfa5ecdbacf0ba6e73b9cbe51`  
		Last Modified: Wed, 01 Nov 2023 16:05:56 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357de4175525102c1d6c8d4fc605461ca1b1791b2a3b6c55c73e3ef6266159ad`  
		Last Modified: Wed, 01 Nov 2023 21:17:50 GMT  
		Size: 4.5 MB (4511226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59aa4bdeb70fa8c96a09911a5e79184a493cb38488e04d22007af9f9164e4f44`  
		Last Modified: Wed, 01 Nov 2023 21:17:50 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7b450bb18e60383a1dd8c51f37de16c5782ba7eba9e2737540247f3a4394c8`  
		Last Modified: Wed, 01 Nov 2023 21:17:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:76d3844fa9c17929397bb168745241a1f8fa36bf63c437d9d255fe217ec6a87c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73995976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6b4383d952151327974f3f21fa7be1e862f9a67c4ee08a264948e4372890be6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 02:41:07 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 15:36:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:36:13 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 15:36:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 15:36:23 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 15:36:23 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 15:36:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:36:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 15:36:24 GMT
WORKDIR /go
# Wed, 01 Nov 2023 19:56:22 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 19:56:22 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 19:56:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 19:56:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 19:56:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74bf0db6f91dfe1899e8204affb86f8c505a5643bdcb83b085888c86e0c7411`  
		Last Modified: Sat, 21 Oct 2023 02:41:18 GMT  
		Size: 286.3 KB (286297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd442d12e388d3f44ee4325caf9e959ca82d4064c8b1b38321da75a84a6ccbd`  
		Last Modified: Wed, 01 Nov 2023 15:41:04 GMT  
		Size: 64.1 MB (64110459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0297817440f5024a6c0e27f7906a375aa91aea5aaf191caa3f1762426e60e9c2`  
		Last Modified: Wed, 01 Nov 2023 15:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9fb63180b1c62b2cfd436428dc31a25bc97989024e217b9d8e508e82b0b287`  
		Last Modified: Wed, 01 Nov 2023 19:56:42 GMT  
		Size: 5.1 MB (5068382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0ee6df11f2e2e143f36f30697c4b309c4560fa062faa2fcb3a1c22db91257e`  
		Last Modified: Wed, 01 Nov 2023 19:56:42 GMT  
		Size: 1.2 MB (1198448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15b8268dd8cba7445da5d02c68c6787ce774d7ecc7dba9fa3f2775a88884d64`  
		Last Modified: Wed, 01 Nov 2023 19:56:41 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:ed1e2679ee802b3a2c8f7b42d4828ecc9ba50b5a029e3d14bbc54fa2a0fc5444
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74214117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2041e14adf1ce1c2b331135049ec2871be632eb2a7130142af035fa662cb1e19`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:13:11 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:13:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:17:44 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:18:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 19:18:14 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:18:14 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:18:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:18:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:18:17 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:09:16 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:09:17 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:09:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:09:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:09:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc67971d1767eae5019ffeaf8f893e6d81dbba50bde347da0c0433c56e3f2a3`  
		Last Modified: Thu, 28 Sep 2023 22:18:17 GMT  
		Size: 286.7 KB (286659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1caf7fa003bdf7c7611eb2e33a11db077a0f632b70d28f5b73096bf051f25aeb`  
		Last Modified: Tue, 10 Oct 2023 19:28:09 GMT  
		Size: 64.1 MB (64125245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9573c5aef56335266ce720d0812f9a0156f628fbd01ba4a6462be56d8742dc8a`  
		Last Modified: Tue, 10 Oct 2023 19:27:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40b483d55ec27555b481cb0fad97faf6e8d1686165905df945c86967ec0ac96`  
		Last Modified: Sat, 21 Oct 2023 00:09:50 GMT  
		Size: 5.3 MB (5268969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966ad11dd0f3a17ae3666a37f54fd9d6265bc0e18133314a565abf1039e90a1f`  
		Last Modified: Sat, 21 Oct 2023 00:09:50 GMT  
		Size: 1.2 MB (1186175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e18b62f88891e2a1b8f7a5e8a66e6ee69c9f42fe03945d66da418c55d339a9`  
		Last Modified: Sat, 21 Oct 2023 00:09:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:02d085e00e424e29b1a4c45b6358c9ac90629ed72540af87be474238770f3217
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76112263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fa19320a45d01205e0025f17edf0aa856b433bd25ee512a7877ec407bdf0a3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:44:44 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 12:29:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 12:29:18 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 12:29:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 12:29:51 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 12:29:52 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 12:29:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 12:29:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 12:29:54 GMT
WORKDIR /go
# Wed, 01 Nov 2023 16:51:53 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 16:51:55 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 16:51:56 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 16:51:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 16:51:57 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 16:51:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 16:52:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 16:52:01 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f15a4d38dd3d4f044868149900a763ac233f1aef33fe18019f45149b6bd02c`  
		Last Modified: Sat, 21 Oct 2023 00:45:00 GMT  
		Size: 285.1 KB (285095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23831500ce8c52e3d80c9eab9eb44d36e8daf00224a75f36d961186e47851ae8`  
		Last Modified: Wed, 01 Nov 2023 12:38:38 GMT  
		Size: 66.2 MB (66234435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92c933a1dfb2cbb65a33ccba713aabb9ff92ce6a0286e12af67e54c51be8a44`  
		Last Modified: Wed, 01 Nov 2023 12:38:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368a8f32c470e61e32632b0c78836e09dc1d70ab0e9a48e1c2bef1d23de82f7d`  
		Last Modified: Wed, 01 Nov 2023 16:52:34 GMT  
		Size: 5.1 MB (5114679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b61d54a31e32a9c971c8d7ea514537dababa89a4e60ce97eca5bdcf4e8d007`  
		Last Modified: Wed, 01 Nov 2023 16:52:33 GMT  
		Size: 1.3 MB (1262390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147c37f0535cd57e5355158d43aa5608a1430f56aa08ef1b4eb9cea12976a728`  
		Last Modified: Wed, 01 Nov 2023 16:52:33 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.4974; amd64

```console
$ docker pull caddy@sha256:951876270030a4a5404a8bab425d35b64f90babc594bb65c261cc05eab33ed79
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2128478401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:883908294a37d78f29e796d389d42c83a12c68a6c0f1113bba3bdd9290db5b05`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 02:23:09 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Oct 2023 02:23:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Oct 2023 02:23:11 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Oct 2023 02:23:12 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Oct 2023 02:24:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:24:31 GMT
ENV GOPATH=C:\go
# Wed, 11 Oct 2023 02:25:33 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Oct 2023 02:25:34 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 11 Oct 2023 02:28:30 GMT
RUN $url = 'https://dl.google.com/go/go1.21.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '27c8daf157493f288d42a6f38debc6a2cb391f6543139eba9152fceca0be2a10'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:28:31 GMT
WORKDIR C:\go
# Wed, 11 Oct 2023 04:03:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:03:14 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 12 Oct 2023 01:42:14 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:42:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 12 Oct 2023 01:43:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 12 Oct 2023 01:43:13 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fded5ce3c59d7e8d637a5536d6eed085ff6b6a323f42c1df76a7be6e9970ee`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a72a6b595ab9f8f71a34a065e75e609b20ea5e026f901820fce6d3c9134939`  
		Last Modified: Wed, 11 Oct 2023 02:46:39 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2574f8b7fb0ec5a8c39ee40a8008f0d24c398380247bf7140be1abdede5542b`  
		Last Modified: Wed, 11 Oct 2023 02:46:40 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951c53676fe729ebf5d3c07215d91afa952e6190715f79a7952f4c3aa121231e`  
		Last Modified: Wed, 11 Oct 2023 02:46:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a382bb149b70b82f9c2f58ebf6a2672dc4c64460017836d73a5a23b7379ea095`  
		Last Modified: Wed, 11 Oct 2023 02:46:44 GMT  
		Size: 25.6 MB (25557568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608a2584f4b3b8f3038fa41c0719005822ab967d85d1231843bd729a7b3d2d60`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1058e02ad62f976d823e3035f0578b2868eb09f28986153342a52014cc5c3810`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 284.8 KB (284754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fce039c31b2e60b62a0ede9974b6574519f2e47e1d8f4e09c7a1f30763aee95`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65449f183261f9bbdb731d41f5e6fca94f3e547e8d996133e418773400cfcfe`  
		Last Modified: Wed, 11 Oct 2023 02:46:59 GMT  
		Size: 69.3 MB (69345382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394e07c2ad53e950c47ffb647836822197dc5f8ebe082eaa045854e2b25bafc7`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993f5e59c63ef5be894fc498ab0e165faa3129d35a8a8f5173f12c6a4232f588`  
		Last Modified: Wed, 11 Oct 2023 04:06:31 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c675831130735b443a544dff1b9c188928f34947a5342350ef04eadc0d1ab27`  
		Last Modified: Wed, 11 Oct 2023 04:06:28 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69fe7c1d1f5383a4421f2a0e7284e17db440ee5b7be9f487ce9048f76970e7b6`  
		Last Modified: Thu, 12 Oct 2023 01:45:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee998763c3cef90b11adda3322e66e1a89d89409d1ed29dd73a4101fb657e29`  
		Last Modified: Thu, 12 Oct 2023 01:45:21 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196a81b981d5dc89b19acce594b87914fc5bc4777e42b1322ca9b9d4c4b4f179`  
		Last Modified: Thu, 12 Oct 2023 01:45:22 GMT  
		Size: 1.7 MB (1682335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3ad6e4e7b1be08f8a79e4d77328648deded93f9ef0d4a1e8202ce4c3a21c67`  
		Last Modified: Thu, 12 Oct 2023 01:45:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.20348.2031; amd64

```console
$ docker pull caddy@sha256:04b6c1b2519c8d35d65976c53b4523d7074d53c7b98fa5b29b83c837e021b493
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1956648108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6c3e402a7640df51573fae3237803e1e5fabce3d4c88849d9513c716654d474`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 02:19:41 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Oct 2023 02:19:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Oct 2023 02:19:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Oct 2023 02:19:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Oct 2023 02:20:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:20:18 GMT
ENV GOPATH=C:\go
# Wed, 11 Oct 2023 02:20:42 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Oct 2023 02:20:42 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 11 Oct 2023 02:22:59 GMT
RUN $url = 'https://dl.google.com/go/go1.21.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '27c8daf157493f288d42a6f38debc6a2cb391f6543139eba9152fceca0be2a10'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:23:01 GMT
WORKDIR C:\go
# Wed, 11 Oct 2023 04:04:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:04:42 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 12 Oct 2023 01:43:30 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:43:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 12 Oct 2023 01:43:51 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 12 Oct 2023 01:43:52 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60407a49ce6121c65fa6399c333c5227a09518414fd987c460ea29cb441ac5a`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe632e8cddda4e5f347720b87b8b3868e2e2969048761e3b0a40799d33f5f7a`  
		Last Modified: Wed, 11 Oct 2023 02:45:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4384696fc834e9658e7b3e5d1ceb1f8b362db85865daf29521b3c75c6999c046`  
		Last Modified: Wed, 11 Oct 2023 02:45:04 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c794ea611ef69f54d577f90b68e165e40a17e43b6d1d08f59951a38e084ea5fb`  
		Last Modified: Wed, 11 Oct 2023 02:45:03 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c74dc2d701da2bfabc4d44e6a4e6b92912515e2ca1fb053ffcc6b0d5cae2972`  
		Last Modified: Wed, 11 Oct 2023 02:45:08 GMT  
		Size: 25.5 MB (25531724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91612399ba7df8de0a05ad078c3817548f0a3b44516b76565e14a96ea62452e9`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7439c7c4353d2432c780827e4926910b19e84fe436d58e0a8129de2f631bd2b8`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 264.4 KB (264384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b0eaedd98e739ace4b7934261c71292195e461adcc977d02e57604d4a42ee8`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f46e84d4d007a200b1d6e7cb5b48db90116cdeb8bd3ec3964a08191875973e2`  
		Last Modified: Wed, 11 Oct 2023 02:45:25 GMT  
		Size: 69.3 MB (69325670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f59bab6d84ca44bbb60474dcf59c9af4f0f15edbdd64249b0eeaf968aff211f`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.6 KB (1556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f449f4d34d707dbde9cbb245c154c0b2e1d1a2c55d172501f8d7da576866f76f`  
		Last Modified: Wed, 11 Oct 2023 04:06:49 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a2edf76facdd17af03954b607484f7f7b36164a30634d19dd96b7320feb6b5`  
		Last Modified: Wed, 11 Oct 2023 04:06:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802c3686d509915fea71538d2c40c7a48c71719fab6144cb4497b6118b276ab9`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99cb183ed6cdad781eaba7bd1b4cb443befd9042c8a59450ee41f0245dd0ece4`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec33434b55fade6bcd7f3f0dfc10c981de93dc44bbae2b8702fdb6418a37a65b`  
		Last Modified: Thu, 12 Oct 2023 01:45:38 GMT  
		Size: 1.7 MB (1664788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0833369ef8236fcf99aba2d1fa48788db07662d0a9885a8429d435bf9f2227b2`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:0b6ab47c59512267b3021fcb39af41d2896fd78718a39fa127cc8f2a4795638e
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
$ docker pull caddy@sha256:d1f6d3dcfec129b4d0e23b6743f576807352958232a7ac6c17ee36f785fe5c58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76972374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e113a57232410dd987d12708b35062e6a269825fa7b4d03aef42c00acc93dce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:54:30 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:54:31 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:20:11 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:20:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 19:20:22 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:20:22 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:20:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:20:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:20:23 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:11:20 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:11:20 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:11:20 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:11:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:11:21 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:11:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:11:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:11:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc37b24bb09971feb8bf4882e861bce9db0c985a16a900adb0dc9de3f854243b`  
		Last Modified: Thu, 28 Sep 2023 22:57:15 GMT  
		Size: 284.7 KB (284690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a4303e95078c253686dcc16d7717644af63809efcbd753c0a999c9aad3fe72`  
		Last Modified: Tue, 10 Oct 2023 19:26:17 GMT  
		Size: 67.0 MB (67012876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359925be0f358b952dc8be63647139c5aab0fff94f7a070d88cb51dd258f80e5`  
		Last Modified: Tue, 10 Oct 2023 19:26:06 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958092cb44d28ddde181d193284001b1146b33a1cf19624e9683fc8f31551043`  
		Last Modified: Sat, 21 Oct 2023 00:11:52 GMT  
		Size: 5.0 MB (4970044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85cdb072dd78dcf6a7b04409cf7c8dc1fddddf912b601b15c6dc94adb2df10b`  
		Last Modified: Sat, 21 Oct 2023 00:11:51 GMT  
		Size: 1.3 MB (1302237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32749367842b0c8b40e7f61a315ff21b4d42211b5399e648beb75d86acb29c4c`  
		Last Modified: Sat, 21 Oct 2023 00:11:51 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:15f0db6d62062758441d2d22fd178c42299cf148c5097ffe10468153ff40c6b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75413855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:509cf858d9f3ffa4a94fe988705864c41bd510f34ade4ece0d2ede4cda23599f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 21:55:22 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 21:55:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 18:49:21 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 18:49:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 18:49:42 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 18:49:42 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 18:49:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 18:49:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 18:49:43 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:06:57 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:06:57 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:06:58 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:06:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:06:58 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:06:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:06:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:06:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3da3b9e7a12f6bb6b7f56e9240c2c92ce8c9f5fd5ef3b3063b9a93d454919e`  
		Last Modified: Thu, 28 Sep 2023 21:58:05 GMT  
		Size: 284.9 KB (284887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbbb7b34bc324d050e49d3dd31294bdde5d6ecda33decf9afe31c11165b138a`  
		Last Modified: Tue, 10 Oct 2023 18:55:32 GMT  
		Size: 65.8 MB (65770135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c022f45a9fb1e7649eb4a663acd4ed6437363b4fc6e56f6af3e5f457a5d06ee8`  
		Last Modified: Tue, 10 Oct 2023 18:55:13 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12bec1760d3cf2773adbb14bd47431e46e130a914a46535c9a70de28e4b363b`  
		Last Modified: Sat, 21 Oct 2023 00:07:30 GMT  
		Size: 5.0 MB (4964316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888b304960048015ef929fcb0ffab750c1ba463aaf1d419272f2233e67195d56`  
		Last Modified: Sat, 21 Oct 2023 00:07:30 GMT  
		Size: 1.2 MB (1248665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00237a85b25c3b9ee3968fe9e98da8f378a4a70ccc746a6524820916085348ef`  
		Last Modified: Sat, 21 Oct 2023 00:07:29 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9275f10d0ef0db0999dc5ed6b19c068a941f59a05d69fad4b3cb07c3f0b14a7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74714658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b10f4fd814dc9e97d1147715baacffedd007b23ec081f4c100520df02050e6c9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:07:30 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 15:58:50 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:58:50 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 15:59:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 15:59:08 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 15:59:08 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 15:59:08 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:59:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 15:59:09 GMT
WORKDIR /go
# Wed, 01 Nov 2023 21:17:21 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 21:17:22 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 21:17:22 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 21:17:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 21:17:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 21:17:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8457acc181d300b4231b44e12aa0bf4a99ced5d51c5dfdc14eb899a341d5b855`  
		Last Modified: Sat, 21 Oct 2023 01:07:42 GMT  
		Size: 284.1 KB (284074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05626b790821d279bd9aea8466a1a79307764cbc389c51ab081a4b98c7657dc2`  
		Last Modified: Wed, 01 Nov 2023 16:06:11 GMT  
		Size: 65.8 MB (65772806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2dba3cbff62191bbc046c664eead34e3af26adfa5ecdbacf0ba6e73b9cbe51`  
		Last Modified: Wed, 01 Nov 2023 16:05:56 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357de4175525102c1d6c8d4fc605461ca1b1791b2a3b6c55c73e3ef6266159ad`  
		Last Modified: Wed, 01 Nov 2023 21:17:50 GMT  
		Size: 4.5 MB (4511226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59aa4bdeb70fa8c96a09911a5e79184a493cb38488e04d22007af9f9164e4f44`  
		Last Modified: Wed, 01 Nov 2023 21:17:50 GMT  
		Size: 1.2 MB (1246086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7b450bb18e60383a1dd8c51f37de16c5782ba7eba9e2737540247f3a4394c8`  
		Last Modified: Wed, 01 Nov 2023 21:17:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:76d3844fa9c17929397bb168745241a1f8fa36bf63c437d9d255fe217ec6a87c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73995976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6b4383d952151327974f3f21fa7be1e862f9a67c4ee08a264948e4372890be6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 02:41:07 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 15:36:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:36:13 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 15:36:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 15:36:23 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 15:36:23 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 15:36:23 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 15:36:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 15:36:24 GMT
WORKDIR /go
# Wed, 01 Nov 2023 19:56:22 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 19:56:22 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 19:56:22 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 19:56:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 19:56:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 19:56:23 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74bf0db6f91dfe1899e8204affb86f8c505a5643bdcb83b085888c86e0c7411`  
		Last Modified: Sat, 21 Oct 2023 02:41:18 GMT  
		Size: 286.3 KB (286297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd442d12e388d3f44ee4325caf9e959ca82d4064c8b1b38321da75a84a6ccbd`  
		Last Modified: Wed, 01 Nov 2023 15:41:04 GMT  
		Size: 64.1 MB (64110459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0297817440f5024a6c0e27f7906a375aa91aea5aaf191caa3f1762426e60e9c2`  
		Last Modified: Wed, 01 Nov 2023 15:40:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9fb63180b1c62b2cfd436428dc31a25bc97989024e217b9d8e508e82b0b287`  
		Last Modified: Wed, 01 Nov 2023 19:56:42 GMT  
		Size: 5.1 MB (5068382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0ee6df11f2e2e143f36f30697c4b309c4560fa062faa2fcb3a1c22db91257e`  
		Last Modified: Wed, 01 Nov 2023 19:56:42 GMT  
		Size: 1.2 MB (1198448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15b8268dd8cba7445da5d02c68c6787ce774d7ecc7dba9fa3f2775a88884d64`  
		Last Modified: Wed, 01 Nov 2023 19:56:41 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:ed1e2679ee802b3a2c8f7b42d4828ecc9ba50b5a029e3d14bbc54fa2a0fc5444
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74214117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2041e14adf1ce1c2b331135049ec2871be632eb2a7130142af035fa662cb1e19`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:13:11 GMT
RUN apk add --no-cache ca-certificates
# Thu, 28 Sep 2023 22:13:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:17:44 GMT
ENV GOLANG_VERSION=1.21.3
# Tue, 10 Oct 2023 19:18:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Oct 2023 19:18:14 GMT
ENV GOTOOLCHAIN=local
# Tue, 10 Oct 2023 19:18:14 GMT
ENV GOPATH=/go
# Tue, 10 Oct 2023 19:18:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 19:18:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 10 Oct 2023 19:18:17 GMT
WORKDIR /go
# Sat, 21 Oct 2023 00:09:16 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_VERSION=v0.3.5
# Sat, 21 Oct 2023 00:09:17 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Sat, 21 Oct 2023 00:09:17 GMT
ENV XCADDY_SETCAP=1
# Sat, 21 Oct 2023 00:09:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Sat, 21 Oct 2023 00:09:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Sat, 21 Oct 2023 00:09:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc67971d1767eae5019ffeaf8f893e6d81dbba50bde347da0c0433c56e3f2a3`  
		Last Modified: Thu, 28 Sep 2023 22:18:17 GMT  
		Size: 286.7 KB (286659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1caf7fa003bdf7c7611eb2e33a11db077a0f632b70d28f5b73096bf051f25aeb`  
		Last Modified: Tue, 10 Oct 2023 19:28:09 GMT  
		Size: 64.1 MB (64125245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9573c5aef56335266ce720d0812f9a0156f628fbd01ba4a6462be56d8742dc8a`  
		Last Modified: Tue, 10 Oct 2023 19:27:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40b483d55ec27555b481cb0fad97faf6e8d1686165905df945c86967ec0ac96`  
		Last Modified: Sat, 21 Oct 2023 00:09:50 GMT  
		Size: 5.3 MB (5268969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966ad11dd0f3a17ae3666a37f54fd9d6265bc0e18133314a565abf1039e90a1f`  
		Last Modified: Sat, 21 Oct 2023 00:09:50 GMT  
		Size: 1.2 MB (1186175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e18b62f88891e2a1b8f7a5e8a66e6ee69c9f42fe03945d66da418c55d339a9`  
		Last Modified: Sat, 21 Oct 2023 00:09:49 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:02d085e00e424e29b1a4c45b6358c9ac90629ed72540af87be474238770f3217
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76112263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fa19320a45d01205e0025f17edf0aa856b433bd25ee512a7877ec407bdf0a3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:44:44 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 12:29:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 12:29:18 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 01 Nov 2023 12:29:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.3.linux-amd64.tar.gz'; 			sha256='1241381b2843fae5a9707eec1f8fb2ef94d827990582c7c7c32f5bdfbfd420c8'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.3.linux-armv6l.tar.gz'; 			sha256='a1ddcaaf0821a12a800884c14cb4268ce1c1f5a0301e9060646f1e15e611c6c7'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.3.linux-arm64.tar.gz'; 			sha256='fc90fa48ae97ba6368eecb914343590bbb61b388089510d0c56c2dde52987ef3'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.3.linux-386.tar.gz'; 			sha256='fb209fd070db500a84291c5a95251cceeb1723e8f6142de9baca5af70a927c0e'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.3.linux-ppc64le.tar.gz'; 			sha256='3b0e10a3704f164a6e85e0377728ec5fd21524fabe4c925610e34076586d5826'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.3.linux-riscv64.tar.gz'; 			sha256='67d14d3e513e505d1ec3ea34b55641c6c29556603c7899af94045c170c1c0f94'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.3.linux-s390x.tar.gz'; 			sha256='4c78e2e6f4c684a3d5a9bdc97202729053f44eb7be188206f0627ef3e18716b6'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.3.src.tar.gz'; 		sha256='186f2b6f8c8b704e696821b09ab2041a5c1ee13dcbc3156a13adcf75931ee488'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 01 Nov 2023 12:29:51 GMT
ENV GOTOOLCHAIN=local
# Wed, 01 Nov 2023 12:29:52 GMT
ENV GOPATH=/go
# Wed, 01 Nov 2023 12:29:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 12:29:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 01 Nov 2023 12:29:54 GMT
WORKDIR /go
# Wed, 01 Nov 2023 16:51:53 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 01 Nov 2023 16:51:55 GMT
ENV XCADDY_VERSION=v0.3.5
# Wed, 01 Nov 2023 16:51:56 GMT
ENV CADDY_VERSION=v2.7.5
# Wed, 01 Nov 2023 16:51:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 01 Nov 2023 16:51:57 GMT
ENV XCADDY_SETCAP=1
# Wed, 01 Nov 2023 16:51:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 01 Nov 2023 16:52:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 01 Nov 2023 16:52:01 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f15a4d38dd3d4f044868149900a763ac233f1aef33fe18019f45149b6bd02c`  
		Last Modified: Sat, 21 Oct 2023 00:45:00 GMT  
		Size: 285.1 KB (285095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23831500ce8c52e3d80c9eab9eb44d36e8daf00224a75f36d961186e47851ae8`  
		Last Modified: Wed, 01 Nov 2023 12:38:38 GMT  
		Size: 66.2 MB (66234435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92c933a1dfb2cbb65a33ccba713aabb9ff92ce6a0286e12af67e54c51be8a44`  
		Last Modified: Wed, 01 Nov 2023 12:38:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368a8f32c470e61e32632b0c78836e09dc1d70ab0e9a48e1c2bef1d23de82f7d`  
		Last Modified: Wed, 01 Nov 2023 16:52:34 GMT  
		Size: 5.1 MB (5114679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b61d54a31e32a9c971c8d7ea514537dababa89a4e60ce97eca5bdcf4e8d007`  
		Last Modified: Wed, 01 Nov 2023 16:52:33 GMT  
		Size: 1.3 MB (1262390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147c37f0535cd57e5355158d43aa5608a1430f56aa08ef1b4eb9cea12976a728`  
		Last Modified: Wed, 01 Nov 2023 16:52:33 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:c0740b75861440c921e23bec00c2ce3e14bda7ca7967b2aec7855352ea96cd0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull caddy@sha256:951876270030a4a5404a8bab425d35b64f90babc594bb65c261cc05eab33ed79
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2128478401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:883908294a37d78f29e796d389d42c83a12c68a6c0f1113bba3bdd9290db5b05`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 02:23:09 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Oct 2023 02:23:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Oct 2023 02:23:11 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Oct 2023 02:23:12 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Oct 2023 02:24:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:24:31 GMT
ENV GOPATH=C:\go
# Wed, 11 Oct 2023 02:25:33 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Oct 2023 02:25:34 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 11 Oct 2023 02:28:30 GMT
RUN $url = 'https://dl.google.com/go/go1.21.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '27c8daf157493f288d42a6f38debc6a2cb391f6543139eba9152fceca0be2a10'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:28:31 GMT
WORKDIR C:\go
# Wed, 11 Oct 2023 04:03:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:03:14 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 12 Oct 2023 01:42:14 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:42:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 12 Oct 2023 01:43:12 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 12 Oct 2023 01:43:13 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fded5ce3c59d7e8d637a5536d6eed085ff6b6a323f42c1df76a7be6e9970ee`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a72a6b595ab9f8f71a34a065e75e609b20ea5e026f901820fce6d3c9134939`  
		Last Modified: Wed, 11 Oct 2023 02:46:39 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2574f8b7fb0ec5a8c39ee40a8008f0d24c398380247bf7140be1abdede5542b`  
		Last Modified: Wed, 11 Oct 2023 02:46:40 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951c53676fe729ebf5d3c07215d91afa952e6190715f79a7952f4c3aa121231e`  
		Last Modified: Wed, 11 Oct 2023 02:46:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a382bb149b70b82f9c2f58ebf6a2672dc4c64460017836d73a5a23b7379ea095`  
		Last Modified: Wed, 11 Oct 2023 02:46:44 GMT  
		Size: 25.6 MB (25557568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608a2584f4b3b8f3038fa41c0719005822ab967d85d1231843bd729a7b3d2d60`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1058e02ad62f976d823e3035f0578b2868eb09f28986153342a52014cc5c3810`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 284.8 KB (284754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fce039c31b2e60b62a0ede9974b6574519f2e47e1d8f4e09c7a1f30763aee95`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65449f183261f9bbdb731d41f5e6fca94f3e547e8d996133e418773400cfcfe`  
		Last Modified: Wed, 11 Oct 2023 02:46:59 GMT  
		Size: 69.3 MB (69345382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394e07c2ad53e950c47ffb647836822197dc5f8ebe082eaa045854e2b25bafc7`  
		Last Modified: Wed, 11 Oct 2023 02:46:37 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993f5e59c63ef5be894fc498ab0e165faa3129d35a8a8f5173f12c6a4232f588`  
		Last Modified: Wed, 11 Oct 2023 04:06:31 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c675831130735b443a544dff1b9c188928f34947a5342350ef04eadc0d1ab27`  
		Last Modified: Wed, 11 Oct 2023 04:06:28 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69fe7c1d1f5383a4421f2a0e7284e17db440ee5b7be9f487ce9048f76970e7b6`  
		Last Modified: Thu, 12 Oct 2023 01:45:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee998763c3cef90b11adda3322e66e1a89d89409d1ed29dd73a4101fb657e29`  
		Last Modified: Thu, 12 Oct 2023 01:45:21 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196a81b981d5dc89b19acce594b87914fc5bc4777e42b1322ca9b9d4c4b4f179`  
		Last Modified: Thu, 12 Oct 2023 01:45:22 GMT  
		Size: 1.7 MB (1682335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3ad6e4e7b1be08f8a79e4d77328648deded93f9ef0d4a1e8202ce4c3a21c67`  
		Last Modified: Thu, 12 Oct 2023 01:45:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:7a4eaeb7416d6a4b442d55eab7e8c7824e36a07baef33353084b943d46b6b7b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `caddy:builder-windowsservercore-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull caddy@sha256:04b6c1b2519c8d35d65976c53b4523d7074d53c7b98fa5b29b83c837e021b493
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1956648108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6c3e402a7640df51573fae3237803e1e5fabce3d4c88849d9513c716654d474`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 02:19:41 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Oct 2023 02:19:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Oct 2023 02:19:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Oct 2023 02:19:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Oct 2023 02:20:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:20:18 GMT
ENV GOPATH=C:\go
# Wed, 11 Oct 2023 02:20:42 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Oct 2023 02:20:42 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 11 Oct 2023 02:22:59 GMT
RUN $url = 'https://dl.google.com/go/go1.21.3.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '27c8daf157493f288d42a6f38debc6a2cb391f6543139eba9152fceca0be2a10'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Oct 2023 02:23:01 GMT
WORKDIR C:\go
# Wed, 11 Oct 2023 04:04:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:04:42 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 12 Oct 2023 01:43:30 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:43:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 12 Oct 2023 01:43:51 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 12 Oct 2023 01:43:52 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60407a49ce6121c65fa6399c333c5227a09518414fd987c460ea29cb441ac5a`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe632e8cddda4e5f347720b87b8b3868e2e2969048761e3b0a40799d33f5f7a`  
		Last Modified: Wed, 11 Oct 2023 02:45:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4384696fc834e9658e7b3e5d1ceb1f8b362db85865daf29521b3c75c6999c046`  
		Last Modified: Wed, 11 Oct 2023 02:45:04 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c794ea611ef69f54d577f90b68e165e40a17e43b6d1d08f59951a38e084ea5fb`  
		Last Modified: Wed, 11 Oct 2023 02:45:03 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c74dc2d701da2bfabc4d44e6a4e6b92912515e2ca1fb053ffcc6b0d5cae2972`  
		Last Modified: Wed, 11 Oct 2023 02:45:08 GMT  
		Size: 25.5 MB (25531724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91612399ba7df8de0a05ad078c3817548f0a3b44516b76565e14a96ea62452e9`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7439c7c4353d2432c780827e4926910b19e84fe436d58e0a8129de2f631bd2b8`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 264.4 KB (264384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b0eaedd98e739ace4b7934261c71292195e461adcc977d02e57604d4a42ee8`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f46e84d4d007a200b1d6e7cb5b48db90116cdeb8bd3ec3964a08191875973e2`  
		Last Modified: Wed, 11 Oct 2023 02:45:25 GMT  
		Size: 69.3 MB (69325670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f59bab6d84ca44bbb60474dcf59c9af4f0f15edbdd64249b0eeaf968aff211f`  
		Last Modified: Wed, 11 Oct 2023 02:45:01 GMT  
		Size: 1.6 KB (1556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f449f4d34d707dbde9cbb245c154c0b2e1d1a2c55d172501f8d7da576866f76f`  
		Last Modified: Wed, 11 Oct 2023 04:06:49 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a2edf76facdd17af03954b607484f7f7b36164a30634d19dd96b7320feb6b5`  
		Last Modified: Wed, 11 Oct 2023 04:06:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802c3686d509915fea71538d2c40c7a48c71719fab6144cb4497b6118b276ab9`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99cb183ed6cdad781eaba7bd1b4cb443befd9042c8a59450ee41f0245dd0ece4`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec33434b55fade6bcd7f3f0dfc10c981de93dc44bbae2b8702fdb6418a37a65b`  
		Last Modified: Thu, 12 Oct 2023 01:45:38 GMT  
		Size: 1.7 MB (1664788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0833369ef8236fcf99aba2d1fa48788db07662d0a9885a8429d435bf9f2227b2`  
		Last Modified: Thu, 12 Oct 2023 01:45:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:325f81ca0328db0737503a53f43717fce79ea0c574e83f8e586c8d350cadf34b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4974; amd64
	-	windows version 10.0.20348.2031; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:a9c7585fdc50bb28d686b73a9b1f0eb9a3d103efd63c48dc334ccb5f51aa1722
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18474311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70c3913f54e294079c54cc8b651576b08dd4add42a0f4c0bc93d539913ae335d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:11:11 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:11:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:11:12 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:11:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:11:15 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:11:15 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:11:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:11:16 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:11:16 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:11:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5433daac73cddf3f03243a31c38d460570073f83e9a8cf64c7f0e3387b85807`  
		Last Modified: Sat, 21 Oct 2023 00:11:36 GMT  
		Size: 350.8 KB (350840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c6b4aafe2c09344f58425bb0fe037a429808edb7b2ba37d79cd35b2775a422`  
		Last Modified: Sat, 21 Oct 2023 00:11:36 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a182bff4e1b33f3d5dd80f809e697793466287c3da7704863c3d0b51d42b5b`  
		Last Modified: Sat, 21 Oct 2023 00:11:39 GMT  
		Size: 14.7 MB (14713998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:f43da8d65d754093117d4c673a7b725316be4e576e32b0d40c995e6ab1a07b7c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17422245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18b3bb2c3e0a97c9fe052eca67890f691907de7a5b514e88a44e660bb905079b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:06:46 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:06:48 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:06:48 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:06:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:06:51 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:06:51 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:06:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:06:52 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:06:52 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:06:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e09dc0459583a6ad3ba0428d5e180b7e3e6ae28360a69e293f03632cec397a0`  
		Last Modified: Sat, 21 Oct 2023 00:07:14 GMT  
		Size: 347.6 KB (347617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4705ff25da68d95a4bd671cbd4cec69369ea788be53bfafb45cdf4a930a725f8`  
		Last Modified: Sat, 21 Oct 2023 00:07:13 GMT  
		Size: 7.5 KB (7504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969c487cd333c7b53a7f57017e0ad77490d3806d9e52259caf9772016e96576d`  
		Last Modified: Sat, 21 Oct 2023 00:07:16 GMT  
		Size: 13.9 MB (13921833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:dd028bb08526d3533680243c94b9464c9c1a6559dccf5dde3b61ec73b9afd002
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17155303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:539aa551acc109f33c6ea5076a1f518af4d0476b517dc698d98c7350e8cb1b1a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:17:55 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:17:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:17:56 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:17:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:17:59 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:17:59 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:17:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:18:00 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:18:00 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:18:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee93e167fdbd8e67ec3f4ed8eaf242e5c8022a9845dd4f797448503af15d777c`  
		Last Modified: Sat, 21 Oct 2023 00:18:22 GMT  
		Size: 344.5 KB (344454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2895c0143aa41e87473191f749160d3109330cdb9de0c90a9b0a9e60e8a3a3e`  
		Last Modified: Sat, 21 Oct 2023 00:18:22 GMT  
		Size: 7.5 KB (7508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f015da3d3488ea9171b2970be40718bfa7e31496bae565a9bc2b677e53c09915`  
		Last Modified: Sat, 21 Oct 2023 00:18:25 GMT  
		Size: 13.9 MB (13903436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:d18ec23ab87841ede7ccefc353c20d1554faddf3ac362213c32ae22311136da5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17273763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cbdde935029392921ca3521ef9ebdb6a2b46cd1d4b7a9dabf0b71b00c593572`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:23:28 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:23:29 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:23:29 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:23:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:23:31 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:23:31 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:23:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:23:32 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:23:32 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:23:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461fe4f467fe88a160e176c442825b4bfea8dde13fc2324393a5d81518375e6f`  
		Last Modified: Sat, 21 Oct 2023 00:23:52 GMT  
		Size: 360.6 KB (360623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9335adc9ff07e38d963f0a71a2f7db01b5b5ed8e9d93fba14e584f25ea05c29d`  
		Last Modified: Sat, 21 Oct 2023 00:23:52 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32426666f5ec8621a07038733361be24f83719a812c0cce54e3f41192b31c2d`  
		Last Modified: Sat, 21 Oct 2023 00:23:54 GMT  
		Size: 13.6 MB (13573803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:1cd57ee42a4e84e91731e9182350ab4fd5b26705ec7286c28c5768c549435fd5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.1 MB (17057167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5aa3d5c5c63bea353c483de170ae8690a4f7eb12042cb84dc2bf0d52bf914b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:09:00 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:09:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:09:02 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:09:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:09:05 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:09:05 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:09:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:09:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:09:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:09:08 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:09:09 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:09:09 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:09:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692440f8f5ba2c6efbf2e74e3301377e3d9a90ae5a7cbd728c771ab306277830`  
		Last Modified: Sat, 21 Oct 2023 00:09:34 GMT  
		Size: 362.2 KB (362183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2886f5cbb210969eea27d97b8a48d88cae7bbe1bdd528a2b2775a8affde3084`  
		Last Modified: Sat, 21 Oct 2023 00:09:33 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdd6a19a7b9d3f4621c5388c53b0a9ea5591e9e72250bc60bcf22ed672632b1`  
		Last Modified: Sat, 21 Oct 2023 00:09:36 GMT  
		Size: 13.3 MB (13340969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:7dc6afd9bb40ff4450e4282bc56431b993d068c5b832c914dd50831189920061
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.8 MB (17822696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be3873facfc56aac0a1a9659efab4cddfc06afe6ac27c54cdd1b6fc9a23f1c1e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:05:23 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Sat, 21 Oct 2023 00:05:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Sat, 21 Oct 2023 00:05:24 GMT
ENV CADDY_VERSION=v2.7.5
# Sat, 21 Oct 2023 00:05:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 21 Oct 2023 00:05:27 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 21 Oct 2023 00:05:27 GMT
ENV XDG_DATA_HOME=/data
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 21 Oct 2023 00:05:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 21 Oct 2023 00:05:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 80
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 443
# Sat, 21 Oct 2023 00:05:28 GMT
EXPOSE 443/udp
# Sat, 21 Oct 2023 00:05:29 GMT
EXPOSE 2019
# Sat, 21 Oct 2023 00:05:29 GMT
WORKDIR /srv
# Sat, 21 Oct 2023 00:05:29 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d6d08cebdb83ff91ba335e0c4aec115b17261ed40307aaee6adde8c6763ad6`  
		Last Modified: Sat, 21 Oct 2023 00:06:00 GMT  
		Size: 355.0 KB (354963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58e0c7856c877cacd1d63a86beb12c9be91c4a0950dd85954db6f16a6d93103`  
		Last Modified: Sat, 21 Oct 2023 00:06:00 GMT  
		Size: 7.5 KB (7507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69bf19674eec620ff3f87ecb754c60b7c137eb6c8c3763ff795739061593a77`  
		Last Modified: Sat, 21 Oct 2023 00:06:02 GMT  
		Size: 14.2 MB (14245123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.4974; amd64

```console
$ docker pull caddy@sha256:77cb1b0b8315f376e69becef400d33c9d8b2a45548714845a821736158771de2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2047649951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3171dc2f25b4435520d8ba983ebf42f070ddec217b0da7677e309cc4cd51b05`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 03:59:19 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:39:06 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:40:04 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:40:05 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:40:06 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:40:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:40:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:40:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:40:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:40:12 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:40:13 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:41:01 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:41:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c4565a9b36858bc727874537e3c99968438a37e53c13057b0b1a233699d014`  
		Last Modified: Wed, 11 Oct 2023 04:05:44 GMT  
		Size: 472.0 KB (472034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df4a75108d3a33583e7ae61f1a019d4865860820bd89280ba414af94dd3f56e`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9dee9792a7bf7e1225840c56fb692536bee1743eba0a4da2faff34533f1160f`  
		Last Modified: Thu, 12 Oct 2023 01:44:37 GMT  
		Size: 15.3 MB (15296055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41900185a2519f01b8bd860f70936cee271612c4023512694b105826e0e0251`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0f1b69a12cd8550d868156e54168abaa32e1df40ee6eb39bc4e173ce04905e`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca266891343bff15b313846692ba3a41f313d5b228bedde964191332a16dffe`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12539eb7433a69ed67556d91b75b66dfedf0543d3efd7dabe82772437307a6f`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5103f279ed518bcfec88e00183e3222b50c1bc2f0e5b42f043e2198da424de98`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efc1cff2dac4308ce732a395ee215e1497d21f737e42e77917debf070afa8d7`  
		Last Modified: Thu, 12 Oct 2023 01:44:35 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cb50f59d2b11532a330925afb6ebd04d9b4708de8b11ae436e258c3764d741`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd11a311e4c0cf49bb544980f2c999751fc5e2fbe80d37b0f719f837abf8c3f`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ccbee9a6b9058ec933797dc1cfed875ceeb0115ce29ee163cd60a66e9f3b2d`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b486fc8ef055010a59374557443d3b713b9e55c1ccd11b7873f47876758976`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41df430d9a95c6000c922dd021b6cb2af0110dcc661ddc37a190a8cf6cd4bb06`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f243061a2e17d508efa4a424310d9ca158ca0cf0f59bd15cac606ab3e74701`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e709fff7d020a5d7c2d9e9e9a664c87392e9f9a4f4ced9802e64ca268995e23`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2c7aca9b511bc62340e6e8883d5f625bdccb805c4e897b837b68f3c79964b5`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38802c5a2b45b7029b250d88dac8209405146b0968925d1204cf17f7c3e76d98`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 269.1 KB (269086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376d19318a370d0da2ffcc29b47c2810278efa9d22fb39799c48687dfee0a2d9`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.20348.2031; amd64

```console
$ docker pull caddy@sha256:05f529a68927f0acfa7afbc79b7a19541f94430c137612ed344de7a822dcfafb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1875907229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8701a0e5aada270070acddeed89c57e20a5cac8afd88ed58da9557bf01dccb27`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:02:07 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:41:20 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:41:42 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:41:42 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:41:43 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:41:44 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:41:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:41:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:41:50 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:41:52 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:42:04 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:42:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c36616366b0df84f087a09bf19876f3872d839997f2f43e4eb8599861417c06`  
		Last Modified: Wed, 11 Oct 2023 04:06:10 GMT  
		Size: 467.9 KB (467933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db420ca589f10e4f9f5bc9dd6badc855d95c6a598888f2eb77a747eced259557`  
		Last Modified: Thu, 12 Oct 2023 01:45:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b5d7433dab05533d906a290a0f42cf31804c132da65c9fd7d4d2c41a64f519`  
		Last Modified: Thu, 12 Oct 2023 01:45:04 GMT  
		Size: 15.3 MB (15284209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62069fdf38bff9495ef2be05d397a55221536f9eec345734d6acec3a6196324f`  
		Last Modified: Thu, 12 Oct 2023 01:45:00 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e237a4c373c6937b5c51d0a3936152ac2b572fd5a432db3690f4070a7c78327`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73fae1c57e166a2ade87aa32e11980b456658212b296eea0f02ba3ec1c6557b`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000f2101dc464fa43321619c6e65c5b9e62b62755f3b141e69bd31892a253ded`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8536723423849b861a08fa490135f690c287be0144267e38fb3e631fb1bddbd2`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f176ef86531863755c3a315ec662b8da324474ae6097d7365dc18b76d61bde5`  
		Last Modified: Thu, 12 Oct 2023 01:44:58 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3973c168b3a63daa069e3a9870395561709d7b27762ffafb16538c773a16ad29`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5a10fbc59abc7ee7cc04a7ff48cc85983728745e91e8ef5fafee0589ba2193`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf033f8ab12414230e08aaada214c761777b0c784908ad2783ee31f8d330d0c9`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e2af83b2af59d76bd9b735c4e71b9492d9dbc120c042b8134ae0a70008f49`  
		Last Modified: Thu, 12 Oct 2023 01:44:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0355ed819405072f13996095ae7ec7044017bee81808dea9500459620118c20b`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e86117e27425829055f627e6156a4a657d9817cf8d2158f0026752366c9022c`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22fbe71be2fe08164a92f1362959f0a4aba194dcf931945d7bb2ac50e8f6467`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed768b9f807d51e5834f0bc8b2ea4dda09a5139d126f9141cb3db51f781ea541`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359fc3c79eda3ddbb39c46b09a4c68137a693a72f8712182d545c546b726027e`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 289.5 KB (289533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e4b8683a429393010114c6906acced22d65d5167cda2cc55238ae5b9f816c0`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:b859825f1b8093a4b961d02fb945e63f5180c5e07e56ce7495384835c016c47d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4974; amd64
	-	windows version 10.0.20348.2031; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.4974; amd64

```console
$ docker pull caddy@sha256:77cb1b0b8315f376e69becef400d33c9d8b2a45548714845a821736158771de2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2047649951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3171dc2f25b4435520d8ba983ebf42f070ddec217b0da7677e309cc4cd51b05`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 03:59:19 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:39:06 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:40:04 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:40:05 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:40:06 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:40:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:40:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:40:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:40:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:40:12 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:40:13 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:41:01 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:41:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c4565a9b36858bc727874537e3c99968438a37e53c13057b0b1a233699d014`  
		Last Modified: Wed, 11 Oct 2023 04:05:44 GMT  
		Size: 472.0 KB (472034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df4a75108d3a33583e7ae61f1a019d4865860820bd89280ba414af94dd3f56e`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9dee9792a7bf7e1225840c56fb692536bee1743eba0a4da2faff34533f1160f`  
		Last Modified: Thu, 12 Oct 2023 01:44:37 GMT  
		Size: 15.3 MB (15296055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41900185a2519f01b8bd860f70936cee271612c4023512694b105826e0e0251`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0f1b69a12cd8550d868156e54168abaa32e1df40ee6eb39bc4e173ce04905e`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca266891343bff15b313846692ba3a41f313d5b228bedde964191332a16dffe`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12539eb7433a69ed67556d91b75b66dfedf0543d3efd7dabe82772437307a6f`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5103f279ed518bcfec88e00183e3222b50c1bc2f0e5b42f043e2198da424de98`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efc1cff2dac4308ce732a395ee215e1497d21f737e42e77917debf070afa8d7`  
		Last Modified: Thu, 12 Oct 2023 01:44:35 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cb50f59d2b11532a330925afb6ebd04d9b4708de8b11ae436e258c3764d741`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd11a311e4c0cf49bb544980f2c999751fc5e2fbe80d37b0f719f837abf8c3f`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ccbee9a6b9058ec933797dc1cfed875ceeb0115ce29ee163cd60a66e9f3b2d`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b486fc8ef055010a59374557443d3b713b9e55c1ccd11b7873f47876758976`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41df430d9a95c6000c922dd021b6cb2af0110dcc661ddc37a190a8cf6cd4bb06`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f243061a2e17d508efa4a424310d9ca158ca0cf0f59bd15cac606ab3e74701`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e709fff7d020a5d7c2d9e9e9a664c87392e9f9a4f4ced9802e64ca268995e23`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2c7aca9b511bc62340e6e8883d5f625bdccb805c4e897b837b68f3c79964b5`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38802c5a2b45b7029b250d88dac8209405146b0968925d1204cf17f7c3e76d98`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 269.1 KB (269086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376d19318a370d0da2ffcc29b47c2810278efa9d22fb39799c48687dfee0a2d9`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.20348.2031; amd64

```console
$ docker pull caddy@sha256:05f529a68927f0acfa7afbc79b7a19541f94430c137612ed344de7a822dcfafb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1875907229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8701a0e5aada270070acddeed89c57e20a5cac8afd88ed58da9557bf01dccb27`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:02:07 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:41:20 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:41:42 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:41:42 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:41:43 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:41:44 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:41:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:41:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:41:50 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:41:52 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:42:04 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:42:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c36616366b0df84f087a09bf19876f3872d839997f2f43e4eb8599861417c06`  
		Last Modified: Wed, 11 Oct 2023 04:06:10 GMT  
		Size: 467.9 KB (467933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db420ca589f10e4f9f5bc9dd6badc855d95c6a598888f2eb77a747eced259557`  
		Last Modified: Thu, 12 Oct 2023 01:45:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b5d7433dab05533d906a290a0f42cf31804c132da65c9fd7d4d2c41a64f519`  
		Last Modified: Thu, 12 Oct 2023 01:45:04 GMT  
		Size: 15.3 MB (15284209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62069fdf38bff9495ef2be05d397a55221536f9eec345734d6acec3a6196324f`  
		Last Modified: Thu, 12 Oct 2023 01:45:00 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e237a4c373c6937b5c51d0a3936152ac2b572fd5a432db3690f4070a7c78327`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73fae1c57e166a2ade87aa32e11980b456658212b296eea0f02ba3ec1c6557b`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000f2101dc464fa43321619c6e65c5b9e62b62755f3b141e69bd31892a253ded`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8536723423849b861a08fa490135f690c287be0144267e38fb3e631fb1bddbd2`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f176ef86531863755c3a315ec662b8da324474ae6097d7365dc18b76d61bde5`  
		Last Modified: Thu, 12 Oct 2023 01:44:58 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3973c168b3a63daa069e3a9870395561709d7b27762ffafb16538c773a16ad29`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5a10fbc59abc7ee7cc04a7ff48cc85983728745e91e8ef5fafee0589ba2193`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf033f8ab12414230e08aaada214c761777b0c784908ad2783ee31f8d330d0c9`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e2af83b2af59d76bd9b735c4e71b9492d9dbc120c042b8134ae0a70008f49`  
		Last Modified: Thu, 12 Oct 2023 01:44:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0355ed819405072f13996095ae7ec7044017bee81808dea9500459620118c20b`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e86117e27425829055f627e6156a4a657d9817cf8d2158f0026752366c9022c`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22fbe71be2fe08164a92f1362959f0a4aba194dcf931945d7bb2ac50e8f6467`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed768b9f807d51e5834f0bc8b2ea4dda09a5139d126f9141cb3db51f781ea541`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359fc3c79eda3ddbb39c46b09a4c68137a693a72f8712182d545c546b726027e`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 289.5 KB (289533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e4b8683a429393010114c6906acced22d65d5167cda2cc55238ae5b9f816c0`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:8169d134dfa19ddbba9eeeb7210c5227c2a61f00906c340474aab1250aba47f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull caddy@sha256:77cb1b0b8315f376e69becef400d33c9d8b2a45548714845a821736158771de2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2047649951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3171dc2f25b4435520d8ba983ebf42f070ddec217b0da7677e309cc4cd51b05`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 03:59:19 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:39:06 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:40:04 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:40:05 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:40:06 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:40:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:40:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:40:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:40:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:40:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:40:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:40:12 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:40:13 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:40:14 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:41:01 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:41:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c4565a9b36858bc727874537e3c99968438a37e53c13057b0b1a233699d014`  
		Last Modified: Wed, 11 Oct 2023 04:05:44 GMT  
		Size: 472.0 KB (472034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df4a75108d3a33583e7ae61f1a019d4865860820bd89280ba414af94dd3f56e`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9dee9792a7bf7e1225840c56fb692536bee1743eba0a4da2faff34533f1160f`  
		Last Modified: Thu, 12 Oct 2023 01:44:37 GMT  
		Size: 15.3 MB (15296055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41900185a2519f01b8bd860f70936cee271612c4023512694b105826e0e0251`  
		Last Modified: Thu, 12 Oct 2023 01:44:34 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0f1b69a12cd8550d868156e54168abaa32e1df40ee6eb39bc4e173ce04905e`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca266891343bff15b313846692ba3a41f313d5b228bedde964191332a16dffe`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12539eb7433a69ed67556d91b75b66dfedf0543d3efd7dabe82772437307a6f`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5103f279ed518bcfec88e00183e3222b50c1bc2f0e5b42f043e2198da424de98`  
		Last Modified: Thu, 12 Oct 2023 01:44:32 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efc1cff2dac4308ce732a395ee215e1497d21f737e42e77917debf070afa8d7`  
		Last Modified: Thu, 12 Oct 2023 01:44:35 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cb50f59d2b11532a330925afb6ebd04d9b4708de8b11ae436e258c3764d741`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd11a311e4c0cf49bb544980f2c999751fc5e2fbe80d37b0f719f837abf8c3f`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ccbee9a6b9058ec933797dc1cfed875ceeb0115ce29ee163cd60a66e9f3b2d`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b486fc8ef055010a59374557443d3b713b9e55c1ccd11b7873f47876758976`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41df430d9a95c6000c922dd021b6cb2af0110dcc661ddc37a190a8cf6cd4bb06`  
		Last Modified: Thu, 12 Oct 2023 01:44:30 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f243061a2e17d508efa4a424310d9ca158ca0cf0f59bd15cac606ab3e74701`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e709fff7d020a5d7c2d9e9e9a664c87392e9f9a4f4ced9802e64ca268995e23`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2c7aca9b511bc62340e6e8883d5f625bdccb805c4e897b837b68f3c79964b5`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38802c5a2b45b7029b250d88dac8209405146b0968925d1204cf17f7c3e76d98`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 269.1 KB (269086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376d19318a370d0da2ffcc29b47c2810278efa9d22fb39799c48687dfee0a2d9`  
		Last Modified: Thu, 12 Oct 2023 01:44:28 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:278d32be7fb2f9a5e3f48ea6a672747dbb4ad6256e4802aff4a1e11a67e2e518
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `caddy:windowsservercore-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull caddy@sha256:05f529a68927f0acfa7afbc79b7a19541f94430c137612ed344de7a822dcfafb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1875907229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8701a0e5aada270070acddeed89c57e20a5cac8afd88ed58da9557bf01dccb27`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 04:02:07 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 12 Oct 2023 01:41:20 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 12 Oct 2023 01:41:42 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 12 Oct 2023 01:41:42 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 12 Oct 2023 01:41:43 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 12 Oct 2023 01:41:44 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 12 Oct 2023 01:41:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 12 Oct 2023 01:41:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 12 Oct 2023 01:41:47 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 12 Oct 2023 01:41:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 12 Oct 2023 01:41:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 12 Oct 2023 01:41:50 GMT
EXPOSE 80
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443
# Thu, 12 Oct 2023 01:41:51 GMT
EXPOSE 443/udp
# Thu, 12 Oct 2023 01:41:52 GMT
EXPOSE 2019
# Thu, 12 Oct 2023 01:42:04 GMT
RUN caddy version
# Thu, 12 Oct 2023 01:42:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c36616366b0df84f087a09bf19876f3872d839997f2f43e4eb8599861417c06`  
		Last Modified: Wed, 11 Oct 2023 04:06:10 GMT  
		Size: 467.9 KB (467933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db420ca589f10e4f9f5bc9dd6badc855d95c6a598888f2eb77a747eced259557`  
		Last Modified: Thu, 12 Oct 2023 01:45:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b5d7433dab05533d906a290a0f42cf31804c132da65c9fd7d4d2c41a64f519`  
		Last Modified: Thu, 12 Oct 2023 01:45:04 GMT  
		Size: 15.3 MB (15284209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62069fdf38bff9495ef2be05d397a55221536f9eec345734d6acec3a6196324f`  
		Last Modified: Thu, 12 Oct 2023 01:45:00 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e237a4c373c6937b5c51d0a3936152ac2b572fd5a432db3690f4070a7c78327`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73fae1c57e166a2ade87aa32e11980b456658212b296eea0f02ba3ec1c6557b`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000f2101dc464fa43321619c6e65c5b9e62b62755f3b141e69bd31892a253ded`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8536723423849b861a08fa490135f690c287be0144267e38fb3e631fb1bddbd2`  
		Last Modified: Thu, 12 Oct 2023 01:44:59 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f176ef86531863755c3a315ec662b8da324474ae6097d7365dc18b76d61bde5`  
		Last Modified: Thu, 12 Oct 2023 01:44:58 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3973c168b3a63daa069e3a9870395561709d7b27762ffafb16538c773a16ad29`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5a10fbc59abc7ee7cc04a7ff48cc85983728745e91e8ef5fafee0589ba2193`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf033f8ab12414230e08aaada214c761777b0c784908ad2783ee31f8d330d0c9`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e2af83b2af59d76bd9b735c4e71b9492d9dbc120c042b8134ae0a70008f49`  
		Last Modified: Thu, 12 Oct 2023 01:44:56 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0355ed819405072f13996095ae7ec7044017bee81808dea9500459620118c20b`  
		Last Modified: Thu, 12 Oct 2023 01:44:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e86117e27425829055f627e6156a4a657d9817cf8d2158f0026752366c9022c`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22fbe71be2fe08164a92f1362959f0a4aba194dcf931945d7bb2ac50e8f6467`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed768b9f807d51e5834f0bc8b2ea4dda09a5139d126f9141cb3db51f781ea541`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359fc3c79eda3ddbb39c46b09a4c68137a693a72f8712182d545c546b726027e`  
		Last Modified: Thu, 12 Oct 2023 01:44:55 GMT  
		Size: 289.5 KB (289533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e4b8683a429393010114c6906acced22d65d5167cda2cc55238ae5b9f816c0`  
		Last Modified: Thu, 12 Oct 2023 01:44:54 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
