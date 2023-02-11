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
-	[`caddy:2.6.3`](#caddy263)
-	[`caddy:2.6.3-alpine`](#caddy263-alpine)
-	[`caddy:2.6.3-builder`](#caddy263-builder)
-	[`caddy:2.6.3-builder-alpine`](#caddy263-builder-alpine)
-	[`caddy:2.6.3-builder-windowsservercore-1809`](#caddy263-builder-windowsservercore-1809)
-	[`caddy:2.6.3-builder-windowsservercore-ltsc2022`](#caddy263-builder-windowsservercore-ltsc2022)
-	[`caddy:2.6.3-windowsservercore`](#caddy263-windowsservercore)
-	[`caddy:2.6.3-windowsservercore-1809`](#caddy263-windowsservercore-1809)
-	[`caddy:2.6.3-windowsservercore-ltsc2022`](#caddy263-windowsservercore-ltsc2022)
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
$ docker pull caddy@sha256:d34a689107f831d1fb6dfb92ce4cff1569e409e5b6dcd2d671d4ffee8b112b76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3887; amd64
	-	windows version 10.0.20348.1487; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:cf66a65d5667b26ba91fab680b59d421266e5042d4191fcdeab3847b31828bf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17441779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:739163e8bd53961abf96cc4f327498332dd905a59d3314fab80a845e62b58f9b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Thu, 09 Feb 2023 03:18:05 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 09 Feb 2023 03:18:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 09 Feb 2023 03:18:06 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:18:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 09 Feb 2023 03:18:10 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 09 Feb 2023 03:18:10 GMT
ENV XDG_DATA_HOME=/data
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 80
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 443
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 03:18:11 GMT
WORKDIR /srv
# Thu, 09 Feb 2023 03:18:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4cf81513fab9758787dbde95dcab4c054bd04137581b68097595a719ae973c`  
		Last Modified: Thu, 09 Feb 2023 03:18:39 GMT  
		Size: 351.2 KB (351181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c3f44eb3bccaf2f5515331e12d4b940a5f6ad016d27f548e0c739d1f6aba66`  
		Last Modified: Thu, 09 Feb 2023 03:18:39 GMT  
		Size: 7.6 KB (7554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04314ed686e612bbb7606d6bacff938564f9b4f7e0dbc72afacd887b3c88afbd`  
		Last Modified: Thu, 09 Feb 2023 03:18:42 GMT  
		Size: 14.3 MB (14276772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e4444abb42ab384f9685f3b25765ed65d8e07daef954ccf7aa73a524a2177064
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16576623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99391525993d815548f2a8e80455bb1ff1b6dd0a769a0dc2a467cbcc3adbc1ad`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:32 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Fri, 10 Feb 2023 20:49:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:28:54 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 21:28:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Fri, 10 Feb 2023 21:28:56 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 21:28:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 21:28:59 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 21:28:59 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 80
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 443
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 21:29:00 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 21:29:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a400dcba29ff44f8e5bf01493def4f19629aca6d103cb2a66ca87c457f7414`  
		Last Modified: Fri, 10 Feb 2023 21:29:47 GMT  
		Size: 345.8 KB (345811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b946768825eb5ed2fc6f932fdb0b0c552f4c35c39dada07eddd70ce4a535953`  
		Last Modified: Fri, 10 Feb 2023 21:29:47 GMT  
		Size: 7.5 KB (7480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda323f820516b366c61a02ba4cfd00cc3a3b6cc9051c58e7359057dea842d8a`  
		Last Modified: Fri, 10 Feb 2023 21:29:51 GMT  
		Size: 13.6 MB (13606554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0a66f97fe167ebcccd1754f2cc7ed8d5f42595f332f60d75e4efd33c5fa880b9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16362110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0940efa30038d45d9b6cbae2aea1235accdd5e653948a6e40e9c3edf6314d4c6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:37:19 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:37:22 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Fri, 10 Feb 2023 22:37:22 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:37:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:37:26 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:37:27 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:37:27 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:37:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:37:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:37:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:37:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:37:30 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:37:30 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:37:31 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:37:31 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:37:31 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:37:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec2ab4edb1f0a14b28a55f050d62d8e54111075639a0fa8f173448814ba0d00`  
		Last Modified: Fri, 10 Feb 2023 22:38:25 GMT  
		Size: 342.6 KB (342588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0580184dd0082f009564a7a3923731f202cbe4bd8b857dbca2c77da8e7434815`  
		Last Modified: Fri, 10 Feb 2023 22:38:25 GMT  
		Size: 7.5 KB (7479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b2a44f2792add2104a1d53c68f1df95779deaee3ec86717f4fb4efd9aa6aaa`  
		Last Modified: Fri, 10 Feb 2023 22:38:28 GMT  
		Size: 13.6 MB (13591549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:4be5e6cdfb930681cc9c4722b0af67e75e53f0cff56c916c1d618eb39d6f5169
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16126925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:995c31e78c533c3ca73152cb87130dfcb16842dd052ab384df917fb755c5dc43`
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
# Fri, 10 Feb 2023 22:00:37 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:00:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:00:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:00:39 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:00:40 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:00:40 GMT
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
	-	`sha256:6403d7bb9250089f4077bba7631d975f97648fbcd782c992704ff3bccc5ae421`  
		Last Modified: Fri, 10 Feb 2023 22:01:03 GMT  
		Size: 13.1 MB (13059715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:50a289625f0ef1adfc05773b5ec8a30f001be347a84f24e1106e351f230758b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15949909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b11b3ee451004883e1f9089fc132ee1ecc849a2d96ef0ff4731334c8279cfa`
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
# Fri, 10 Feb 2023 22:13:23 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:13:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:13:28 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:13:28 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:13:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:13:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:13:33 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:13:33 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:13:33 GMT
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
	-	`sha256:2ecc7ec17344834a2337d83b9b7be44f97f0c0b55dfea5e1d8af80c8d5c32221`  
		Last Modified: Fri, 10 Feb 2023 22:14:19 GMT  
		Size: 12.8 MB (12774635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:9c69a670bfaa4e7166553c41a7303b114a524eed38924ad0d1d5599e6b7b2463
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16787086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9abb18c28ea7e824ff4385016f24b30d1a455d1b902f8667a1a9300078826a`
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
# Fri, 10 Feb 2023 22:14:19 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:14:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:14:21 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:14:22 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:14:23 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:14:23 GMT
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
	-	`sha256:94fd73a8831c9e57fdf8c430154c9adc56e54610a462128c8f0a1b3937aef704`  
		Last Modified: Fri, 10 Feb 2023 22:15:07 GMT  
		Size: 13.8 MB (13833147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.3887; amd64

```console
$ docker pull caddy@sha256:935d1f4349cc551dfe9b76d6ba5fe6355414519a3037a7689fe765033ae8dcd6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1723388621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1deb1aecac8501d9afe22abd2fc90f15552c63366f8016ad2e6d1602be5cdf6d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:16:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:16:36 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:17:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:17:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:17:21 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:17:22 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:17:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:17:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:17:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:17:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:17:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:17:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:17:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:17:31 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:17:32 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:17:33 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:17:34 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:17:53 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:17:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47af8a9c9ef8e49d65e53dd207ad0935ce7a2b50b2f253e6a5b037494ae19d0a`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 401.5 KB (401472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5841cb6343add9dd7b89906610425117976b050c0634eedbc5c38302aa024e`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d760049e5c9f1fb1d7ec05a3eea55088808f484912e87cda07f3709363fe3c2c`  
		Last Modified: Thu, 09 Feb 2023 01:16:53 GMT  
		Size: 14.7 MB (14680484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3239225b5bad52e6004b638bd356e7d29e7fded5d31d90541907e1a769a115`  
		Last Modified: Thu, 09 Feb 2023 01:16:49 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6823ad091829bc6d98a58a18b075e20c551bde81d504bdbfda09b5a3d7c5d0`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4873a8802163accb90dd2318bd05ddfa4f94692b2731d6e23095e3bb46b98fd`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabf39e152fd5c18e0c3ac503e054c36e2775512f9fa7bb11b9221442b2bc1fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af12dc4018ba87a8e25003874e2d8e959a25b1c19932553daec8f4c410ebd61f`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fefa1f82e39e2af863b13609d78d966746d852af0cea54dcb17f45a8386c39d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d5b41708aea61714f00bc0f35ea1efc60db85c04ab6754e4d6b4485dc59a28`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a8b1cf8bcc4175323f7feaa280e3122f03aa7f9d35666fcc55c6b7d1e628ae`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c3f865e552649c436d5ffc0f3c83a3b5ba3026b2cff2ab3f381a5cdf2e2f2`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201cfdbfc1583e2ea070418e6aad0ec6604fb52c68117460b1a4c5b511b56ecc`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef83199fb67566ea043dbf7fab6f54754a4d0496655be1157819973573247bb`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45db789a3d9786dea133341e2c9f16e14b23a664297ad7f9a371961a0c21588`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a4e021c112717a1fee7cd62cdc17d41521f3514f10bf8ec30457b95aaf44fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4c0327054bc1f199339822d4074ee176c4184b9357ec28d9250f27f0c12e26`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63a4d912695117a127068d20ceefbaa19e41c8a42d65788d37915d737d998d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:44 GMT  
		Size: 338.6 KB (338620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421719fbbf536a3651d6762e36406f19dd0b5601f4a300d9c47af9ccfa3573d2`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.20348.1487; amd64

```console
$ docker pull caddy@sha256:22cdfda624195707c05f1d681c1cdd97b504f06b282d981718e1b716b2dc6bfb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1401937005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca7c6af6ec202266d95f15726fee733430a631c6c4eddfd9cc7d000b817a0f19`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:18:43 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:18:44 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:19:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:19:16 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:19:17 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:19:18 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:19:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:19:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:19:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:19:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:19:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:19:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:19:26 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:19:27 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:19:29 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:19:30 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:19:47 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:19:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42eb48143612ee855d99c932e324b1bd035c60554117edeaa805402060613c51`  
		Last Modified: Thu, 09 Feb 2023 01:17:17 GMT  
		Size: 635.9 KB (635943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714ae92cb5dac0e72097d35b932125b5ea3f03214de78e03119a4517be6fd10`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a5533d3ddbff5ea35dbb0e11b10fe817ce3ef1a3fd7f44706cb1b6288e0406`  
		Last Modified: Thu, 09 Feb 2023 01:17:20 GMT  
		Size: 14.9 MB (14899830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e59c8f0dc8d987210bdfe89eaded536b0ef8ac727eb7d75b76aea9c296208a`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22bfc3588219a43ce294aab21751b407ae75504bf3ddcee69f42498672b6c46`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f7db57dc0a0b0126433f60d3d0005f9aaa0d405fe63cfc3b4e15388fdfa010`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7b9e3a2510b5ab3b7ac4103d653c8efd12e95b63327d5c5fb81b6ea341e2b5`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4109b3b0ca73b5355a12ee74b7c32b4015a6208fdb279fd0ab60074247e22309`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3c568a1866d44483984b2be40142a55371adf3b8dc991bdb5ab4c45c0be3d4`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6221c7c14444b318e798e231adeeb83ea155c157283e9def018c43415238aa7`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e81980463382095586f78276db5cd808400136543fc1a0f522af1f3eaee034`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f0d8afe85320b7cf4542ad649671660bbb8e74ec3ad3067408e79fb21dbf77`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7def0e2b3dd94a350c82bb6a4903fdfc65d1d3d9772dd8195a5eb14ba766c45`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0b51c8090bf08cc2ae3a9fc340c9b70ba1e077f32b7d7d025b7d9fb472d978`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3653016f515e293fc93892b9e021e05a6a183ad3dcdaf243311513e222534c7`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d1dafd3fbb7403b7f093ed63553863bd9904f6010b1b91f98d9bfba9c4d8bb`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92817327253aaae4d632a75ff38a01dbebfe11f9105c4db828c52f221262ce4`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43bce457643a143e82e49e57d9b8a69a416e254d2439f30d7e4dd25c84e43c0`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 348.1 KB (348138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a0e899ab4c995de79522a5022b8cca4765559a4de2d5c728821d947b497de1`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:7e7286bb77df853f278887dd9159bd643abca8447ad4a0fddb4c48ec00a7e6cc
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
$ docker pull caddy@sha256:cf66a65d5667b26ba91fab680b59d421266e5042d4191fcdeab3847b31828bf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17441779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:739163e8bd53961abf96cc4f327498332dd905a59d3314fab80a845e62b58f9b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Thu, 09 Feb 2023 03:18:05 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 09 Feb 2023 03:18:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 09 Feb 2023 03:18:06 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:18:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 09 Feb 2023 03:18:10 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 09 Feb 2023 03:18:10 GMT
ENV XDG_DATA_HOME=/data
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 80
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 443
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 03:18:11 GMT
WORKDIR /srv
# Thu, 09 Feb 2023 03:18:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4cf81513fab9758787dbde95dcab4c054bd04137581b68097595a719ae973c`  
		Last Modified: Thu, 09 Feb 2023 03:18:39 GMT  
		Size: 351.2 KB (351181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c3f44eb3bccaf2f5515331e12d4b940a5f6ad016d27f548e0c739d1f6aba66`  
		Last Modified: Thu, 09 Feb 2023 03:18:39 GMT  
		Size: 7.6 KB (7554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04314ed686e612bbb7606d6bacff938564f9b4f7e0dbc72afacd887b3c88afbd`  
		Last Modified: Thu, 09 Feb 2023 03:18:42 GMT  
		Size: 14.3 MB (14276772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e4444abb42ab384f9685f3b25765ed65d8e07daef954ccf7aa73a524a2177064
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16576623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99391525993d815548f2a8e80455bb1ff1b6dd0a769a0dc2a467cbcc3adbc1ad`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:32 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Fri, 10 Feb 2023 20:49:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:28:54 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 21:28:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Fri, 10 Feb 2023 21:28:56 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 21:28:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 21:28:59 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 21:28:59 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 80
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 443
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 21:29:00 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 21:29:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a400dcba29ff44f8e5bf01493def4f19629aca6d103cb2a66ca87c457f7414`  
		Last Modified: Fri, 10 Feb 2023 21:29:47 GMT  
		Size: 345.8 KB (345811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b946768825eb5ed2fc6f932fdb0b0c552f4c35c39dada07eddd70ce4a535953`  
		Last Modified: Fri, 10 Feb 2023 21:29:47 GMT  
		Size: 7.5 KB (7480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda323f820516b366c61a02ba4cfd00cc3a3b6cc9051c58e7359057dea842d8a`  
		Last Modified: Fri, 10 Feb 2023 21:29:51 GMT  
		Size: 13.6 MB (13606554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0a66f97fe167ebcccd1754f2cc7ed8d5f42595f332f60d75e4efd33c5fa880b9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16362110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0940efa30038d45d9b6cbae2aea1235accdd5e653948a6e40e9c3edf6314d4c6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:37:19 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:37:22 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Fri, 10 Feb 2023 22:37:22 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:37:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:37:26 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:37:27 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:37:27 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:37:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:37:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:37:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:37:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:37:30 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:37:30 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:37:31 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:37:31 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:37:31 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:37:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec2ab4edb1f0a14b28a55f050d62d8e54111075639a0fa8f173448814ba0d00`  
		Last Modified: Fri, 10 Feb 2023 22:38:25 GMT  
		Size: 342.6 KB (342588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0580184dd0082f009564a7a3923731f202cbe4bd8b857dbca2c77da8e7434815`  
		Last Modified: Fri, 10 Feb 2023 22:38:25 GMT  
		Size: 7.5 KB (7479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b2a44f2792add2104a1d53c68f1df95779deaee3ec86717f4fb4efd9aa6aaa`  
		Last Modified: Fri, 10 Feb 2023 22:38:28 GMT  
		Size: 13.6 MB (13591549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:4be5e6cdfb930681cc9c4722b0af67e75e53f0cff56c916c1d618eb39d6f5169
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16126925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:995c31e78c533c3ca73152cb87130dfcb16842dd052ab384df917fb755c5dc43`
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
# Fri, 10 Feb 2023 22:00:37 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:00:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:00:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:00:39 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:00:40 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:00:40 GMT
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
	-	`sha256:6403d7bb9250089f4077bba7631d975f97648fbcd782c992704ff3bccc5ae421`  
		Last Modified: Fri, 10 Feb 2023 22:01:03 GMT  
		Size: 13.1 MB (13059715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:50a289625f0ef1adfc05773b5ec8a30f001be347a84f24e1106e351f230758b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15949909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b11b3ee451004883e1f9089fc132ee1ecc849a2d96ef0ff4731334c8279cfa`
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
# Fri, 10 Feb 2023 22:13:23 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:13:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:13:28 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:13:28 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:13:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:13:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:13:33 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:13:33 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:13:33 GMT
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
	-	`sha256:2ecc7ec17344834a2337d83b9b7be44f97f0c0b55dfea5e1d8af80c8d5c32221`  
		Last Modified: Fri, 10 Feb 2023 22:14:19 GMT  
		Size: 12.8 MB (12774635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:9c69a670bfaa4e7166553c41a7303b114a524eed38924ad0d1d5599e6b7b2463
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16787086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9abb18c28ea7e824ff4385016f24b30d1a455d1b902f8667a1a9300078826a`
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
# Fri, 10 Feb 2023 22:14:19 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:14:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:14:21 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:14:22 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:14:23 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:14:23 GMT
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
	-	`sha256:94fd73a8831c9e57fdf8c430154c9adc56e54610a462128c8f0a1b3937aef704`  
		Last Modified: Fri, 10 Feb 2023 22:15:07 GMT  
		Size: 13.8 MB (13833147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:458901eb7e2d1f60ea430e23833e47d4b3ada93d601df57a34674b67675483b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3887; amd64
	-	windows version 10.0.20348.1487; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:b86e1de154ca5d11618a408742e2b6f16f99e55cdc0ee97fe0965da9f1b1572f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131390128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:858147920561fe47255b181692d82558dbab931f4393f33ba8697b9c647f690e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:50:11 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:50:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:23 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:01 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:02 GMT
WORKDIR /go
# Thu, 09 Feb 2023 03:18:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 03:18:17 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 03:18:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 03:18:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 03:18:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f8637abd914a8a62416e027a351293d0472bc4b4f44383c6f425fd0e03861c`  
		Last Modified: Mon, 09 Jan 2023 17:56:43 GMT  
		Size: 284.8 KB (284814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48e7ca896ec974241d86439d34188186e085705e42d914d8b7757c27eea8613`  
		Last Modified: Wed, 11 Jan 2023 00:08:38 GMT  
		Size: 122.3 MB (122328552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f26d270037d8578282b40f86c0a1816fc5d034d6213f7dcab8440056a589309`  
		Last Modified: Wed, 11 Jan 2023 00:08:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807cf12e90d621962959f760ccbca1b77b95c6120884fefcc4385f12614f9e49`  
		Last Modified: Thu, 09 Feb 2023 03:18:55 GMT  
		Size: 4.2 MB (4187743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1e21e6198268a646e1f41d15b44931dc2d1ffaf7448588af3237d7443de8df`  
		Last Modified: Thu, 09 Feb 2023 03:18:54 GMT  
		Size: 1.2 MB (1217832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86c409f0ecb7b6ab12d691c73e32350f6453fc6e477af6fe53ec7946e91ec08`  
		Last Modified: Thu, 09 Feb 2023 03:18:54 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2d6f2baed8a8d6af9014cc57d9488335fd4d9ded609476ce98307a241b55f680
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127387922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad435c186a3c6ffdd4910420eabfef5bbf8a84e247d2473ac2c1394e5ece3781`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:28:28 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:28:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:57:48 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:48 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:49 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:49:43 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:49:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:49:44 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:49:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:49:45 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:49:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:49:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:49:47 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3919da799d44c7be2eecafbf780801f4cd562b289c55ebe566999525497cd24`  
		Last Modified: Mon, 09 Jan 2023 17:37:35 GMT  
		Size: 286.1 KB (286122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c266a9580739a5c56dffcd14ce61144c9f58539d8c927ccd3df332434ad8d57`  
		Last Modified: Wed, 11 Jan 2023 00:11:13 GMT  
		Size: 118.7 MB (118677328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9666a7ae960b29537b5e693ea358a6181a3b9b73110b1099f22596b2dedbe3bd`  
		Last Modified: Wed, 11 Jan 2023 00:10:50 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b71d65a08c2aecf44c515cedf0abefc5f896bd9942291a29ddcf6646452661`  
		Last Modified: Wed, 08 Feb 2023 23:50:58 GMT  
		Size: 4.2 MB (4150629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a427cd9f7efb7c150d196c96034cdc132bf3c26025a87378400da762842a4923`  
		Last Modified: Wed, 08 Feb 2023 23:50:57 GMT  
		Size: 1.2 MB (1166069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278f59186f97ea59dd8a5f727fe7b3e2aa46b384971583b5b277b871a61b2131`  
		Last Modified: Wed, 08 Feb 2023 23:50:57 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:ad4dce5e6c2c07e73c35c50cdc26e110c439a947f626c86482c0bc5165ad8d9e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126503260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be8c29fce7791d265104052e6900b3eca71a13aa0b77861ded3aac664b4e9ae7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:04:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 10 Jan 2023 01:04:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:59:19 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:02:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:02:06 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:02:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:02:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:02:08 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:57:41 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:57:42 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:57:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:57:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:57:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c7609f223a73f5c1097b3b7cb1ea29e1e540da920bc3b48b8672a1d5ef1dc9`  
		Last Modified: Tue, 10 Jan 2023 01:13:57 GMT  
		Size: 285.4 KB (285359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da97c3a81e19449c60385f1e4cf4fd4fc9ffd14d08a26ccb6782cafd2d5d6f66`  
		Last Modified: Wed, 11 Jan 2023 00:15:15 GMT  
		Size: 118.5 MB (118468701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e98750b6aa4570218317d53b00f803a47aff7219e78c594d1666eef08e0258`  
		Last Modified: Wed, 11 Jan 2023 00:14:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ffc027d61bfbcc1c13359e022e0e4e6a5ef7cf40c49a8979e7d2f2a40add601`  
		Last Modified: Wed, 08 Feb 2023 23:58:48 GMT  
		Size: 3.7 MB (3720136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c82d9a2e5d63888f8bbe98b76b4b3565ccc2c8ce45526e794fae5f54d98ba49`  
		Last Modified: Wed, 08 Feb 2023 23:58:48 GMT  
		Size: 1.2 MB (1163326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0730779ca73578c83a210e39877a270c4a66834bd12b23cf515389d07213ac72`  
		Last Modified: Wed, 08 Feb 2023 23:58:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:bddc4b456724f377099c6889de30e23e6b434d71153db528d9746fade979f0c8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125786646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4850c9ee7a87ef514c7c4e3c3773db8494849b1ba453095ffe6fc5df07f158b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:37:51 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:37:52 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:14 GMT
ENV GOLANG_VERSION=1.19.5
# Tue, 10 Jan 2023 23:59:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Jan 2023 23:59:24 GMT
ENV GOPATH=/go
# Tue, 10 Jan 2023 23:59:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:59:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 10 Jan 2023 23:59:25 GMT
WORKDIR /go
# Thu, 09 Feb 2023 03:57:02 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 03:57:02 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 03:57:03 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:57:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 03:57:03 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 03:57:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 03:57:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 03:57:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3aa66ae7ca151fbd33126b15fa4d01bd5ceb35d53de36a8c6c82ecde58b596`  
		Last Modified: Mon, 09 Jan 2023 17:42:45 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491d6e59a2be619159e6630fabdf81f0255c275176cd97d109fa2f417935d6a8`  
		Last Modified: Wed, 11 Jan 2023 00:06:29 GMT  
		Size: 116.9 MB (116882841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4d12be79e26ab534722d5e8e5c9d931ed5ebd84ded16cae4b12390bb543502`  
		Last Modified: Wed, 11 Jan 2023 00:06:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c89dffd73dee99c1e6d53d4ea8cc302fa2089ee3edef14dc51585b33986fc9`  
		Last Modified: Thu, 09 Feb 2023 03:57:40 GMT  
		Size: 4.2 MB (4234011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cfcadb2a14be80b0bad3d94a219fcb7e0889a821a54688bc4ca6f47b905d88`  
		Last Modified: Thu, 09 Feb 2023 03:57:39 GMT  
		Size: 1.1 MB (1123736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b4461ab8f854d2e2000cacc11f5ee723a0888222cbd031ae1d1f0ae14c3e94`  
		Last Modified: Thu, 09 Feb 2023 03:57:39 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:7805a8da1341b4d0a403cd79ce628ded1f59f183d0c9d1a736e8d898370ca860
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126524152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c705e4439b5eac8b98303529a2168b757e4fad96343a01659c151be8647f401f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:13 GMT
ADD file:9a1d27fdc0c915f387f2446c85193d5215b18020b313114f0bf2799efcc1baae in / 
# Mon, 09 Jan 2023 17:05:13 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:34:40 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 21:34:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:42 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:01:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:01:19 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:01:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:01:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:01:20 GMT
WORKDIR /go
# Thu, 09 Feb 2023 06:18:37 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 06:18:37 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 06:18:38 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 06:18:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 06:18:38 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 06:18:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 06:18:42 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 06:18:42 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f45bfda3aa14e255d9eb4c9a108eb3d8c6721946b4aa2e5808e5092242344a1c`  
		Last Modified: Mon, 09 Jan 2023 17:05:56 GMT  
		Size: 3.4 MB (3384562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ab1c47929aa42b49b577230cb740bcf3e8aebc5abb60aabb4e6ee296dc2cad`  
		Last Modified: Mon, 09 Jan 2023 21:44:30 GMT  
		Size: 286.6 KB (286647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ded0f2fb726423b204889105ff334f3133acd9bbd8a5edfddad43e6e904485`  
		Last Modified: Wed, 11 Jan 2023 00:14:05 GMT  
		Size: 117.3 MB (117267319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c616b872c15882d15d49d081ce173bb6fa4e0f36ffead4b1938923db8038bd`  
		Last Modified: Wed, 11 Jan 2023 00:13:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e47ce9bd35950f8803ed14aa1fe38b85865479ec312ffa8b32df18b26add09`  
		Last Modified: Thu, 09 Feb 2023 06:19:42 GMT  
		Size: 4.5 MB (4479174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e8d19e2da6aa4d4205abf9c47ab0c45f001d2f8af00e99eb2bd7fec2852519`  
		Last Modified: Thu, 09 Feb 2023 06:19:41 GMT  
		Size: 1.1 MB (1105889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb53e3916ae4f3ac3cd8e441e2276b18484cf30de7a4f7b9ccb908933cd7502a`  
		Last Modified: Thu, 09 Feb 2023 06:19:41 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:3fa0a9eed3f7aaac0dbb713789109e64e4a585c7a9293211ecacc1d944b973be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129575744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a22f7e76fad31ed672b8977ea04a84eb19571daac58c337bd73a5c173ceecc6b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:44 GMT
ADD file:eabe7c3c368e65478b53ac35c1daf3b703f2bca4ecdab2d080a65e8b981d7d4a in / 
# Mon, 09 Jan 2023 17:05:46 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:42:43 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:42:43 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:53 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:56 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:57 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:41:57 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:41:58 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:42:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:42:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:42:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ae982806674c51a962c0fdd6e19f464ebd673df529c5cfb7c1d049e0b618d384`  
		Last Modified: Mon, 09 Jan 2023 17:06:50 GMT  
		Size: 3.2 MB (3170744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a5579d5fa8a33df30a972596fba4f03e76edabd19e57e62163b9c717fc188f`  
		Last Modified: Mon, 09 Jan 2023 17:54:33 GMT  
		Size: 285.0 KB (285022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4535e632f08f4af238fcccc27545520d10696aa3ce5920e33ba5578c3ee0e23`  
		Last Modified: Wed, 11 Jan 2023 00:12:31 GMT  
		Size: 120.8 MB (120785530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7633b4de83c59883de617e4ab5c606af3c556d6de4e45337bc59bff5bf7fe8ee`  
		Last Modified: Wed, 11 Jan 2023 00:12:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54414a7d37854703b1d037b805f6d0a49d2d398794414e3cedd1507c4bff0b82`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 4.2 MB (4163474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1779d1179e942debc68a6641287b6503a7e6949318c9272acb0273d7947d66e7`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 1.2 MB (1170413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597462f6847e463140e07072d10801a4c80c146d229deb04ef5cbc8b6f043464`  
		Last Modified: Wed, 08 Feb 2023 23:42:50 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.3887; amd64

```console
$ docker pull caddy@sha256:feeef34c537e9ea177fbaddb84e47df2e84a5cce70f7c8e3730e41822897b57e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1893070742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14ec5079fc868b1ce19abdcd6fca0964fae438be489b78914e21eac77dee89b3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 03:01:55 GMT
ENV GIT_VERSION=2.23.0
# Thu, 12 Jan 2023 03:01:56 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 12 Jan 2023 03:01:57 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 12 Jan 2023 03:01:58 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 12 Jan 2023 03:02:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:03:01 GMT
ENV GOPATH=C:\go
# Thu, 12 Jan 2023 03:03:35 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 Jan 2023 03:20:09 GMT
ENV GOLANG_VERSION=1.19.5
# Thu, 12 Jan 2023 03:23:52 GMT
RUN $url = 'https://dl.google.com/go/go1.19.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '167db91a2e40aeb453d3e59d213ecab06f62e1c4a84d13a06ccda1d999961caa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:23:54 GMT
WORKDIR C:\go
# Thu, 12 Jan 2023 05:33:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:19:59 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 00:20:00 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:20:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 00:20:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Feb 2023 00:20:35 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203425975bec1802428fad91a2e5f01172b161062c12eddf729e548bf7e134e0`  
		Last Modified: Thu, 12 Jan 2023 03:48:09 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80e42e19ab862b4adea06f1995e1f5cbb2c11ad8d68ae4a7bb5d0da5d0e6f38`  
		Last Modified: Thu, 12 Jan 2023 03:48:06 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be5d5df8cec6d1386f78a342668c3d2cb809372865459c1b35aa8d5a39a463b`  
		Last Modified: Thu, 12 Jan 2023 03:48:06 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e467d553c4972b55bf8e3d80b16f245e5bb38f28d80b91ca4f9f90c09a6c28d`  
		Last Modified: Thu, 12 Jan 2023 03:48:05 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97054b77b205167acd5a303c8aa82e380f090ff4e2ded81d3425ec78500139d`  
		Last Modified: Thu, 12 Jan 2023 03:48:14 GMT  
		Size: 25.5 MB (25470784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e150d9e1a1da09e17313cb3b6358d2f16cf2919c51e9addf30500de9d03292ef`  
		Last Modified: Thu, 12 Jan 2023 03:48:03 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c0d792e2a7942826a61fdc26b6081ab404122751ff4f4dd8f5b8b0eca21399`  
		Last Modified: Thu, 12 Jan 2023 03:48:03 GMT  
		Size: 324.5 KB (324466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cdd2ff60bbafbd62e677e0798ee562e3c4b291b841c6d0904ca080220e132a`  
		Last Modified: Thu, 12 Jan 2023 03:52:14 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17e6f8c13d649cbaec88dcdd4b1de7b004cf19227fbb4f923bd031b6b57988f`  
		Last Modified: Thu, 12 Jan 2023 03:53:12 GMT  
		Size: 157.7 MB (157659743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29fbb32977b62254a5de7ced98fe2a21e0342aa9db7b3cf32be4013d96b2cd9`  
		Last Modified: Thu, 12 Jan 2023 03:52:14 GMT  
		Size: 1.6 KB (1563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2fbb7e05d875affd4596aa7b87572980a3ab74800cff17a34deb445bed71b8`  
		Last Modified: Thu, 12 Jan 2023 05:36:53 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edae42a55d8aaff06e33b6f9ac104d54771346e5f4f59afd8ce90c794716611a`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb86a1e32dd5f27c1ba5ed4c675ff8c1477230677af11f17c75379385bd990b4`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d846d73e8be9adf7269d7376adebc7a8e8706b560a5f0d67886ab98c1d00c233`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2d31296154ed152465faac00831500590d35be69015063bb3ae3cc3514575d`  
		Last Modified: Thu, 09 Feb 2023 01:17:38 GMT  
		Size: 1.7 MB (1653847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef57a9413d8bab4ab7212470d9ac2b9eafc5efb5dc44aef718c91f935daddce`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.20348.1487; amd64

```console
$ docker pull caddy@sha256:e288b33447f0b01c2ee0954c57e574b43ce9ed4b56cbd813eca3cb1df8d9f766
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1572061864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c236dcd08d81ed31367d57c62c7e77e2421092030cd5365c6a225b0ad121c6b5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 02:57:40 GMT
ENV GIT_VERSION=2.23.0
# Thu, 12 Jan 2023 02:57:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 12 Jan 2023 02:57:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 12 Jan 2023 02:57:42 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 12 Jan 2023 02:58:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 02:58:23 GMT
ENV GOPATH=C:\go
# Thu, 12 Jan 2023 02:58:47 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 Jan 2023 03:16:17 GMT
ENV GOLANG_VERSION=1.19.5
# Thu, 12 Jan 2023 03:19:43 GMT
RUN $url = 'https://dl.google.com/go/go1.19.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '167db91a2e40aeb453d3e59d213ecab06f62e1c4a84d13a06ccda1d999961caa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:19:45 GMT
WORKDIR C:\go
# Thu, 12 Jan 2023 05:34:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:20:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 00:20:47 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:20:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 00:21:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Feb 2023 00:21:22 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2fc8728d9c7bf65edf893fd902f8b1bd780f93623858960c9db79e39922b169`  
		Last Modified: Thu, 12 Jan 2023 03:47:24 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7935a4c648078e79f67a11bcd5908e251110dd6c5a4ee49a607f332dd25af9`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d257f8b122044547f89f00f58661b25aca97c92f3831e7aaa11975639b6e35d4`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95acaa75c1852ba1320c5db382b01f587badb615b6746b59be27eedcf96ab667`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5201ba65043fa621c187729f18aecf4c549cdfa12cd6d8cab7a901d893f3a8a8`  
		Last Modified: Thu, 12 Jan 2023 03:47:29 GMT  
		Size: 25.7 MB (25702230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a317a349bca5ab28ba7c1ce039928a56390f7e7a8d7ddec07efcc1c9883e5d`  
		Last Modified: Thu, 12 Jan 2023 03:47:18 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8850296b8fbb853a6eb6341f7484cd4bc622e9f679f12c4123eddf08b7f398fb`  
		Last Modified: Thu, 12 Jan 2023 03:47:18 GMT  
		Size: 554.2 KB (554212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80b3d62f45a345eaac7caba0cdc514011cc61ea8f9d7d7b82d1bd4f8f3dbea4`  
		Last Modified: Thu, 12 Jan 2023 03:50:53 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320dc1bc3ac081a72fbca97a699b20068d92c70b3caaec8ca53036ab37509933`  
		Last Modified: Thu, 12 Jan 2023 03:51:58 GMT  
		Size: 157.9 MB (157885976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230636fcbea662dc69129c73285f4376c0b83a3222e8d438ec859d14ee1201b8`  
		Last Modified: Thu, 12 Jan 2023 03:50:53 GMT  
		Size: 1.6 KB (1569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581e22afffddeddb0a4127481e5016946bd3f35379291c6bb1e3b85e92e7acef`  
		Last Modified: Thu, 12 Jan 2023 05:37:10 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13aaa30213dc8e6b5906114a862d8398ac157fd2f8c835767a058069f180a181`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b39a2446c556432e7503cc419fe42c4d14ff3fc744cf6d475136c5058bc18d6`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43ea60403f6819d31f67d7dc2d230def090cb6366c7cd272d99d8d06aac019d`  
		Last Modified: Thu, 09 Feb 2023 01:17:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5970b711fddee53f278567276c42d2b169c5286a5133ba48ce3a599b253b37ab`  
		Last Modified: Thu, 09 Feb 2023 01:17:55 GMT  
		Size: 1.9 MB (1871861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1270e653c78ffbadd8ab6379e16db4c45c20fb148d294ec9654f1d13367fea6`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:e6c08f0694b44abd7ae623da15e368a4828a38cae59c041ab8f55c750fc66351
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
$ docker pull caddy@sha256:b86e1de154ca5d11618a408742e2b6f16f99e55cdc0ee97fe0965da9f1b1572f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131390128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:858147920561fe47255b181692d82558dbab931f4393f33ba8697b9c647f690e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:50:11 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:50:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:23 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:01 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:02 GMT
WORKDIR /go
# Thu, 09 Feb 2023 03:18:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 03:18:17 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 03:18:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 03:18:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 03:18:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f8637abd914a8a62416e027a351293d0472bc4b4f44383c6f425fd0e03861c`  
		Last Modified: Mon, 09 Jan 2023 17:56:43 GMT  
		Size: 284.8 KB (284814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48e7ca896ec974241d86439d34188186e085705e42d914d8b7757c27eea8613`  
		Last Modified: Wed, 11 Jan 2023 00:08:38 GMT  
		Size: 122.3 MB (122328552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f26d270037d8578282b40f86c0a1816fc5d034d6213f7dcab8440056a589309`  
		Last Modified: Wed, 11 Jan 2023 00:08:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807cf12e90d621962959f760ccbca1b77b95c6120884fefcc4385f12614f9e49`  
		Last Modified: Thu, 09 Feb 2023 03:18:55 GMT  
		Size: 4.2 MB (4187743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1e21e6198268a646e1f41d15b44931dc2d1ffaf7448588af3237d7443de8df`  
		Last Modified: Thu, 09 Feb 2023 03:18:54 GMT  
		Size: 1.2 MB (1217832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86c409f0ecb7b6ab12d691c73e32350f6453fc6e477af6fe53ec7946e91ec08`  
		Last Modified: Thu, 09 Feb 2023 03:18:54 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2d6f2baed8a8d6af9014cc57d9488335fd4d9ded609476ce98307a241b55f680
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127387922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad435c186a3c6ffdd4910420eabfef5bbf8a84e247d2473ac2c1394e5ece3781`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:28:28 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:28:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:57:48 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:48 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:49 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:49:43 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:49:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:49:44 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:49:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:49:45 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:49:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:49:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:49:47 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3919da799d44c7be2eecafbf780801f4cd562b289c55ebe566999525497cd24`  
		Last Modified: Mon, 09 Jan 2023 17:37:35 GMT  
		Size: 286.1 KB (286122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c266a9580739a5c56dffcd14ce61144c9f58539d8c927ccd3df332434ad8d57`  
		Last Modified: Wed, 11 Jan 2023 00:11:13 GMT  
		Size: 118.7 MB (118677328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9666a7ae960b29537b5e693ea358a6181a3b9b73110b1099f22596b2dedbe3bd`  
		Last Modified: Wed, 11 Jan 2023 00:10:50 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b71d65a08c2aecf44c515cedf0abefc5f896bd9942291a29ddcf6646452661`  
		Last Modified: Wed, 08 Feb 2023 23:50:58 GMT  
		Size: 4.2 MB (4150629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a427cd9f7efb7c150d196c96034cdc132bf3c26025a87378400da762842a4923`  
		Last Modified: Wed, 08 Feb 2023 23:50:57 GMT  
		Size: 1.2 MB (1166069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278f59186f97ea59dd8a5f727fe7b3e2aa46b384971583b5b277b871a61b2131`  
		Last Modified: Wed, 08 Feb 2023 23:50:57 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:ad4dce5e6c2c07e73c35c50cdc26e110c439a947f626c86482c0bc5165ad8d9e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126503260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be8c29fce7791d265104052e6900b3eca71a13aa0b77861ded3aac664b4e9ae7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:04:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 10 Jan 2023 01:04:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:59:19 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:02:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:02:06 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:02:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:02:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:02:08 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:57:41 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:57:42 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:57:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:57:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:57:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c7609f223a73f5c1097b3b7cb1ea29e1e540da920bc3b48b8672a1d5ef1dc9`  
		Last Modified: Tue, 10 Jan 2023 01:13:57 GMT  
		Size: 285.4 KB (285359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da97c3a81e19449c60385f1e4cf4fd4fc9ffd14d08a26ccb6782cafd2d5d6f66`  
		Last Modified: Wed, 11 Jan 2023 00:15:15 GMT  
		Size: 118.5 MB (118468701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e98750b6aa4570218317d53b00f803a47aff7219e78c594d1666eef08e0258`  
		Last Modified: Wed, 11 Jan 2023 00:14:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ffc027d61bfbcc1c13359e022e0e4e6a5ef7cf40c49a8979e7d2f2a40add601`  
		Last Modified: Wed, 08 Feb 2023 23:58:48 GMT  
		Size: 3.7 MB (3720136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c82d9a2e5d63888f8bbe98b76b4b3565ccc2c8ce45526e794fae5f54d98ba49`  
		Last Modified: Wed, 08 Feb 2023 23:58:48 GMT  
		Size: 1.2 MB (1163326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0730779ca73578c83a210e39877a270c4a66834bd12b23cf515389d07213ac72`  
		Last Modified: Wed, 08 Feb 2023 23:58:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:bddc4b456724f377099c6889de30e23e6b434d71153db528d9746fade979f0c8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125786646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4850c9ee7a87ef514c7c4e3c3773db8494849b1ba453095ffe6fc5df07f158b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:37:51 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:37:52 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:14 GMT
ENV GOLANG_VERSION=1.19.5
# Tue, 10 Jan 2023 23:59:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Jan 2023 23:59:24 GMT
ENV GOPATH=/go
# Tue, 10 Jan 2023 23:59:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:59:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 10 Jan 2023 23:59:25 GMT
WORKDIR /go
# Thu, 09 Feb 2023 03:57:02 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 03:57:02 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 03:57:03 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:57:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 03:57:03 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 03:57:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 03:57:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 03:57:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3aa66ae7ca151fbd33126b15fa4d01bd5ceb35d53de36a8c6c82ecde58b596`  
		Last Modified: Mon, 09 Jan 2023 17:42:45 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491d6e59a2be619159e6630fabdf81f0255c275176cd97d109fa2f417935d6a8`  
		Last Modified: Wed, 11 Jan 2023 00:06:29 GMT  
		Size: 116.9 MB (116882841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4d12be79e26ab534722d5e8e5c9d931ed5ebd84ded16cae4b12390bb543502`  
		Last Modified: Wed, 11 Jan 2023 00:06:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c89dffd73dee99c1e6d53d4ea8cc302fa2089ee3edef14dc51585b33986fc9`  
		Last Modified: Thu, 09 Feb 2023 03:57:40 GMT  
		Size: 4.2 MB (4234011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cfcadb2a14be80b0bad3d94a219fcb7e0889a821a54688bc4ca6f47b905d88`  
		Last Modified: Thu, 09 Feb 2023 03:57:39 GMT  
		Size: 1.1 MB (1123736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b4461ab8f854d2e2000cacc11f5ee723a0888222cbd031ae1d1f0ae14c3e94`  
		Last Modified: Thu, 09 Feb 2023 03:57:39 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:7805a8da1341b4d0a403cd79ce628ded1f59f183d0c9d1a736e8d898370ca860
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126524152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c705e4439b5eac8b98303529a2168b757e4fad96343a01659c151be8647f401f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:13 GMT
ADD file:9a1d27fdc0c915f387f2446c85193d5215b18020b313114f0bf2799efcc1baae in / 
# Mon, 09 Jan 2023 17:05:13 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:34:40 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 21:34:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:42 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:01:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:01:19 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:01:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:01:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:01:20 GMT
WORKDIR /go
# Thu, 09 Feb 2023 06:18:37 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 06:18:37 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 06:18:38 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 06:18:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 06:18:38 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 06:18:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 06:18:42 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 06:18:42 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f45bfda3aa14e255d9eb4c9a108eb3d8c6721946b4aa2e5808e5092242344a1c`  
		Last Modified: Mon, 09 Jan 2023 17:05:56 GMT  
		Size: 3.4 MB (3384562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ab1c47929aa42b49b577230cb740bcf3e8aebc5abb60aabb4e6ee296dc2cad`  
		Last Modified: Mon, 09 Jan 2023 21:44:30 GMT  
		Size: 286.6 KB (286647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ded0f2fb726423b204889105ff334f3133acd9bbd8a5edfddad43e6e904485`  
		Last Modified: Wed, 11 Jan 2023 00:14:05 GMT  
		Size: 117.3 MB (117267319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c616b872c15882d15d49d081ce173bb6fa4e0f36ffead4b1938923db8038bd`  
		Last Modified: Wed, 11 Jan 2023 00:13:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e47ce9bd35950f8803ed14aa1fe38b85865479ec312ffa8b32df18b26add09`  
		Last Modified: Thu, 09 Feb 2023 06:19:42 GMT  
		Size: 4.5 MB (4479174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e8d19e2da6aa4d4205abf9c47ab0c45f001d2f8af00e99eb2bd7fec2852519`  
		Last Modified: Thu, 09 Feb 2023 06:19:41 GMT  
		Size: 1.1 MB (1105889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb53e3916ae4f3ac3cd8e441e2276b18484cf30de7a4f7b9ccb908933cd7502a`  
		Last Modified: Thu, 09 Feb 2023 06:19:41 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:3fa0a9eed3f7aaac0dbb713789109e64e4a585c7a9293211ecacc1d944b973be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129575744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a22f7e76fad31ed672b8977ea04a84eb19571daac58c337bd73a5c173ceecc6b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:44 GMT
ADD file:eabe7c3c368e65478b53ac35c1daf3b703f2bca4ecdab2d080a65e8b981d7d4a in / 
# Mon, 09 Jan 2023 17:05:46 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:42:43 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:42:43 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:53 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:56 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:57 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:41:57 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:41:58 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:42:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:42:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:42:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ae982806674c51a962c0fdd6e19f464ebd673df529c5cfb7c1d049e0b618d384`  
		Last Modified: Mon, 09 Jan 2023 17:06:50 GMT  
		Size: 3.2 MB (3170744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a5579d5fa8a33df30a972596fba4f03e76edabd19e57e62163b9c717fc188f`  
		Last Modified: Mon, 09 Jan 2023 17:54:33 GMT  
		Size: 285.0 KB (285022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4535e632f08f4af238fcccc27545520d10696aa3ce5920e33ba5578c3ee0e23`  
		Last Modified: Wed, 11 Jan 2023 00:12:31 GMT  
		Size: 120.8 MB (120785530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7633b4de83c59883de617e4ab5c606af3c556d6de4e45337bc59bff5bf7fe8ee`  
		Last Modified: Wed, 11 Jan 2023 00:12:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54414a7d37854703b1d037b805f6d0a49d2d398794414e3cedd1507c4bff0b82`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 4.2 MB (4163474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1779d1179e942debc68a6641287b6503a7e6949318c9272acb0273d7947d66e7`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 1.2 MB (1170413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597462f6847e463140e07072d10801a4c80c146d229deb04ef5cbc8b6f043464`  
		Last Modified: Wed, 08 Feb 2023 23:42:50 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:4c57090f03b98d1a89618055d77e7e8864830bf83840fd17b1228bfa3cc8db4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull caddy@sha256:feeef34c537e9ea177fbaddb84e47df2e84a5cce70f7c8e3730e41822897b57e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1893070742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14ec5079fc868b1ce19abdcd6fca0964fae438be489b78914e21eac77dee89b3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 03:01:55 GMT
ENV GIT_VERSION=2.23.0
# Thu, 12 Jan 2023 03:01:56 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 12 Jan 2023 03:01:57 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 12 Jan 2023 03:01:58 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 12 Jan 2023 03:02:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:03:01 GMT
ENV GOPATH=C:\go
# Thu, 12 Jan 2023 03:03:35 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 Jan 2023 03:20:09 GMT
ENV GOLANG_VERSION=1.19.5
# Thu, 12 Jan 2023 03:23:52 GMT
RUN $url = 'https://dl.google.com/go/go1.19.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '167db91a2e40aeb453d3e59d213ecab06f62e1c4a84d13a06ccda1d999961caa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:23:54 GMT
WORKDIR C:\go
# Thu, 12 Jan 2023 05:33:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:19:59 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 00:20:00 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:20:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 00:20:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Feb 2023 00:20:35 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203425975bec1802428fad91a2e5f01172b161062c12eddf729e548bf7e134e0`  
		Last Modified: Thu, 12 Jan 2023 03:48:09 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80e42e19ab862b4adea06f1995e1f5cbb2c11ad8d68ae4a7bb5d0da5d0e6f38`  
		Last Modified: Thu, 12 Jan 2023 03:48:06 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be5d5df8cec6d1386f78a342668c3d2cb809372865459c1b35aa8d5a39a463b`  
		Last Modified: Thu, 12 Jan 2023 03:48:06 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e467d553c4972b55bf8e3d80b16f245e5bb38f28d80b91ca4f9f90c09a6c28d`  
		Last Modified: Thu, 12 Jan 2023 03:48:05 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97054b77b205167acd5a303c8aa82e380f090ff4e2ded81d3425ec78500139d`  
		Last Modified: Thu, 12 Jan 2023 03:48:14 GMT  
		Size: 25.5 MB (25470784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e150d9e1a1da09e17313cb3b6358d2f16cf2919c51e9addf30500de9d03292ef`  
		Last Modified: Thu, 12 Jan 2023 03:48:03 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c0d792e2a7942826a61fdc26b6081ab404122751ff4f4dd8f5b8b0eca21399`  
		Last Modified: Thu, 12 Jan 2023 03:48:03 GMT  
		Size: 324.5 KB (324466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cdd2ff60bbafbd62e677e0798ee562e3c4b291b841c6d0904ca080220e132a`  
		Last Modified: Thu, 12 Jan 2023 03:52:14 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17e6f8c13d649cbaec88dcdd4b1de7b004cf19227fbb4f923bd031b6b57988f`  
		Last Modified: Thu, 12 Jan 2023 03:53:12 GMT  
		Size: 157.7 MB (157659743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29fbb32977b62254a5de7ced98fe2a21e0342aa9db7b3cf32be4013d96b2cd9`  
		Last Modified: Thu, 12 Jan 2023 03:52:14 GMT  
		Size: 1.6 KB (1563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2fbb7e05d875affd4596aa7b87572980a3ab74800cff17a34deb445bed71b8`  
		Last Modified: Thu, 12 Jan 2023 05:36:53 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edae42a55d8aaff06e33b6f9ac104d54771346e5f4f59afd8ce90c794716611a`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb86a1e32dd5f27c1ba5ed4c675ff8c1477230677af11f17c75379385bd990b4`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d846d73e8be9adf7269d7376adebc7a8e8706b560a5f0d67886ab98c1d00c233`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2d31296154ed152465faac00831500590d35be69015063bb3ae3cc3514575d`  
		Last Modified: Thu, 09 Feb 2023 01:17:38 GMT  
		Size: 1.7 MB (1653847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef57a9413d8bab4ab7212470d9ac2b9eafc5efb5dc44aef718c91f935daddce`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:5016a9ee6f22300f4699ec2ba33c105b273e55c4b6931dcdbe8a7326d9dc037a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1487; amd64

### `caddy:2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1487; amd64

```console
$ docker pull caddy@sha256:e288b33447f0b01c2ee0954c57e574b43ce9ed4b56cbd813eca3cb1df8d9f766
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1572061864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c236dcd08d81ed31367d57c62c7e77e2421092030cd5365c6a225b0ad121c6b5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 02:57:40 GMT
ENV GIT_VERSION=2.23.0
# Thu, 12 Jan 2023 02:57:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 12 Jan 2023 02:57:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 12 Jan 2023 02:57:42 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 12 Jan 2023 02:58:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 02:58:23 GMT
ENV GOPATH=C:\go
# Thu, 12 Jan 2023 02:58:47 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 Jan 2023 03:16:17 GMT
ENV GOLANG_VERSION=1.19.5
# Thu, 12 Jan 2023 03:19:43 GMT
RUN $url = 'https://dl.google.com/go/go1.19.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '167db91a2e40aeb453d3e59d213ecab06f62e1c4a84d13a06ccda1d999961caa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:19:45 GMT
WORKDIR C:\go
# Thu, 12 Jan 2023 05:34:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:20:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 00:20:47 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:20:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 00:21:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Feb 2023 00:21:22 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2fc8728d9c7bf65edf893fd902f8b1bd780f93623858960c9db79e39922b169`  
		Last Modified: Thu, 12 Jan 2023 03:47:24 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7935a4c648078e79f67a11bcd5908e251110dd6c5a4ee49a607f332dd25af9`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d257f8b122044547f89f00f58661b25aca97c92f3831e7aaa11975639b6e35d4`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95acaa75c1852ba1320c5db382b01f587badb615b6746b59be27eedcf96ab667`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5201ba65043fa621c187729f18aecf4c549cdfa12cd6d8cab7a901d893f3a8a8`  
		Last Modified: Thu, 12 Jan 2023 03:47:29 GMT  
		Size: 25.7 MB (25702230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a317a349bca5ab28ba7c1ce039928a56390f7e7a8d7ddec07efcc1c9883e5d`  
		Last Modified: Thu, 12 Jan 2023 03:47:18 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8850296b8fbb853a6eb6341f7484cd4bc622e9f679f12c4123eddf08b7f398fb`  
		Last Modified: Thu, 12 Jan 2023 03:47:18 GMT  
		Size: 554.2 KB (554212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80b3d62f45a345eaac7caba0cdc514011cc61ea8f9d7d7b82d1bd4f8f3dbea4`  
		Last Modified: Thu, 12 Jan 2023 03:50:53 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320dc1bc3ac081a72fbca97a699b20068d92c70b3caaec8ca53036ab37509933`  
		Last Modified: Thu, 12 Jan 2023 03:51:58 GMT  
		Size: 157.9 MB (157885976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230636fcbea662dc69129c73285f4376c0b83a3222e8d438ec859d14ee1201b8`  
		Last Modified: Thu, 12 Jan 2023 03:50:53 GMT  
		Size: 1.6 KB (1569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581e22afffddeddb0a4127481e5016946bd3f35379291c6bb1e3b85e92e7acef`  
		Last Modified: Thu, 12 Jan 2023 05:37:10 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13aaa30213dc8e6b5906114a862d8398ac157fd2f8c835767a058069f180a181`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b39a2446c556432e7503cc419fe42c4d14ff3fc744cf6d475136c5058bc18d6`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43ea60403f6819d31f67d7dc2d230def090cb6366c7cd272d99d8d06aac019d`  
		Last Modified: Thu, 09 Feb 2023 01:17:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5970b711fddee53f278567276c42d2b169c5286a5133ba48ce3a599b253b37ab`  
		Last Modified: Thu, 09 Feb 2023 01:17:55 GMT  
		Size: 1.9 MB (1871861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1270e653c78ffbadd8ab6379e16db4c45c20fb148d294ec9654f1d13367fea6`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:0824e61dd8be6c1fa86bcf0faf1d4c5d8a41c047e0d4bf9ec8bbb73f243adaf6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3887; amd64
	-	windows version 10.0.20348.1487; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.3887; amd64

```console
$ docker pull caddy@sha256:935d1f4349cc551dfe9b76d6ba5fe6355414519a3037a7689fe765033ae8dcd6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1723388621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1deb1aecac8501d9afe22abd2fc90f15552c63366f8016ad2e6d1602be5cdf6d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:16:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:16:36 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:17:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:17:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:17:21 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:17:22 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:17:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:17:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:17:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:17:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:17:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:17:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:17:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:17:31 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:17:32 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:17:33 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:17:34 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:17:53 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:17:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47af8a9c9ef8e49d65e53dd207ad0935ce7a2b50b2f253e6a5b037494ae19d0a`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 401.5 KB (401472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5841cb6343add9dd7b89906610425117976b050c0634eedbc5c38302aa024e`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d760049e5c9f1fb1d7ec05a3eea55088808f484912e87cda07f3709363fe3c2c`  
		Last Modified: Thu, 09 Feb 2023 01:16:53 GMT  
		Size: 14.7 MB (14680484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3239225b5bad52e6004b638bd356e7d29e7fded5d31d90541907e1a769a115`  
		Last Modified: Thu, 09 Feb 2023 01:16:49 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6823ad091829bc6d98a58a18b075e20c551bde81d504bdbfda09b5a3d7c5d0`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4873a8802163accb90dd2318bd05ddfa4f94692b2731d6e23095e3bb46b98fd`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabf39e152fd5c18e0c3ac503e054c36e2775512f9fa7bb11b9221442b2bc1fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af12dc4018ba87a8e25003874e2d8e959a25b1c19932553daec8f4c410ebd61f`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fefa1f82e39e2af863b13609d78d966746d852af0cea54dcb17f45a8386c39d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d5b41708aea61714f00bc0f35ea1efc60db85c04ab6754e4d6b4485dc59a28`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a8b1cf8bcc4175323f7feaa280e3122f03aa7f9d35666fcc55c6b7d1e628ae`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c3f865e552649c436d5ffc0f3c83a3b5ba3026b2cff2ab3f381a5cdf2e2f2`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201cfdbfc1583e2ea070418e6aad0ec6604fb52c68117460b1a4c5b511b56ecc`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef83199fb67566ea043dbf7fab6f54754a4d0496655be1157819973573247bb`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45db789a3d9786dea133341e2c9f16e14b23a664297ad7f9a371961a0c21588`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a4e021c112717a1fee7cd62cdc17d41521f3514f10bf8ec30457b95aaf44fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4c0327054bc1f199339822d4074ee176c4184b9357ec28d9250f27f0c12e26`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63a4d912695117a127068d20ceefbaa19e41c8a42d65788d37915d737d998d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:44 GMT  
		Size: 338.6 KB (338620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421719fbbf536a3651d6762e36406f19dd0b5601f4a300d9c47af9ccfa3573d2`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.20348.1487; amd64

```console
$ docker pull caddy@sha256:22cdfda624195707c05f1d681c1cdd97b504f06b282d981718e1b716b2dc6bfb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1401937005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca7c6af6ec202266d95f15726fee733430a631c6c4eddfd9cc7d000b817a0f19`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:18:43 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:18:44 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:19:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:19:16 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:19:17 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:19:18 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:19:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:19:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:19:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:19:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:19:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:19:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:19:26 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:19:27 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:19:29 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:19:30 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:19:47 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:19:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42eb48143612ee855d99c932e324b1bd035c60554117edeaa805402060613c51`  
		Last Modified: Thu, 09 Feb 2023 01:17:17 GMT  
		Size: 635.9 KB (635943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714ae92cb5dac0e72097d35b932125b5ea3f03214de78e03119a4517be6fd10`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a5533d3ddbff5ea35dbb0e11b10fe817ce3ef1a3fd7f44706cb1b6288e0406`  
		Last Modified: Thu, 09 Feb 2023 01:17:20 GMT  
		Size: 14.9 MB (14899830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e59c8f0dc8d987210bdfe89eaded536b0ef8ac727eb7d75b76aea9c296208a`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22bfc3588219a43ce294aab21751b407ae75504bf3ddcee69f42498672b6c46`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f7db57dc0a0b0126433f60d3d0005f9aaa0d405fe63cfc3b4e15388fdfa010`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7b9e3a2510b5ab3b7ac4103d653c8efd12e95b63327d5c5fb81b6ea341e2b5`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4109b3b0ca73b5355a12ee74b7c32b4015a6208fdb279fd0ab60074247e22309`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3c568a1866d44483984b2be40142a55371adf3b8dc991bdb5ab4c45c0be3d4`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6221c7c14444b318e798e231adeeb83ea155c157283e9def018c43415238aa7`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e81980463382095586f78276db5cd808400136543fc1a0f522af1f3eaee034`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f0d8afe85320b7cf4542ad649671660bbb8e74ec3ad3067408e79fb21dbf77`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7def0e2b3dd94a350c82bb6a4903fdfc65d1d3d9772dd8195a5eb14ba766c45`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0b51c8090bf08cc2ae3a9fc340c9b70ba1e077f32b7d7d025b7d9fb472d978`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3653016f515e293fc93892b9e021e05a6a183ad3dcdaf243311513e222534c7`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d1dafd3fbb7403b7f093ed63553863bd9904f6010b1b91f98d9bfba9c4d8bb`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92817327253aaae4d632a75ff38a01dbebfe11f9105c4db828c52f221262ce4`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43bce457643a143e82e49e57d9b8a69a416e254d2439f30d7e4dd25c84e43c0`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 348.1 KB (348138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a0e899ab4c995de79522a5022b8cca4765559a4de2d5c728821d947b497de1`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:6fc3086452e6c85e993bf4b4834c55848a3977b547662cd4ce9fc98a17a495e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull caddy@sha256:935d1f4349cc551dfe9b76d6ba5fe6355414519a3037a7689fe765033ae8dcd6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1723388621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1deb1aecac8501d9afe22abd2fc90f15552c63366f8016ad2e6d1602be5cdf6d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:16:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:16:36 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:17:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:17:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:17:21 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:17:22 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:17:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:17:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:17:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:17:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:17:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:17:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:17:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:17:31 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:17:32 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:17:33 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:17:34 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:17:53 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:17:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47af8a9c9ef8e49d65e53dd207ad0935ce7a2b50b2f253e6a5b037494ae19d0a`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 401.5 KB (401472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5841cb6343add9dd7b89906610425117976b050c0634eedbc5c38302aa024e`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d760049e5c9f1fb1d7ec05a3eea55088808f484912e87cda07f3709363fe3c2c`  
		Last Modified: Thu, 09 Feb 2023 01:16:53 GMT  
		Size: 14.7 MB (14680484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3239225b5bad52e6004b638bd356e7d29e7fded5d31d90541907e1a769a115`  
		Last Modified: Thu, 09 Feb 2023 01:16:49 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6823ad091829bc6d98a58a18b075e20c551bde81d504bdbfda09b5a3d7c5d0`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4873a8802163accb90dd2318bd05ddfa4f94692b2731d6e23095e3bb46b98fd`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabf39e152fd5c18e0c3ac503e054c36e2775512f9fa7bb11b9221442b2bc1fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af12dc4018ba87a8e25003874e2d8e959a25b1c19932553daec8f4c410ebd61f`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fefa1f82e39e2af863b13609d78d966746d852af0cea54dcb17f45a8386c39d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d5b41708aea61714f00bc0f35ea1efc60db85c04ab6754e4d6b4485dc59a28`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a8b1cf8bcc4175323f7feaa280e3122f03aa7f9d35666fcc55c6b7d1e628ae`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c3f865e552649c436d5ffc0f3c83a3b5ba3026b2cff2ab3f381a5cdf2e2f2`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201cfdbfc1583e2ea070418e6aad0ec6604fb52c68117460b1a4c5b511b56ecc`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef83199fb67566ea043dbf7fab6f54754a4d0496655be1157819973573247bb`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45db789a3d9786dea133341e2c9f16e14b23a664297ad7f9a371961a0c21588`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a4e021c112717a1fee7cd62cdc17d41521f3514f10bf8ec30457b95aaf44fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4c0327054bc1f199339822d4074ee176c4184b9357ec28d9250f27f0c12e26`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63a4d912695117a127068d20ceefbaa19e41c8a42d65788d37915d737d998d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:44 GMT  
		Size: 338.6 KB (338620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421719fbbf536a3651d6762e36406f19dd0b5601f4a300d9c47af9ccfa3573d2`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:65b3d9f69c1f9e10dae44434f033715465a5e5331b38550f4f47baa12a60a39c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1487; amd64

### `caddy:2-windowsservercore-ltsc2022` - windows version 10.0.20348.1487; amd64

```console
$ docker pull caddy@sha256:22cdfda624195707c05f1d681c1cdd97b504f06b282d981718e1b716b2dc6bfb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1401937005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca7c6af6ec202266d95f15726fee733430a631c6c4eddfd9cc7d000b817a0f19`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:18:43 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:18:44 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:19:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:19:16 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:19:17 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:19:18 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:19:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:19:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:19:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:19:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:19:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:19:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:19:26 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:19:27 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:19:29 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:19:30 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:19:47 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:19:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42eb48143612ee855d99c932e324b1bd035c60554117edeaa805402060613c51`  
		Last Modified: Thu, 09 Feb 2023 01:17:17 GMT  
		Size: 635.9 KB (635943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714ae92cb5dac0e72097d35b932125b5ea3f03214de78e03119a4517be6fd10`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a5533d3ddbff5ea35dbb0e11b10fe817ce3ef1a3fd7f44706cb1b6288e0406`  
		Last Modified: Thu, 09 Feb 2023 01:17:20 GMT  
		Size: 14.9 MB (14899830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e59c8f0dc8d987210bdfe89eaded536b0ef8ac727eb7d75b76aea9c296208a`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22bfc3588219a43ce294aab21751b407ae75504bf3ddcee69f42498672b6c46`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f7db57dc0a0b0126433f60d3d0005f9aaa0d405fe63cfc3b4e15388fdfa010`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7b9e3a2510b5ab3b7ac4103d653c8efd12e95b63327d5c5fb81b6ea341e2b5`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4109b3b0ca73b5355a12ee74b7c32b4015a6208fdb279fd0ab60074247e22309`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3c568a1866d44483984b2be40142a55371adf3b8dc991bdb5ab4c45c0be3d4`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6221c7c14444b318e798e231adeeb83ea155c157283e9def018c43415238aa7`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e81980463382095586f78276db5cd808400136543fc1a0f522af1f3eaee034`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f0d8afe85320b7cf4542ad649671660bbb8e74ec3ad3067408e79fb21dbf77`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7def0e2b3dd94a350c82bb6a4903fdfc65d1d3d9772dd8195a5eb14ba766c45`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0b51c8090bf08cc2ae3a9fc340c9b70ba1e077f32b7d7d025b7d9fb472d978`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3653016f515e293fc93892b9e021e05a6a183ad3dcdaf243311513e222534c7`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d1dafd3fbb7403b7f093ed63553863bd9904f6010b1b91f98d9bfba9c4d8bb`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92817327253aaae4d632a75ff38a01dbebfe11f9105c4db828c52f221262ce4`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43bce457643a143e82e49e57d9b8a69a416e254d2439f30d7e4dd25c84e43c0`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 348.1 KB (348138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a0e899ab4c995de79522a5022b8cca4765559a4de2d5c728821d947b497de1`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6`

```console
$ docker pull caddy@sha256:d34a689107f831d1fb6dfb92ce4cff1569e409e5b6dcd2d671d4ffee8b112b76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3887; amd64
	-	windows version 10.0.20348.1487; amd64

### `caddy:2.6` - linux; amd64

```console
$ docker pull caddy@sha256:cf66a65d5667b26ba91fab680b59d421266e5042d4191fcdeab3847b31828bf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17441779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:739163e8bd53961abf96cc4f327498332dd905a59d3314fab80a845e62b58f9b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Thu, 09 Feb 2023 03:18:05 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 09 Feb 2023 03:18:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 09 Feb 2023 03:18:06 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:18:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 09 Feb 2023 03:18:10 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 09 Feb 2023 03:18:10 GMT
ENV XDG_DATA_HOME=/data
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 80
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 443
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 03:18:11 GMT
WORKDIR /srv
# Thu, 09 Feb 2023 03:18:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4cf81513fab9758787dbde95dcab4c054bd04137581b68097595a719ae973c`  
		Last Modified: Thu, 09 Feb 2023 03:18:39 GMT  
		Size: 351.2 KB (351181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c3f44eb3bccaf2f5515331e12d4b940a5f6ad016d27f548e0c739d1f6aba66`  
		Last Modified: Thu, 09 Feb 2023 03:18:39 GMT  
		Size: 7.6 KB (7554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04314ed686e612bbb7606d6bacff938564f9b4f7e0dbc72afacd887b3c88afbd`  
		Last Modified: Thu, 09 Feb 2023 03:18:42 GMT  
		Size: 14.3 MB (14276772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e4444abb42ab384f9685f3b25765ed65d8e07daef954ccf7aa73a524a2177064
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16576623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99391525993d815548f2a8e80455bb1ff1b6dd0a769a0dc2a467cbcc3adbc1ad`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:32 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Fri, 10 Feb 2023 20:49:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:28:54 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 21:28:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Fri, 10 Feb 2023 21:28:56 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 21:28:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 21:28:59 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 21:28:59 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 80
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 443
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 21:29:00 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 21:29:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a400dcba29ff44f8e5bf01493def4f19629aca6d103cb2a66ca87c457f7414`  
		Last Modified: Fri, 10 Feb 2023 21:29:47 GMT  
		Size: 345.8 KB (345811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b946768825eb5ed2fc6f932fdb0b0c552f4c35c39dada07eddd70ce4a535953`  
		Last Modified: Fri, 10 Feb 2023 21:29:47 GMT  
		Size: 7.5 KB (7480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda323f820516b366c61a02ba4cfd00cc3a3b6cc9051c58e7359057dea842d8a`  
		Last Modified: Fri, 10 Feb 2023 21:29:51 GMT  
		Size: 13.6 MB (13606554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0a66f97fe167ebcccd1754f2cc7ed8d5f42595f332f60d75e4efd33c5fa880b9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16362110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0940efa30038d45d9b6cbae2aea1235accdd5e653948a6e40e9c3edf6314d4c6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:37:19 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:37:22 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Fri, 10 Feb 2023 22:37:22 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:37:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:37:26 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:37:27 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:37:27 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:37:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:37:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:37:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:37:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:37:30 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:37:30 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:37:31 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:37:31 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:37:31 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:37:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec2ab4edb1f0a14b28a55f050d62d8e54111075639a0fa8f173448814ba0d00`  
		Last Modified: Fri, 10 Feb 2023 22:38:25 GMT  
		Size: 342.6 KB (342588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0580184dd0082f009564a7a3923731f202cbe4bd8b857dbca2c77da8e7434815`  
		Last Modified: Fri, 10 Feb 2023 22:38:25 GMT  
		Size: 7.5 KB (7479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b2a44f2792add2104a1d53c68f1df95779deaee3ec86717f4fb4efd9aa6aaa`  
		Last Modified: Fri, 10 Feb 2023 22:38:28 GMT  
		Size: 13.6 MB (13591549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:4be5e6cdfb930681cc9c4722b0af67e75e53f0cff56c916c1d618eb39d6f5169
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16126925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:995c31e78c533c3ca73152cb87130dfcb16842dd052ab384df917fb755c5dc43`
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
# Fri, 10 Feb 2023 22:00:37 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:00:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:00:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:00:39 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:00:40 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:00:40 GMT
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
	-	`sha256:6403d7bb9250089f4077bba7631d975f97648fbcd782c992704ff3bccc5ae421`  
		Last Modified: Fri, 10 Feb 2023 22:01:03 GMT  
		Size: 13.1 MB (13059715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - linux; ppc64le

```console
$ docker pull caddy@sha256:50a289625f0ef1adfc05773b5ec8a30f001be347a84f24e1106e351f230758b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15949909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b11b3ee451004883e1f9089fc132ee1ecc849a2d96ef0ff4731334c8279cfa`
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
# Fri, 10 Feb 2023 22:13:23 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:13:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:13:28 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:13:28 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:13:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:13:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:13:33 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:13:33 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:13:33 GMT
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
	-	`sha256:2ecc7ec17344834a2337d83b9b7be44f97f0c0b55dfea5e1d8af80c8d5c32221`  
		Last Modified: Fri, 10 Feb 2023 22:14:19 GMT  
		Size: 12.8 MB (12774635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - linux; s390x

```console
$ docker pull caddy@sha256:9c69a670bfaa4e7166553c41a7303b114a524eed38924ad0d1d5599e6b7b2463
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16787086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9abb18c28ea7e824ff4385016f24b30d1a455d1b902f8667a1a9300078826a`
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
# Fri, 10 Feb 2023 22:14:19 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:14:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:14:21 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:14:22 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:14:23 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:14:23 GMT
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
	-	`sha256:94fd73a8831c9e57fdf8c430154c9adc56e54610a462128c8f0a1b3937aef704`  
		Last Modified: Fri, 10 Feb 2023 22:15:07 GMT  
		Size: 13.8 MB (13833147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - windows version 10.0.17763.3887; amd64

```console
$ docker pull caddy@sha256:935d1f4349cc551dfe9b76d6ba5fe6355414519a3037a7689fe765033ae8dcd6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1723388621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1deb1aecac8501d9afe22abd2fc90f15552c63366f8016ad2e6d1602be5cdf6d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:16:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:16:36 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:17:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:17:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:17:21 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:17:22 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:17:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:17:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:17:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:17:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:17:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:17:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:17:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:17:31 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:17:32 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:17:33 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:17:34 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:17:53 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:17:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47af8a9c9ef8e49d65e53dd207ad0935ce7a2b50b2f253e6a5b037494ae19d0a`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 401.5 KB (401472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5841cb6343add9dd7b89906610425117976b050c0634eedbc5c38302aa024e`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d760049e5c9f1fb1d7ec05a3eea55088808f484912e87cda07f3709363fe3c2c`  
		Last Modified: Thu, 09 Feb 2023 01:16:53 GMT  
		Size: 14.7 MB (14680484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3239225b5bad52e6004b638bd356e7d29e7fded5d31d90541907e1a769a115`  
		Last Modified: Thu, 09 Feb 2023 01:16:49 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6823ad091829bc6d98a58a18b075e20c551bde81d504bdbfda09b5a3d7c5d0`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4873a8802163accb90dd2318bd05ddfa4f94692b2731d6e23095e3bb46b98fd`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabf39e152fd5c18e0c3ac503e054c36e2775512f9fa7bb11b9221442b2bc1fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af12dc4018ba87a8e25003874e2d8e959a25b1c19932553daec8f4c410ebd61f`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fefa1f82e39e2af863b13609d78d966746d852af0cea54dcb17f45a8386c39d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d5b41708aea61714f00bc0f35ea1efc60db85c04ab6754e4d6b4485dc59a28`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a8b1cf8bcc4175323f7feaa280e3122f03aa7f9d35666fcc55c6b7d1e628ae`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c3f865e552649c436d5ffc0f3c83a3b5ba3026b2cff2ab3f381a5cdf2e2f2`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201cfdbfc1583e2ea070418e6aad0ec6604fb52c68117460b1a4c5b511b56ecc`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef83199fb67566ea043dbf7fab6f54754a4d0496655be1157819973573247bb`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45db789a3d9786dea133341e2c9f16e14b23a664297ad7f9a371961a0c21588`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a4e021c112717a1fee7cd62cdc17d41521f3514f10bf8ec30457b95aaf44fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4c0327054bc1f199339822d4074ee176c4184b9357ec28d9250f27f0c12e26`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63a4d912695117a127068d20ceefbaa19e41c8a42d65788d37915d737d998d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:44 GMT  
		Size: 338.6 KB (338620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421719fbbf536a3651d6762e36406f19dd0b5601f4a300d9c47af9ccfa3573d2`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - windows version 10.0.20348.1487; amd64

```console
$ docker pull caddy@sha256:22cdfda624195707c05f1d681c1cdd97b504f06b282d981718e1b716b2dc6bfb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1401937005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca7c6af6ec202266d95f15726fee733430a631c6c4eddfd9cc7d000b817a0f19`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:18:43 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:18:44 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:19:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:19:16 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:19:17 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:19:18 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:19:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:19:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:19:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:19:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:19:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:19:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:19:26 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:19:27 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:19:29 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:19:30 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:19:47 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:19:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42eb48143612ee855d99c932e324b1bd035c60554117edeaa805402060613c51`  
		Last Modified: Thu, 09 Feb 2023 01:17:17 GMT  
		Size: 635.9 KB (635943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714ae92cb5dac0e72097d35b932125b5ea3f03214de78e03119a4517be6fd10`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a5533d3ddbff5ea35dbb0e11b10fe817ce3ef1a3fd7f44706cb1b6288e0406`  
		Last Modified: Thu, 09 Feb 2023 01:17:20 GMT  
		Size: 14.9 MB (14899830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e59c8f0dc8d987210bdfe89eaded536b0ef8ac727eb7d75b76aea9c296208a`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22bfc3588219a43ce294aab21751b407ae75504bf3ddcee69f42498672b6c46`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f7db57dc0a0b0126433f60d3d0005f9aaa0d405fe63cfc3b4e15388fdfa010`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7b9e3a2510b5ab3b7ac4103d653c8efd12e95b63327d5c5fb81b6ea341e2b5`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4109b3b0ca73b5355a12ee74b7c32b4015a6208fdb279fd0ab60074247e22309`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3c568a1866d44483984b2be40142a55371adf3b8dc991bdb5ab4c45c0be3d4`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6221c7c14444b318e798e231adeeb83ea155c157283e9def018c43415238aa7`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e81980463382095586f78276db5cd808400136543fc1a0f522af1f3eaee034`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f0d8afe85320b7cf4542ad649671660bbb8e74ec3ad3067408e79fb21dbf77`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7def0e2b3dd94a350c82bb6a4903fdfc65d1d3d9772dd8195a5eb14ba766c45`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0b51c8090bf08cc2ae3a9fc340c9b70ba1e077f32b7d7d025b7d9fb472d978`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3653016f515e293fc93892b9e021e05a6a183ad3dcdaf243311513e222534c7`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d1dafd3fbb7403b7f093ed63553863bd9904f6010b1b91f98d9bfba9c4d8bb`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92817327253aaae4d632a75ff38a01dbebfe11f9105c4db828c52f221262ce4`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43bce457643a143e82e49e57d9b8a69a416e254d2439f30d7e4dd25c84e43c0`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 348.1 KB (348138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a0e899ab4c995de79522a5022b8cca4765559a4de2d5c728821d947b497de1`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-alpine`

```console
$ docker pull caddy@sha256:7e7286bb77df853f278887dd9159bd643abca8447ad4a0fddb4c48ec00a7e6cc
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
$ docker pull caddy@sha256:cf66a65d5667b26ba91fab680b59d421266e5042d4191fcdeab3847b31828bf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17441779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:739163e8bd53961abf96cc4f327498332dd905a59d3314fab80a845e62b58f9b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Thu, 09 Feb 2023 03:18:05 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 09 Feb 2023 03:18:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 09 Feb 2023 03:18:06 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:18:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 09 Feb 2023 03:18:10 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 09 Feb 2023 03:18:10 GMT
ENV XDG_DATA_HOME=/data
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 80
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 443
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 03:18:11 GMT
WORKDIR /srv
# Thu, 09 Feb 2023 03:18:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4cf81513fab9758787dbde95dcab4c054bd04137581b68097595a719ae973c`  
		Last Modified: Thu, 09 Feb 2023 03:18:39 GMT  
		Size: 351.2 KB (351181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c3f44eb3bccaf2f5515331e12d4b940a5f6ad016d27f548e0c739d1f6aba66`  
		Last Modified: Thu, 09 Feb 2023 03:18:39 GMT  
		Size: 7.6 KB (7554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04314ed686e612bbb7606d6bacff938564f9b4f7e0dbc72afacd887b3c88afbd`  
		Last Modified: Thu, 09 Feb 2023 03:18:42 GMT  
		Size: 14.3 MB (14276772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e4444abb42ab384f9685f3b25765ed65d8e07daef954ccf7aa73a524a2177064
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16576623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99391525993d815548f2a8e80455bb1ff1b6dd0a769a0dc2a467cbcc3adbc1ad`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:32 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Fri, 10 Feb 2023 20:49:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:28:54 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 21:28:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Fri, 10 Feb 2023 21:28:56 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 21:28:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 21:28:59 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 21:28:59 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 80
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 443
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 21:29:00 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 21:29:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a400dcba29ff44f8e5bf01493def4f19629aca6d103cb2a66ca87c457f7414`  
		Last Modified: Fri, 10 Feb 2023 21:29:47 GMT  
		Size: 345.8 KB (345811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b946768825eb5ed2fc6f932fdb0b0c552f4c35c39dada07eddd70ce4a535953`  
		Last Modified: Fri, 10 Feb 2023 21:29:47 GMT  
		Size: 7.5 KB (7480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda323f820516b366c61a02ba4cfd00cc3a3b6cc9051c58e7359057dea842d8a`  
		Last Modified: Fri, 10 Feb 2023 21:29:51 GMT  
		Size: 13.6 MB (13606554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0a66f97fe167ebcccd1754f2cc7ed8d5f42595f332f60d75e4efd33c5fa880b9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16362110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0940efa30038d45d9b6cbae2aea1235accdd5e653948a6e40e9c3edf6314d4c6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:37:19 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:37:22 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Fri, 10 Feb 2023 22:37:22 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:37:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:37:26 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:37:27 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:37:27 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:37:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:37:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:37:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:37:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:37:30 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:37:30 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:37:31 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:37:31 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:37:31 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:37:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec2ab4edb1f0a14b28a55f050d62d8e54111075639a0fa8f173448814ba0d00`  
		Last Modified: Fri, 10 Feb 2023 22:38:25 GMT  
		Size: 342.6 KB (342588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0580184dd0082f009564a7a3923731f202cbe4bd8b857dbca2c77da8e7434815`  
		Last Modified: Fri, 10 Feb 2023 22:38:25 GMT  
		Size: 7.5 KB (7479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b2a44f2792add2104a1d53c68f1df95779deaee3ec86717f4fb4efd9aa6aaa`  
		Last Modified: Fri, 10 Feb 2023 22:38:28 GMT  
		Size: 13.6 MB (13591549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:4be5e6cdfb930681cc9c4722b0af67e75e53f0cff56c916c1d618eb39d6f5169
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16126925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:995c31e78c533c3ca73152cb87130dfcb16842dd052ab384df917fb755c5dc43`
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
# Fri, 10 Feb 2023 22:00:37 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:00:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:00:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:00:39 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:00:40 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:00:40 GMT
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
	-	`sha256:6403d7bb9250089f4077bba7631d975f97648fbcd782c992704ff3bccc5ae421`  
		Last Modified: Fri, 10 Feb 2023 22:01:03 GMT  
		Size: 13.1 MB (13059715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:50a289625f0ef1adfc05773b5ec8a30f001be347a84f24e1106e351f230758b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15949909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b11b3ee451004883e1f9089fc132ee1ecc849a2d96ef0ff4731334c8279cfa`
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
# Fri, 10 Feb 2023 22:13:23 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:13:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:13:28 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:13:28 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:13:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:13:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:13:33 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:13:33 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:13:33 GMT
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
	-	`sha256:2ecc7ec17344834a2337d83b9b7be44f97f0c0b55dfea5e1d8af80c8d5c32221`  
		Last Modified: Fri, 10 Feb 2023 22:14:19 GMT  
		Size: 12.8 MB (12774635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:9c69a670bfaa4e7166553c41a7303b114a524eed38924ad0d1d5599e6b7b2463
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16787086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9abb18c28ea7e824ff4385016f24b30d1a455d1b902f8667a1a9300078826a`
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
# Fri, 10 Feb 2023 22:14:19 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:14:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:14:21 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:14:22 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:14:23 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:14:23 GMT
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
	-	`sha256:94fd73a8831c9e57fdf8c430154c9adc56e54610a462128c8f0a1b3937aef704`  
		Last Modified: Fri, 10 Feb 2023 22:15:07 GMT  
		Size: 13.8 MB (13833147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder`

```console
$ docker pull caddy@sha256:458901eb7e2d1f60ea430e23833e47d4b3ada93d601df57a34674b67675483b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3887; amd64
	-	windows version 10.0.20348.1487; amd64

### `caddy:2.6-builder` - linux; amd64

```console
$ docker pull caddy@sha256:b86e1de154ca5d11618a408742e2b6f16f99e55cdc0ee97fe0965da9f1b1572f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131390128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:858147920561fe47255b181692d82558dbab931f4393f33ba8697b9c647f690e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:50:11 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:50:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:23 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:01 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:02 GMT
WORKDIR /go
# Thu, 09 Feb 2023 03:18:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 03:18:17 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 03:18:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 03:18:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 03:18:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f8637abd914a8a62416e027a351293d0472bc4b4f44383c6f425fd0e03861c`  
		Last Modified: Mon, 09 Jan 2023 17:56:43 GMT  
		Size: 284.8 KB (284814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48e7ca896ec974241d86439d34188186e085705e42d914d8b7757c27eea8613`  
		Last Modified: Wed, 11 Jan 2023 00:08:38 GMT  
		Size: 122.3 MB (122328552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f26d270037d8578282b40f86c0a1816fc5d034d6213f7dcab8440056a589309`  
		Last Modified: Wed, 11 Jan 2023 00:08:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807cf12e90d621962959f760ccbca1b77b95c6120884fefcc4385f12614f9e49`  
		Last Modified: Thu, 09 Feb 2023 03:18:55 GMT  
		Size: 4.2 MB (4187743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1e21e6198268a646e1f41d15b44931dc2d1ffaf7448588af3237d7443de8df`  
		Last Modified: Thu, 09 Feb 2023 03:18:54 GMT  
		Size: 1.2 MB (1217832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86c409f0ecb7b6ab12d691c73e32350f6453fc6e477af6fe53ec7946e91ec08`  
		Last Modified: Thu, 09 Feb 2023 03:18:54 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2d6f2baed8a8d6af9014cc57d9488335fd4d9ded609476ce98307a241b55f680
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127387922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad435c186a3c6ffdd4910420eabfef5bbf8a84e247d2473ac2c1394e5ece3781`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:28:28 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:28:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:57:48 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:48 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:49 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:49:43 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:49:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:49:44 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:49:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:49:45 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:49:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:49:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:49:47 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3919da799d44c7be2eecafbf780801f4cd562b289c55ebe566999525497cd24`  
		Last Modified: Mon, 09 Jan 2023 17:37:35 GMT  
		Size: 286.1 KB (286122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c266a9580739a5c56dffcd14ce61144c9f58539d8c927ccd3df332434ad8d57`  
		Last Modified: Wed, 11 Jan 2023 00:11:13 GMT  
		Size: 118.7 MB (118677328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9666a7ae960b29537b5e693ea358a6181a3b9b73110b1099f22596b2dedbe3bd`  
		Last Modified: Wed, 11 Jan 2023 00:10:50 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b71d65a08c2aecf44c515cedf0abefc5f896bd9942291a29ddcf6646452661`  
		Last Modified: Wed, 08 Feb 2023 23:50:58 GMT  
		Size: 4.2 MB (4150629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a427cd9f7efb7c150d196c96034cdc132bf3c26025a87378400da762842a4923`  
		Last Modified: Wed, 08 Feb 2023 23:50:57 GMT  
		Size: 1.2 MB (1166069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278f59186f97ea59dd8a5f727fe7b3e2aa46b384971583b5b277b871a61b2131`  
		Last Modified: Wed, 08 Feb 2023 23:50:57 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:ad4dce5e6c2c07e73c35c50cdc26e110c439a947f626c86482c0bc5165ad8d9e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126503260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be8c29fce7791d265104052e6900b3eca71a13aa0b77861ded3aac664b4e9ae7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:04:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 10 Jan 2023 01:04:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:59:19 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:02:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:02:06 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:02:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:02:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:02:08 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:57:41 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:57:42 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:57:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:57:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:57:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c7609f223a73f5c1097b3b7cb1ea29e1e540da920bc3b48b8672a1d5ef1dc9`  
		Last Modified: Tue, 10 Jan 2023 01:13:57 GMT  
		Size: 285.4 KB (285359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da97c3a81e19449c60385f1e4cf4fd4fc9ffd14d08a26ccb6782cafd2d5d6f66`  
		Last Modified: Wed, 11 Jan 2023 00:15:15 GMT  
		Size: 118.5 MB (118468701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e98750b6aa4570218317d53b00f803a47aff7219e78c594d1666eef08e0258`  
		Last Modified: Wed, 11 Jan 2023 00:14:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ffc027d61bfbcc1c13359e022e0e4e6a5ef7cf40c49a8979e7d2f2a40add601`  
		Last Modified: Wed, 08 Feb 2023 23:58:48 GMT  
		Size: 3.7 MB (3720136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c82d9a2e5d63888f8bbe98b76b4b3565ccc2c8ce45526e794fae5f54d98ba49`  
		Last Modified: Wed, 08 Feb 2023 23:58:48 GMT  
		Size: 1.2 MB (1163326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0730779ca73578c83a210e39877a270c4a66834bd12b23cf515389d07213ac72`  
		Last Modified: Wed, 08 Feb 2023 23:58:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:bddc4b456724f377099c6889de30e23e6b434d71153db528d9746fade979f0c8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125786646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4850c9ee7a87ef514c7c4e3c3773db8494849b1ba453095ffe6fc5df07f158b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:37:51 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:37:52 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:14 GMT
ENV GOLANG_VERSION=1.19.5
# Tue, 10 Jan 2023 23:59:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Jan 2023 23:59:24 GMT
ENV GOPATH=/go
# Tue, 10 Jan 2023 23:59:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:59:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 10 Jan 2023 23:59:25 GMT
WORKDIR /go
# Thu, 09 Feb 2023 03:57:02 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 03:57:02 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 03:57:03 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:57:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 03:57:03 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 03:57:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 03:57:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 03:57:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3aa66ae7ca151fbd33126b15fa4d01bd5ceb35d53de36a8c6c82ecde58b596`  
		Last Modified: Mon, 09 Jan 2023 17:42:45 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491d6e59a2be619159e6630fabdf81f0255c275176cd97d109fa2f417935d6a8`  
		Last Modified: Wed, 11 Jan 2023 00:06:29 GMT  
		Size: 116.9 MB (116882841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4d12be79e26ab534722d5e8e5c9d931ed5ebd84ded16cae4b12390bb543502`  
		Last Modified: Wed, 11 Jan 2023 00:06:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c89dffd73dee99c1e6d53d4ea8cc302fa2089ee3edef14dc51585b33986fc9`  
		Last Modified: Thu, 09 Feb 2023 03:57:40 GMT  
		Size: 4.2 MB (4234011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cfcadb2a14be80b0bad3d94a219fcb7e0889a821a54688bc4ca6f47b905d88`  
		Last Modified: Thu, 09 Feb 2023 03:57:39 GMT  
		Size: 1.1 MB (1123736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b4461ab8f854d2e2000cacc11f5ee723a0888222cbd031ae1d1f0ae14c3e94`  
		Last Modified: Thu, 09 Feb 2023 03:57:39 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:7805a8da1341b4d0a403cd79ce628ded1f59f183d0c9d1a736e8d898370ca860
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126524152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c705e4439b5eac8b98303529a2168b757e4fad96343a01659c151be8647f401f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:13 GMT
ADD file:9a1d27fdc0c915f387f2446c85193d5215b18020b313114f0bf2799efcc1baae in / 
# Mon, 09 Jan 2023 17:05:13 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:34:40 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 21:34:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:42 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:01:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:01:19 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:01:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:01:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:01:20 GMT
WORKDIR /go
# Thu, 09 Feb 2023 06:18:37 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 06:18:37 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 06:18:38 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 06:18:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 06:18:38 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 06:18:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 06:18:42 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 06:18:42 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f45bfda3aa14e255d9eb4c9a108eb3d8c6721946b4aa2e5808e5092242344a1c`  
		Last Modified: Mon, 09 Jan 2023 17:05:56 GMT  
		Size: 3.4 MB (3384562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ab1c47929aa42b49b577230cb740bcf3e8aebc5abb60aabb4e6ee296dc2cad`  
		Last Modified: Mon, 09 Jan 2023 21:44:30 GMT  
		Size: 286.6 KB (286647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ded0f2fb726423b204889105ff334f3133acd9bbd8a5edfddad43e6e904485`  
		Last Modified: Wed, 11 Jan 2023 00:14:05 GMT  
		Size: 117.3 MB (117267319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c616b872c15882d15d49d081ce173bb6fa4e0f36ffead4b1938923db8038bd`  
		Last Modified: Wed, 11 Jan 2023 00:13:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e47ce9bd35950f8803ed14aa1fe38b85865479ec312ffa8b32df18b26add09`  
		Last Modified: Thu, 09 Feb 2023 06:19:42 GMT  
		Size: 4.5 MB (4479174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e8d19e2da6aa4d4205abf9c47ab0c45f001d2f8af00e99eb2bd7fec2852519`  
		Last Modified: Thu, 09 Feb 2023 06:19:41 GMT  
		Size: 1.1 MB (1105889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb53e3916ae4f3ac3cd8e441e2276b18484cf30de7a4f7b9ccb908933cd7502a`  
		Last Modified: Thu, 09 Feb 2023 06:19:41 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; s390x

```console
$ docker pull caddy@sha256:3fa0a9eed3f7aaac0dbb713789109e64e4a585c7a9293211ecacc1d944b973be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129575744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a22f7e76fad31ed672b8977ea04a84eb19571daac58c337bd73a5c173ceecc6b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:44 GMT
ADD file:eabe7c3c368e65478b53ac35c1daf3b703f2bca4ecdab2d080a65e8b981d7d4a in / 
# Mon, 09 Jan 2023 17:05:46 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:42:43 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:42:43 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:53 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:56 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:57 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:41:57 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:41:58 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:42:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:42:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:42:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ae982806674c51a962c0fdd6e19f464ebd673df529c5cfb7c1d049e0b618d384`  
		Last Modified: Mon, 09 Jan 2023 17:06:50 GMT  
		Size: 3.2 MB (3170744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a5579d5fa8a33df30a972596fba4f03e76edabd19e57e62163b9c717fc188f`  
		Last Modified: Mon, 09 Jan 2023 17:54:33 GMT  
		Size: 285.0 KB (285022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4535e632f08f4af238fcccc27545520d10696aa3ce5920e33ba5578c3ee0e23`  
		Last Modified: Wed, 11 Jan 2023 00:12:31 GMT  
		Size: 120.8 MB (120785530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7633b4de83c59883de617e4ab5c606af3c556d6de4e45337bc59bff5bf7fe8ee`  
		Last Modified: Wed, 11 Jan 2023 00:12:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54414a7d37854703b1d037b805f6d0a49d2d398794414e3cedd1507c4bff0b82`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 4.2 MB (4163474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1779d1179e942debc68a6641287b6503a7e6949318c9272acb0273d7947d66e7`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 1.2 MB (1170413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597462f6847e463140e07072d10801a4c80c146d229deb04ef5cbc8b6f043464`  
		Last Modified: Wed, 08 Feb 2023 23:42:50 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - windows version 10.0.17763.3887; amd64

```console
$ docker pull caddy@sha256:feeef34c537e9ea177fbaddb84e47df2e84a5cce70f7c8e3730e41822897b57e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1893070742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14ec5079fc868b1ce19abdcd6fca0964fae438be489b78914e21eac77dee89b3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 03:01:55 GMT
ENV GIT_VERSION=2.23.0
# Thu, 12 Jan 2023 03:01:56 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 12 Jan 2023 03:01:57 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 12 Jan 2023 03:01:58 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 12 Jan 2023 03:02:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:03:01 GMT
ENV GOPATH=C:\go
# Thu, 12 Jan 2023 03:03:35 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 Jan 2023 03:20:09 GMT
ENV GOLANG_VERSION=1.19.5
# Thu, 12 Jan 2023 03:23:52 GMT
RUN $url = 'https://dl.google.com/go/go1.19.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '167db91a2e40aeb453d3e59d213ecab06f62e1c4a84d13a06ccda1d999961caa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:23:54 GMT
WORKDIR C:\go
# Thu, 12 Jan 2023 05:33:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:19:59 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 00:20:00 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:20:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 00:20:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Feb 2023 00:20:35 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203425975bec1802428fad91a2e5f01172b161062c12eddf729e548bf7e134e0`  
		Last Modified: Thu, 12 Jan 2023 03:48:09 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80e42e19ab862b4adea06f1995e1f5cbb2c11ad8d68ae4a7bb5d0da5d0e6f38`  
		Last Modified: Thu, 12 Jan 2023 03:48:06 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be5d5df8cec6d1386f78a342668c3d2cb809372865459c1b35aa8d5a39a463b`  
		Last Modified: Thu, 12 Jan 2023 03:48:06 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e467d553c4972b55bf8e3d80b16f245e5bb38f28d80b91ca4f9f90c09a6c28d`  
		Last Modified: Thu, 12 Jan 2023 03:48:05 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97054b77b205167acd5a303c8aa82e380f090ff4e2ded81d3425ec78500139d`  
		Last Modified: Thu, 12 Jan 2023 03:48:14 GMT  
		Size: 25.5 MB (25470784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e150d9e1a1da09e17313cb3b6358d2f16cf2919c51e9addf30500de9d03292ef`  
		Last Modified: Thu, 12 Jan 2023 03:48:03 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c0d792e2a7942826a61fdc26b6081ab404122751ff4f4dd8f5b8b0eca21399`  
		Last Modified: Thu, 12 Jan 2023 03:48:03 GMT  
		Size: 324.5 KB (324466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cdd2ff60bbafbd62e677e0798ee562e3c4b291b841c6d0904ca080220e132a`  
		Last Modified: Thu, 12 Jan 2023 03:52:14 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17e6f8c13d649cbaec88dcdd4b1de7b004cf19227fbb4f923bd031b6b57988f`  
		Last Modified: Thu, 12 Jan 2023 03:53:12 GMT  
		Size: 157.7 MB (157659743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29fbb32977b62254a5de7ced98fe2a21e0342aa9db7b3cf32be4013d96b2cd9`  
		Last Modified: Thu, 12 Jan 2023 03:52:14 GMT  
		Size: 1.6 KB (1563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2fbb7e05d875affd4596aa7b87572980a3ab74800cff17a34deb445bed71b8`  
		Last Modified: Thu, 12 Jan 2023 05:36:53 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edae42a55d8aaff06e33b6f9ac104d54771346e5f4f59afd8ce90c794716611a`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb86a1e32dd5f27c1ba5ed4c675ff8c1477230677af11f17c75379385bd990b4`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d846d73e8be9adf7269d7376adebc7a8e8706b560a5f0d67886ab98c1d00c233`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2d31296154ed152465faac00831500590d35be69015063bb3ae3cc3514575d`  
		Last Modified: Thu, 09 Feb 2023 01:17:38 GMT  
		Size: 1.7 MB (1653847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef57a9413d8bab4ab7212470d9ac2b9eafc5efb5dc44aef718c91f935daddce`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - windows version 10.0.20348.1487; amd64

```console
$ docker pull caddy@sha256:e288b33447f0b01c2ee0954c57e574b43ce9ed4b56cbd813eca3cb1df8d9f766
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1572061864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c236dcd08d81ed31367d57c62c7e77e2421092030cd5365c6a225b0ad121c6b5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 02:57:40 GMT
ENV GIT_VERSION=2.23.0
# Thu, 12 Jan 2023 02:57:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 12 Jan 2023 02:57:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 12 Jan 2023 02:57:42 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 12 Jan 2023 02:58:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 02:58:23 GMT
ENV GOPATH=C:\go
# Thu, 12 Jan 2023 02:58:47 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 Jan 2023 03:16:17 GMT
ENV GOLANG_VERSION=1.19.5
# Thu, 12 Jan 2023 03:19:43 GMT
RUN $url = 'https://dl.google.com/go/go1.19.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '167db91a2e40aeb453d3e59d213ecab06f62e1c4a84d13a06ccda1d999961caa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:19:45 GMT
WORKDIR C:\go
# Thu, 12 Jan 2023 05:34:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:20:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 00:20:47 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:20:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 00:21:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Feb 2023 00:21:22 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2fc8728d9c7bf65edf893fd902f8b1bd780f93623858960c9db79e39922b169`  
		Last Modified: Thu, 12 Jan 2023 03:47:24 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7935a4c648078e79f67a11bcd5908e251110dd6c5a4ee49a607f332dd25af9`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d257f8b122044547f89f00f58661b25aca97c92f3831e7aaa11975639b6e35d4`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95acaa75c1852ba1320c5db382b01f587badb615b6746b59be27eedcf96ab667`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5201ba65043fa621c187729f18aecf4c549cdfa12cd6d8cab7a901d893f3a8a8`  
		Last Modified: Thu, 12 Jan 2023 03:47:29 GMT  
		Size: 25.7 MB (25702230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a317a349bca5ab28ba7c1ce039928a56390f7e7a8d7ddec07efcc1c9883e5d`  
		Last Modified: Thu, 12 Jan 2023 03:47:18 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8850296b8fbb853a6eb6341f7484cd4bc622e9f679f12c4123eddf08b7f398fb`  
		Last Modified: Thu, 12 Jan 2023 03:47:18 GMT  
		Size: 554.2 KB (554212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80b3d62f45a345eaac7caba0cdc514011cc61ea8f9d7d7b82d1bd4f8f3dbea4`  
		Last Modified: Thu, 12 Jan 2023 03:50:53 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320dc1bc3ac081a72fbca97a699b20068d92c70b3caaec8ca53036ab37509933`  
		Last Modified: Thu, 12 Jan 2023 03:51:58 GMT  
		Size: 157.9 MB (157885976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230636fcbea662dc69129c73285f4376c0b83a3222e8d438ec859d14ee1201b8`  
		Last Modified: Thu, 12 Jan 2023 03:50:53 GMT  
		Size: 1.6 KB (1569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581e22afffddeddb0a4127481e5016946bd3f35379291c6bb1e3b85e92e7acef`  
		Last Modified: Thu, 12 Jan 2023 05:37:10 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13aaa30213dc8e6b5906114a862d8398ac157fd2f8c835767a058069f180a181`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b39a2446c556432e7503cc419fe42c4d14ff3fc744cf6d475136c5058bc18d6`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43ea60403f6819d31f67d7dc2d230def090cb6366c7cd272d99d8d06aac019d`  
		Last Modified: Thu, 09 Feb 2023 01:17:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5970b711fddee53f278567276c42d2b169c5286a5133ba48ce3a599b253b37ab`  
		Last Modified: Thu, 09 Feb 2023 01:17:55 GMT  
		Size: 1.9 MB (1871861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1270e653c78ffbadd8ab6379e16db4c45c20fb148d294ec9654f1d13367fea6`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder-alpine`

```console
$ docker pull caddy@sha256:e6c08f0694b44abd7ae623da15e368a4828a38cae59c041ab8f55c750fc66351
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
$ docker pull caddy@sha256:b86e1de154ca5d11618a408742e2b6f16f99e55cdc0ee97fe0965da9f1b1572f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131390128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:858147920561fe47255b181692d82558dbab931f4393f33ba8697b9c647f690e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:50:11 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:50:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:23 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:01 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:02 GMT
WORKDIR /go
# Thu, 09 Feb 2023 03:18:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 03:18:17 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 03:18:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 03:18:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 03:18:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f8637abd914a8a62416e027a351293d0472bc4b4f44383c6f425fd0e03861c`  
		Last Modified: Mon, 09 Jan 2023 17:56:43 GMT  
		Size: 284.8 KB (284814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48e7ca896ec974241d86439d34188186e085705e42d914d8b7757c27eea8613`  
		Last Modified: Wed, 11 Jan 2023 00:08:38 GMT  
		Size: 122.3 MB (122328552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f26d270037d8578282b40f86c0a1816fc5d034d6213f7dcab8440056a589309`  
		Last Modified: Wed, 11 Jan 2023 00:08:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807cf12e90d621962959f760ccbca1b77b95c6120884fefcc4385f12614f9e49`  
		Last Modified: Thu, 09 Feb 2023 03:18:55 GMT  
		Size: 4.2 MB (4187743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1e21e6198268a646e1f41d15b44931dc2d1ffaf7448588af3237d7443de8df`  
		Last Modified: Thu, 09 Feb 2023 03:18:54 GMT  
		Size: 1.2 MB (1217832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86c409f0ecb7b6ab12d691c73e32350f6453fc6e477af6fe53ec7946e91ec08`  
		Last Modified: Thu, 09 Feb 2023 03:18:54 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2d6f2baed8a8d6af9014cc57d9488335fd4d9ded609476ce98307a241b55f680
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127387922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad435c186a3c6ffdd4910420eabfef5bbf8a84e247d2473ac2c1394e5ece3781`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:28:28 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:28:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:57:48 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:48 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:49 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:49:43 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:49:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:49:44 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:49:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:49:45 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:49:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:49:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:49:47 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3919da799d44c7be2eecafbf780801f4cd562b289c55ebe566999525497cd24`  
		Last Modified: Mon, 09 Jan 2023 17:37:35 GMT  
		Size: 286.1 KB (286122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c266a9580739a5c56dffcd14ce61144c9f58539d8c927ccd3df332434ad8d57`  
		Last Modified: Wed, 11 Jan 2023 00:11:13 GMT  
		Size: 118.7 MB (118677328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9666a7ae960b29537b5e693ea358a6181a3b9b73110b1099f22596b2dedbe3bd`  
		Last Modified: Wed, 11 Jan 2023 00:10:50 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b71d65a08c2aecf44c515cedf0abefc5f896bd9942291a29ddcf6646452661`  
		Last Modified: Wed, 08 Feb 2023 23:50:58 GMT  
		Size: 4.2 MB (4150629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a427cd9f7efb7c150d196c96034cdc132bf3c26025a87378400da762842a4923`  
		Last Modified: Wed, 08 Feb 2023 23:50:57 GMT  
		Size: 1.2 MB (1166069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278f59186f97ea59dd8a5f727fe7b3e2aa46b384971583b5b277b871a61b2131`  
		Last Modified: Wed, 08 Feb 2023 23:50:57 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:ad4dce5e6c2c07e73c35c50cdc26e110c439a947f626c86482c0bc5165ad8d9e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126503260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be8c29fce7791d265104052e6900b3eca71a13aa0b77861ded3aac664b4e9ae7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:04:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 10 Jan 2023 01:04:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:59:19 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:02:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:02:06 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:02:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:02:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:02:08 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:57:41 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:57:42 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:57:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:57:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:57:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c7609f223a73f5c1097b3b7cb1ea29e1e540da920bc3b48b8672a1d5ef1dc9`  
		Last Modified: Tue, 10 Jan 2023 01:13:57 GMT  
		Size: 285.4 KB (285359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da97c3a81e19449c60385f1e4cf4fd4fc9ffd14d08a26ccb6782cafd2d5d6f66`  
		Last Modified: Wed, 11 Jan 2023 00:15:15 GMT  
		Size: 118.5 MB (118468701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e98750b6aa4570218317d53b00f803a47aff7219e78c594d1666eef08e0258`  
		Last Modified: Wed, 11 Jan 2023 00:14:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ffc027d61bfbcc1c13359e022e0e4e6a5ef7cf40c49a8979e7d2f2a40add601`  
		Last Modified: Wed, 08 Feb 2023 23:58:48 GMT  
		Size: 3.7 MB (3720136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c82d9a2e5d63888f8bbe98b76b4b3565ccc2c8ce45526e794fae5f54d98ba49`  
		Last Modified: Wed, 08 Feb 2023 23:58:48 GMT  
		Size: 1.2 MB (1163326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0730779ca73578c83a210e39877a270c4a66834bd12b23cf515389d07213ac72`  
		Last Modified: Wed, 08 Feb 2023 23:58:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:bddc4b456724f377099c6889de30e23e6b434d71153db528d9746fade979f0c8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125786646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4850c9ee7a87ef514c7c4e3c3773db8494849b1ba453095ffe6fc5df07f158b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:37:51 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:37:52 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:14 GMT
ENV GOLANG_VERSION=1.19.5
# Tue, 10 Jan 2023 23:59:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Jan 2023 23:59:24 GMT
ENV GOPATH=/go
# Tue, 10 Jan 2023 23:59:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:59:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 10 Jan 2023 23:59:25 GMT
WORKDIR /go
# Thu, 09 Feb 2023 03:57:02 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 03:57:02 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 03:57:03 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:57:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 03:57:03 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 03:57:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 03:57:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 03:57:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3aa66ae7ca151fbd33126b15fa4d01bd5ceb35d53de36a8c6c82ecde58b596`  
		Last Modified: Mon, 09 Jan 2023 17:42:45 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491d6e59a2be619159e6630fabdf81f0255c275176cd97d109fa2f417935d6a8`  
		Last Modified: Wed, 11 Jan 2023 00:06:29 GMT  
		Size: 116.9 MB (116882841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4d12be79e26ab534722d5e8e5c9d931ed5ebd84ded16cae4b12390bb543502`  
		Last Modified: Wed, 11 Jan 2023 00:06:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c89dffd73dee99c1e6d53d4ea8cc302fa2089ee3edef14dc51585b33986fc9`  
		Last Modified: Thu, 09 Feb 2023 03:57:40 GMT  
		Size: 4.2 MB (4234011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cfcadb2a14be80b0bad3d94a219fcb7e0889a821a54688bc4ca6f47b905d88`  
		Last Modified: Thu, 09 Feb 2023 03:57:39 GMT  
		Size: 1.1 MB (1123736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b4461ab8f854d2e2000cacc11f5ee723a0888222cbd031ae1d1f0ae14c3e94`  
		Last Modified: Thu, 09 Feb 2023 03:57:39 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:7805a8da1341b4d0a403cd79ce628ded1f59f183d0c9d1a736e8d898370ca860
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126524152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c705e4439b5eac8b98303529a2168b757e4fad96343a01659c151be8647f401f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:13 GMT
ADD file:9a1d27fdc0c915f387f2446c85193d5215b18020b313114f0bf2799efcc1baae in / 
# Mon, 09 Jan 2023 17:05:13 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:34:40 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 21:34:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:42 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:01:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:01:19 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:01:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:01:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:01:20 GMT
WORKDIR /go
# Thu, 09 Feb 2023 06:18:37 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 06:18:37 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 06:18:38 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 06:18:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 06:18:38 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 06:18:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 06:18:42 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 06:18:42 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f45bfda3aa14e255d9eb4c9a108eb3d8c6721946b4aa2e5808e5092242344a1c`  
		Last Modified: Mon, 09 Jan 2023 17:05:56 GMT  
		Size: 3.4 MB (3384562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ab1c47929aa42b49b577230cb740bcf3e8aebc5abb60aabb4e6ee296dc2cad`  
		Last Modified: Mon, 09 Jan 2023 21:44:30 GMT  
		Size: 286.6 KB (286647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ded0f2fb726423b204889105ff334f3133acd9bbd8a5edfddad43e6e904485`  
		Last Modified: Wed, 11 Jan 2023 00:14:05 GMT  
		Size: 117.3 MB (117267319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c616b872c15882d15d49d081ce173bb6fa4e0f36ffead4b1938923db8038bd`  
		Last Modified: Wed, 11 Jan 2023 00:13:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e47ce9bd35950f8803ed14aa1fe38b85865479ec312ffa8b32df18b26add09`  
		Last Modified: Thu, 09 Feb 2023 06:19:42 GMT  
		Size: 4.5 MB (4479174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e8d19e2da6aa4d4205abf9c47ab0c45f001d2f8af00e99eb2bd7fec2852519`  
		Last Modified: Thu, 09 Feb 2023 06:19:41 GMT  
		Size: 1.1 MB (1105889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb53e3916ae4f3ac3cd8e441e2276b18484cf30de7a4f7b9ccb908933cd7502a`  
		Last Modified: Thu, 09 Feb 2023 06:19:41 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:3fa0a9eed3f7aaac0dbb713789109e64e4a585c7a9293211ecacc1d944b973be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129575744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a22f7e76fad31ed672b8977ea04a84eb19571daac58c337bd73a5c173ceecc6b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:44 GMT
ADD file:eabe7c3c368e65478b53ac35c1daf3b703f2bca4ecdab2d080a65e8b981d7d4a in / 
# Mon, 09 Jan 2023 17:05:46 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:42:43 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:42:43 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:53 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:56 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:57 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:41:57 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:41:58 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:42:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:42:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:42:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ae982806674c51a962c0fdd6e19f464ebd673df529c5cfb7c1d049e0b618d384`  
		Last Modified: Mon, 09 Jan 2023 17:06:50 GMT  
		Size: 3.2 MB (3170744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a5579d5fa8a33df30a972596fba4f03e76edabd19e57e62163b9c717fc188f`  
		Last Modified: Mon, 09 Jan 2023 17:54:33 GMT  
		Size: 285.0 KB (285022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4535e632f08f4af238fcccc27545520d10696aa3ce5920e33ba5578c3ee0e23`  
		Last Modified: Wed, 11 Jan 2023 00:12:31 GMT  
		Size: 120.8 MB (120785530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7633b4de83c59883de617e4ab5c606af3c556d6de4e45337bc59bff5bf7fe8ee`  
		Last Modified: Wed, 11 Jan 2023 00:12:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54414a7d37854703b1d037b805f6d0a49d2d398794414e3cedd1507c4bff0b82`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 4.2 MB (4163474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1779d1179e942debc68a6641287b6503a7e6949318c9272acb0273d7947d66e7`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 1.2 MB (1170413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597462f6847e463140e07072d10801a4c80c146d229deb04ef5cbc8b6f043464`  
		Last Modified: Wed, 08 Feb 2023 23:42:50 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:4c57090f03b98d1a89618055d77e7e8864830bf83840fd17b1228bfa3cc8db4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `caddy:2.6-builder-windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull caddy@sha256:feeef34c537e9ea177fbaddb84e47df2e84a5cce70f7c8e3730e41822897b57e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1893070742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14ec5079fc868b1ce19abdcd6fca0964fae438be489b78914e21eac77dee89b3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 03:01:55 GMT
ENV GIT_VERSION=2.23.0
# Thu, 12 Jan 2023 03:01:56 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 12 Jan 2023 03:01:57 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 12 Jan 2023 03:01:58 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 12 Jan 2023 03:02:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:03:01 GMT
ENV GOPATH=C:\go
# Thu, 12 Jan 2023 03:03:35 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 Jan 2023 03:20:09 GMT
ENV GOLANG_VERSION=1.19.5
# Thu, 12 Jan 2023 03:23:52 GMT
RUN $url = 'https://dl.google.com/go/go1.19.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '167db91a2e40aeb453d3e59d213ecab06f62e1c4a84d13a06ccda1d999961caa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:23:54 GMT
WORKDIR C:\go
# Thu, 12 Jan 2023 05:33:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:19:59 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 00:20:00 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:20:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 00:20:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Feb 2023 00:20:35 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203425975bec1802428fad91a2e5f01172b161062c12eddf729e548bf7e134e0`  
		Last Modified: Thu, 12 Jan 2023 03:48:09 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80e42e19ab862b4adea06f1995e1f5cbb2c11ad8d68ae4a7bb5d0da5d0e6f38`  
		Last Modified: Thu, 12 Jan 2023 03:48:06 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be5d5df8cec6d1386f78a342668c3d2cb809372865459c1b35aa8d5a39a463b`  
		Last Modified: Thu, 12 Jan 2023 03:48:06 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e467d553c4972b55bf8e3d80b16f245e5bb38f28d80b91ca4f9f90c09a6c28d`  
		Last Modified: Thu, 12 Jan 2023 03:48:05 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97054b77b205167acd5a303c8aa82e380f090ff4e2ded81d3425ec78500139d`  
		Last Modified: Thu, 12 Jan 2023 03:48:14 GMT  
		Size: 25.5 MB (25470784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e150d9e1a1da09e17313cb3b6358d2f16cf2919c51e9addf30500de9d03292ef`  
		Last Modified: Thu, 12 Jan 2023 03:48:03 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c0d792e2a7942826a61fdc26b6081ab404122751ff4f4dd8f5b8b0eca21399`  
		Last Modified: Thu, 12 Jan 2023 03:48:03 GMT  
		Size: 324.5 KB (324466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cdd2ff60bbafbd62e677e0798ee562e3c4b291b841c6d0904ca080220e132a`  
		Last Modified: Thu, 12 Jan 2023 03:52:14 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17e6f8c13d649cbaec88dcdd4b1de7b004cf19227fbb4f923bd031b6b57988f`  
		Last Modified: Thu, 12 Jan 2023 03:53:12 GMT  
		Size: 157.7 MB (157659743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29fbb32977b62254a5de7ced98fe2a21e0342aa9db7b3cf32be4013d96b2cd9`  
		Last Modified: Thu, 12 Jan 2023 03:52:14 GMT  
		Size: 1.6 KB (1563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2fbb7e05d875affd4596aa7b87572980a3ab74800cff17a34deb445bed71b8`  
		Last Modified: Thu, 12 Jan 2023 05:36:53 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edae42a55d8aaff06e33b6f9ac104d54771346e5f4f59afd8ce90c794716611a`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb86a1e32dd5f27c1ba5ed4c675ff8c1477230677af11f17c75379385bd990b4`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d846d73e8be9adf7269d7376adebc7a8e8706b560a5f0d67886ab98c1d00c233`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2d31296154ed152465faac00831500590d35be69015063bb3ae3cc3514575d`  
		Last Modified: Thu, 09 Feb 2023 01:17:38 GMT  
		Size: 1.7 MB (1653847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef57a9413d8bab4ab7212470d9ac2b9eafc5efb5dc44aef718c91f935daddce`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:5016a9ee6f22300f4699ec2ba33c105b273e55c4b6931dcdbe8a7326d9dc037a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1487; amd64

### `caddy:2.6-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1487; amd64

```console
$ docker pull caddy@sha256:e288b33447f0b01c2ee0954c57e574b43ce9ed4b56cbd813eca3cb1df8d9f766
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1572061864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c236dcd08d81ed31367d57c62c7e77e2421092030cd5365c6a225b0ad121c6b5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 02:57:40 GMT
ENV GIT_VERSION=2.23.0
# Thu, 12 Jan 2023 02:57:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 12 Jan 2023 02:57:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 12 Jan 2023 02:57:42 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 12 Jan 2023 02:58:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 02:58:23 GMT
ENV GOPATH=C:\go
# Thu, 12 Jan 2023 02:58:47 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 Jan 2023 03:16:17 GMT
ENV GOLANG_VERSION=1.19.5
# Thu, 12 Jan 2023 03:19:43 GMT
RUN $url = 'https://dl.google.com/go/go1.19.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '167db91a2e40aeb453d3e59d213ecab06f62e1c4a84d13a06ccda1d999961caa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:19:45 GMT
WORKDIR C:\go
# Thu, 12 Jan 2023 05:34:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:20:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 00:20:47 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:20:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 00:21:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Feb 2023 00:21:22 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2fc8728d9c7bf65edf893fd902f8b1bd780f93623858960c9db79e39922b169`  
		Last Modified: Thu, 12 Jan 2023 03:47:24 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7935a4c648078e79f67a11bcd5908e251110dd6c5a4ee49a607f332dd25af9`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d257f8b122044547f89f00f58661b25aca97c92f3831e7aaa11975639b6e35d4`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95acaa75c1852ba1320c5db382b01f587badb615b6746b59be27eedcf96ab667`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5201ba65043fa621c187729f18aecf4c549cdfa12cd6d8cab7a901d893f3a8a8`  
		Last Modified: Thu, 12 Jan 2023 03:47:29 GMT  
		Size: 25.7 MB (25702230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a317a349bca5ab28ba7c1ce039928a56390f7e7a8d7ddec07efcc1c9883e5d`  
		Last Modified: Thu, 12 Jan 2023 03:47:18 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8850296b8fbb853a6eb6341f7484cd4bc622e9f679f12c4123eddf08b7f398fb`  
		Last Modified: Thu, 12 Jan 2023 03:47:18 GMT  
		Size: 554.2 KB (554212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80b3d62f45a345eaac7caba0cdc514011cc61ea8f9d7d7b82d1bd4f8f3dbea4`  
		Last Modified: Thu, 12 Jan 2023 03:50:53 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320dc1bc3ac081a72fbca97a699b20068d92c70b3caaec8ca53036ab37509933`  
		Last Modified: Thu, 12 Jan 2023 03:51:58 GMT  
		Size: 157.9 MB (157885976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230636fcbea662dc69129c73285f4376c0b83a3222e8d438ec859d14ee1201b8`  
		Last Modified: Thu, 12 Jan 2023 03:50:53 GMT  
		Size: 1.6 KB (1569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581e22afffddeddb0a4127481e5016946bd3f35379291c6bb1e3b85e92e7acef`  
		Last Modified: Thu, 12 Jan 2023 05:37:10 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13aaa30213dc8e6b5906114a862d8398ac157fd2f8c835767a058069f180a181`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b39a2446c556432e7503cc419fe42c4d14ff3fc744cf6d475136c5058bc18d6`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43ea60403f6819d31f67d7dc2d230def090cb6366c7cd272d99d8d06aac019d`  
		Last Modified: Thu, 09 Feb 2023 01:17:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5970b711fddee53f278567276c42d2b169c5286a5133ba48ce3a599b253b37ab`  
		Last Modified: Thu, 09 Feb 2023 01:17:55 GMT  
		Size: 1.9 MB (1871861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1270e653c78ffbadd8ab6379e16db4c45c20fb148d294ec9654f1d13367fea6`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-windowsservercore`

```console
$ docker pull caddy@sha256:0824e61dd8be6c1fa86bcf0faf1d4c5d8a41c047e0d4bf9ec8bbb73f243adaf6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3887; amd64
	-	windows version 10.0.20348.1487; amd64

### `caddy:2.6-windowsservercore` - windows version 10.0.17763.3887; amd64

```console
$ docker pull caddy@sha256:935d1f4349cc551dfe9b76d6ba5fe6355414519a3037a7689fe765033ae8dcd6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1723388621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1deb1aecac8501d9afe22abd2fc90f15552c63366f8016ad2e6d1602be5cdf6d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:16:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:16:36 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:17:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:17:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:17:21 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:17:22 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:17:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:17:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:17:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:17:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:17:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:17:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:17:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:17:31 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:17:32 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:17:33 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:17:34 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:17:53 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:17:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47af8a9c9ef8e49d65e53dd207ad0935ce7a2b50b2f253e6a5b037494ae19d0a`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 401.5 KB (401472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5841cb6343add9dd7b89906610425117976b050c0634eedbc5c38302aa024e`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d760049e5c9f1fb1d7ec05a3eea55088808f484912e87cda07f3709363fe3c2c`  
		Last Modified: Thu, 09 Feb 2023 01:16:53 GMT  
		Size: 14.7 MB (14680484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3239225b5bad52e6004b638bd356e7d29e7fded5d31d90541907e1a769a115`  
		Last Modified: Thu, 09 Feb 2023 01:16:49 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6823ad091829bc6d98a58a18b075e20c551bde81d504bdbfda09b5a3d7c5d0`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4873a8802163accb90dd2318bd05ddfa4f94692b2731d6e23095e3bb46b98fd`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabf39e152fd5c18e0c3ac503e054c36e2775512f9fa7bb11b9221442b2bc1fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af12dc4018ba87a8e25003874e2d8e959a25b1c19932553daec8f4c410ebd61f`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fefa1f82e39e2af863b13609d78d966746d852af0cea54dcb17f45a8386c39d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d5b41708aea61714f00bc0f35ea1efc60db85c04ab6754e4d6b4485dc59a28`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a8b1cf8bcc4175323f7feaa280e3122f03aa7f9d35666fcc55c6b7d1e628ae`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c3f865e552649c436d5ffc0f3c83a3b5ba3026b2cff2ab3f381a5cdf2e2f2`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201cfdbfc1583e2ea070418e6aad0ec6604fb52c68117460b1a4c5b511b56ecc`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef83199fb67566ea043dbf7fab6f54754a4d0496655be1157819973573247bb`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45db789a3d9786dea133341e2c9f16e14b23a664297ad7f9a371961a0c21588`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a4e021c112717a1fee7cd62cdc17d41521f3514f10bf8ec30457b95aaf44fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4c0327054bc1f199339822d4074ee176c4184b9357ec28d9250f27f0c12e26`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63a4d912695117a127068d20ceefbaa19e41c8a42d65788d37915d737d998d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:44 GMT  
		Size: 338.6 KB (338620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421719fbbf536a3651d6762e36406f19dd0b5601f4a300d9c47af9ccfa3573d2`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-windowsservercore` - windows version 10.0.20348.1487; amd64

```console
$ docker pull caddy@sha256:22cdfda624195707c05f1d681c1cdd97b504f06b282d981718e1b716b2dc6bfb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1401937005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca7c6af6ec202266d95f15726fee733430a631c6c4eddfd9cc7d000b817a0f19`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:18:43 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:18:44 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:19:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:19:16 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:19:17 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:19:18 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:19:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:19:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:19:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:19:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:19:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:19:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:19:26 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:19:27 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:19:29 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:19:30 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:19:47 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:19:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42eb48143612ee855d99c932e324b1bd035c60554117edeaa805402060613c51`  
		Last Modified: Thu, 09 Feb 2023 01:17:17 GMT  
		Size: 635.9 KB (635943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714ae92cb5dac0e72097d35b932125b5ea3f03214de78e03119a4517be6fd10`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a5533d3ddbff5ea35dbb0e11b10fe817ce3ef1a3fd7f44706cb1b6288e0406`  
		Last Modified: Thu, 09 Feb 2023 01:17:20 GMT  
		Size: 14.9 MB (14899830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e59c8f0dc8d987210bdfe89eaded536b0ef8ac727eb7d75b76aea9c296208a`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22bfc3588219a43ce294aab21751b407ae75504bf3ddcee69f42498672b6c46`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f7db57dc0a0b0126433f60d3d0005f9aaa0d405fe63cfc3b4e15388fdfa010`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7b9e3a2510b5ab3b7ac4103d653c8efd12e95b63327d5c5fb81b6ea341e2b5`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4109b3b0ca73b5355a12ee74b7c32b4015a6208fdb279fd0ab60074247e22309`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3c568a1866d44483984b2be40142a55371adf3b8dc991bdb5ab4c45c0be3d4`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6221c7c14444b318e798e231adeeb83ea155c157283e9def018c43415238aa7`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e81980463382095586f78276db5cd808400136543fc1a0f522af1f3eaee034`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f0d8afe85320b7cf4542ad649671660bbb8e74ec3ad3067408e79fb21dbf77`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7def0e2b3dd94a350c82bb6a4903fdfc65d1d3d9772dd8195a5eb14ba766c45`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0b51c8090bf08cc2ae3a9fc340c9b70ba1e077f32b7d7d025b7d9fb472d978`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3653016f515e293fc93892b9e021e05a6a183ad3dcdaf243311513e222534c7`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d1dafd3fbb7403b7f093ed63553863bd9904f6010b1b91f98d9bfba9c4d8bb`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92817327253aaae4d632a75ff38a01dbebfe11f9105c4db828c52f221262ce4`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43bce457643a143e82e49e57d9b8a69a416e254d2439f30d7e4dd25c84e43c0`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 348.1 KB (348138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a0e899ab4c995de79522a5022b8cca4765559a4de2d5c728821d947b497de1`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-windowsservercore-1809`

```console
$ docker pull caddy@sha256:6fc3086452e6c85e993bf4b4834c55848a3977b547662cd4ce9fc98a17a495e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `caddy:2.6-windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull caddy@sha256:935d1f4349cc551dfe9b76d6ba5fe6355414519a3037a7689fe765033ae8dcd6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1723388621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1deb1aecac8501d9afe22abd2fc90f15552c63366f8016ad2e6d1602be5cdf6d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:16:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:16:36 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:17:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:17:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:17:21 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:17:22 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:17:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:17:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:17:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:17:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:17:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:17:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:17:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:17:31 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:17:32 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:17:33 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:17:34 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:17:53 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:17:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47af8a9c9ef8e49d65e53dd207ad0935ce7a2b50b2f253e6a5b037494ae19d0a`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 401.5 KB (401472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5841cb6343add9dd7b89906610425117976b050c0634eedbc5c38302aa024e`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d760049e5c9f1fb1d7ec05a3eea55088808f484912e87cda07f3709363fe3c2c`  
		Last Modified: Thu, 09 Feb 2023 01:16:53 GMT  
		Size: 14.7 MB (14680484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3239225b5bad52e6004b638bd356e7d29e7fded5d31d90541907e1a769a115`  
		Last Modified: Thu, 09 Feb 2023 01:16:49 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6823ad091829bc6d98a58a18b075e20c551bde81d504bdbfda09b5a3d7c5d0`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4873a8802163accb90dd2318bd05ddfa4f94692b2731d6e23095e3bb46b98fd`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabf39e152fd5c18e0c3ac503e054c36e2775512f9fa7bb11b9221442b2bc1fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af12dc4018ba87a8e25003874e2d8e959a25b1c19932553daec8f4c410ebd61f`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fefa1f82e39e2af863b13609d78d966746d852af0cea54dcb17f45a8386c39d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d5b41708aea61714f00bc0f35ea1efc60db85c04ab6754e4d6b4485dc59a28`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a8b1cf8bcc4175323f7feaa280e3122f03aa7f9d35666fcc55c6b7d1e628ae`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c3f865e552649c436d5ffc0f3c83a3b5ba3026b2cff2ab3f381a5cdf2e2f2`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201cfdbfc1583e2ea070418e6aad0ec6604fb52c68117460b1a4c5b511b56ecc`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef83199fb67566ea043dbf7fab6f54754a4d0496655be1157819973573247bb`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45db789a3d9786dea133341e2c9f16e14b23a664297ad7f9a371961a0c21588`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a4e021c112717a1fee7cd62cdc17d41521f3514f10bf8ec30457b95aaf44fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4c0327054bc1f199339822d4074ee176c4184b9357ec28d9250f27f0c12e26`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63a4d912695117a127068d20ceefbaa19e41c8a42d65788d37915d737d998d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:44 GMT  
		Size: 338.6 KB (338620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421719fbbf536a3651d6762e36406f19dd0b5601f4a300d9c47af9ccfa3573d2`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:65b3d9f69c1f9e10dae44434f033715465a5e5331b38550f4f47baa12a60a39c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1487; amd64

### `caddy:2.6-windowsservercore-ltsc2022` - windows version 10.0.20348.1487; amd64

```console
$ docker pull caddy@sha256:22cdfda624195707c05f1d681c1cdd97b504f06b282d981718e1b716b2dc6bfb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1401937005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca7c6af6ec202266d95f15726fee733430a631c6c4eddfd9cc7d000b817a0f19`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:18:43 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:18:44 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:19:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:19:16 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:19:17 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:19:18 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:19:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:19:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:19:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:19:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:19:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:19:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:19:26 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:19:27 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:19:29 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:19:30 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:19:47 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:19:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42eb48143612ee855d99c932e324b1bd035c60554117edeaa805402060613c51`  
		Last Modified: Thu, 09 Feb 2023 01:17:17 GMT  
		Size: 635.9 KB (635943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714ae92cb5dac0e72097d35b932125b5ea3f03214de78e03119a4517be6fd10`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a5533d3ddbff5ea35dbb0e11b10fe817ce3ef1a3fd7f44706cb1b6288e0406`  
		Last Modified: Thu, 09 Feb 2023 01:17:20 GMT  
		Size: 14.9 MB (14899830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e59c8f0dc8d987210bdfe89eaded536b0ef8ac727eb7d75b76aea9c296208a`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22bfc3588219a43ce294aab21751b407ae75504bf3ddcee69f42498672b6c46`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f7db57dc0a0b0126433f60d3d0005f9aaa0d405fe63cfc3b4e15388fdfa010`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7b9e3a2510b5ab3b7ac4103d653c8efd12e95b63327d5c5fb81b6ea341e2b5`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4109b3b0ca73b5355a12ee74b7c32b4015a6208fdb279fd0ab60074247e22309`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3c568a1866d44483984b2be40142a55371adf3b8dc991bdb5ab4c45c0be3d4`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6221c7c14444b318e798e231adeeb83ea155c157283e9def018c43415238aa7`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e81980463382095586f78276db5cd808400136543fc1a0f522af1f3eaee034`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f0d8afe85320b7cf4542ad649671660bbb8e74ec3ad3067408e79fb21dbf77`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7def0e2b3dd94a350c82bb6a4903fdfc65d1d3d9772dd8195a5eb14ba766c45`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0b51c8090bf08cc2ae3a9fc340c9b70ba1e077f32b7d7d025b7d9fb472d978`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3653016f515e293fc93892b9e021e05a6a183ad3dcdaf243311513e222534c7`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d1dafd3fbb7403b7f093ed63553863bd9904f6010b1b91f98d9bfba9c4d8bb`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92817327253aaae4d632a75ff38a01dbebfe11f9105c4db828c52f221262ce4`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43bce457643a143e82e49e57d9b8a69a416e254d2439f30d7e4dd25c84e43c0`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 348.1 KB (348138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a0e899ab4c995de79522a5022b8cca4765559a4de2d5c728821d947b497de1`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.3`

```console
$ docker pull caddy@sha256:d34a689107f831d1fb6dfb92ce4cff1569e409e5b6dcd2d671d4ffee8b112b76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3887; amd64
	-	windows version 10.0.20348.1487; amd64

### `caddy:2.6.3` - linux; amd64

```console
$ docker pull caddy@sha256:cf66a65d5667b26ba91fab680b59d421266e5042d4191fcdeab3847b31828bf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17441779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:739163e8bd53961abf96cc4f327498332dd905a59d3314fab80a845e62b58f9b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Thu, 09 Feb 2023 03:18:05 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 09 Feb 2023 03:18:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 09 Feb 2023 03:18:06 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:18:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 09 Feb 2023 03:18:10 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 09 Feb 2023 03:18:10 GMT
ENV XDG_DATA_HOME=/data
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 80
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 443
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 03:18:11 GMT
WORKDIR /srv
# Thu, 09 Feb 2023 03:18:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4cf81513fab9758787dbde95dcab4c054bd04137581b68097595a719ae973c`  
		Last Modified: Thu, 09 Feb 2023 03:18:39 GMT  
		Size: 351.2 KB (351181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c3f44eb3bccaf2f5515331e12d4b940a5f6ad016d27f548e0c739d1f6aba66`  
		Last Modified: Thu, 09 Feb 2023 03:18:39 GMT  
		Size: 7.6 KB (7554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04314ed686e612bbb7606d6bacff938564f9b4f7e0dbc72afacd887b3c88afbd`  
		Last Modified: Thu, 09 Feb 2023 03:18:42 GMT  
		Size: 14.3 MB (14276772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e4444abb42ab384f9685f3b25765ed65d8e07daef954ccf7aa73a524a2177064
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16576623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99391525993d815548f2a8e80455bb1ff1b6dd0a769a0dc2a467cbcc3adbc1ad`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:32 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Fri, 10 Feb 2023 20:49:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:28:54 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 21:28:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Fri, 10 Feb 2023 21:28:56 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 21:28:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 21:28:59 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 21:28:59 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 80
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 443
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 21:29:00 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 21:29:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a400dcba29ff44f8e5bf01493def4f19629aca6d103cb2a66ca87c457f7414`  
		Last Modified: Fri, 10 Feb 2023 21:29:47 GMT  
		Size: 345.8 KB (345811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b946768825eb5ed2fc6f932fdb0b0c552f4c35c39dada07eddd70ce4a535953`  
		Last Modified: Fri, 10 Feb 2023 21:29:47 GMT  
		Size: 7.5 KB (7480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda323f820516b366c61a02ba4cfd00cc3a3b6cc9051c58e7359057dea842d8a`  
		Last Modified: Fri, 10 Feb 2023 21:29:51 GMT  
		Size: 13.6 MB (13606554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0a66f97fe167ebcccd1754f2cc7ed8d5f42595f332f60d75e4efd33c5fa880b9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16362110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0940efa30038d45d9b6cbae2aea1235accdd5e653948a6e40e9c3edf6314d4c6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:37:19 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:37:22 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Fri, 10 Feb 2023 22:37:22 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:37:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:37:26 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:37:27 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:37:27 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:37:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:37:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:37:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:37:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:37:30 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:37:30 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:37:31 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:37:31 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:37:31 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:37:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec2ab4edb1f0a14b28a55f050d62d8e54111075639a0fa8f173448814ba0d00`  
		Last Modified: Fri, 10 Feb 2023 22:38:25 GMT  
		Size: 342.6 KB (342588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0580184dd0082f009564a7a3923731f202cbe4bd8b857dbca2c77da8e7434815`  
		Last Modified: Fri, 10 Feb 2023 22:38:25 GMT  
		Size: 7.5 KB (7479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b2a44f2792add2104a1d53c68f1df95779deaee3ec86717f4fb4efd9aa6aaa`  
		Last Modified: Fri, 10 Feb 2023 22:38:28 GMT  
		Size: 13.6 MB (13591549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:4be5e6cdfb930681cc9c4722b0af67e75e53f0cff56c916c1d618eb39d6f5169
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16126925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:995c31e78c533c3ca73152cb87130dfcb16842dd052ab384df917fb755c5dc43`
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
# Fri, 10 Feb 2023 22:00:37 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:00:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:00:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:00:39 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:00:40 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:00:40 GMT
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
	-	`sha256:6403d7bb9250089f4077bba7631d975f97648fbcd782c992704ff3bccc5ae421`  
		Last Modified: Fri, 10 Feb 2023 22:01:03 GMT  
		Size: 13.1 MB (13059715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3` - linux; ppc64le

```console
$ docker pull caddy@sha256:50a289625f0ef1adfc05773b5ec8a30f001be347a84f24e1106e351f230758b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15949909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b11b3ee451004883e1f9089fc132ee1ecc849a2d96ef0ff4731334c8279cfa`
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
# Fri, 10 Feb 2023 22:13:23 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:13:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:13:28 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:13:28 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:13:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:13:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:13:33 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:13:33 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:13:33 GMT
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
	-	`sha256:2ecc7ec17344834a2337d83b9b7be44f97f0c0b55dfea5e1d8af80c8d5c32221`  
		Last Modified: Fri, 10 Feb 2023 22:14:19 GMT  
		Size: 12.8 MB (12774635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3` - linux; s390x

```console
$ docker pull caddy@sha256:9c69a670bfaa4e7166553c41a7303b114a524eed38924ad0d1d5599e6b7b2463
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16787086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9abb18c28ea7e824ff4385016f24b30d1a455d1b902f8667a1a9300078826a`
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
# Fri, 10 Feb 2023 22:14:19 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:14:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:14:21 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:14:22 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:14:23 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:14:23 GMT
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
	-	`sha256:94fd73a8831c9e57fdf8c430154c9adc56e54610a462128c8f0a1b3937aef704`  
		Last Modified: Fri, 10 Feb 2023 22:15:07 GMT  
		Size: 13.8 MB (13833147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3` - windows version 10.0.17763.3887; amd64

```console
$ docker pull caddy@sha256:935d1f4349cc551dfe9b76d6ba5fe6355414519a3037a7689fe765033ae8dcd6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1723388621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1deb1aecac8501d9afe22abd2fc90f15552c63366f8016ad2e6d1602be5cdf6d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:16:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:16:36 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:17:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:17:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:17:21 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:17:22 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:17:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:17:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:17:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:17:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:17:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:17:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:17:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:17:31 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:17:32 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:17:33 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:17:34 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:17:53 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:17:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47af8a9c9ef8e49d65e53dd207ad0935ce7a2b50b2f253e6a5b037494ae19d0a`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 401.5 KB (401472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5841cb6343add9dd7b89906610425117976b050c0634eedbc5c38302aa024e`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d760049e5c9f1fb1d7ec05a3eea55088808f484912e87cda07f3709363fe3c2c`  
		Last Modified: Thu, 09 Feb 2023 01:16:53 GMT  
		Size: 14.7 MB (14680484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3239225b5bad52e6004b638bd356e7d29e7fded5d31d90541907e1a769a115`  
		Last Modified: Thu, 09 Feb 2023 01:16:49 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6823ad091829bc6d98a58a18b075e20c551bde81d504bdbfda09b5a3d7c5d0`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4873a8802163accb90dd2318bd05ddfa4f94692b2731d6e23095e3bb46b98fd`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabf39e152fd5c18e0c3ac503e054c36e2775512f9fa7bb11b9221442b2bc1fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af12dc4018ba87a8e25003874e2d8e959a25b1c19932553daec8f4c410ebd61f`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fefa1f82e39e2af863b13609d78d966746d852af0cea54dcb17f45a8386c39d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d5b41708aea61714f00bc0f35ea1efc60db85c04ab6754e4d6b4485dc59a28`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a8b1cf8bcc4175323f7feaa280e3122f03aa7f9d35666fcc55c6b7d1e628ae`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c3f865e552649c436d5ffc0f3c83a3b5ba3026b2cff2ab3f381a5cdf2e2f2`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201cfdbfc1583e2ea070418e6aad0ec6604fb52c68117460b1a4c5b511b56ecc`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef83199fb67566ea043dbf7fab6f54754a4d0496655be1157819973573247bb`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45db789a3d9786dea133341e2c9f16e14b23a664297ad7f9a371961a0c21588`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a4e021c112717a1fee7cd62cdc17d41521f3514f10bf8ec30457b95aaf44fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4c0327054bc1f199339822d4074ee176c4184b9357ec28d9250f27f0c12e26`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63a4d912695117a127068d20ceefbaa19e41c8a42d65788d37915d737d998d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:44 GMT  
		Size: 338.6 KB (338620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421719fbbf536a3651d6762e36406f19dd0b5601f4a300d9c47af9ccfa3573d2`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3` - windows version 10.0.20348.1487; amd64

```console
$ docker pull caddy@sha256:22cdfda624195707c05f1d681c1cdd97b504f06b282d981718e1b716b2dc6bfb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1401937005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca7c6af6ec202266d95f15726fee733430a631c6c4eddfd9cc7d000b817a0f19`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:18:43 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:18:44 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:19:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:19:16 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:19:17 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:19:18 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:19:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:19:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:19:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:19:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:19:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:19:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:19:26 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:19:27 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:19:29 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:19:30 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:19:47 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:19:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42eb48143612ee855d99c932e324b1bd035c60554117edeaa805402060613c51`  
		Last Modified: Thu, 09 Feb 2023 01:17:17 GMT  
		Size: 635.9 KB (635943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714ae92cb5dac0e72097d35b932125b5ea3f03214de78e03119a4517be6fd10`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a5533d3ddbff5ea35dbb0e11b10fe817ce3ef1a3fd7f44706cb1b6288e0406`  
		Last Modified: Thu, 09 Feb 2023 01:17:20 GMT  
		Size: 14.9 MB (14899830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e59c8f0dc8d987210bdfe89eaded536b0ef8ac727eb7d75b76aea9c296208a`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22bfc3588219a43ce294aab21751b407ae75504bf3ddcee69f42498672b6c46`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f7db57dc0a0b0126433f60d3d0005f9aaa0d405fe63cfc3b4e15388fdfa010`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7b9e3a2510b5ab3b7ac4103d653c8efd12e95b63327d5c5fb81b6ea341e2b5`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4109b3b0ca73b5355a12ee74b7c32b4015a6208fdb279fd0ab60074247e22309`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3c568a1866d44483984b2be40142a55371adf3b8dc991bdb5ab4c45c0be3d4`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6221c7c14444b318e798e231adeeb83ea155c157283e9def018c43415238aa7`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e81980463382095586f78276db5cd808400136543fc1a0f522af1f3eaee034`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f0d8afe85320b7cf4542ad649671660bbb8e74ec3ad3067408e79fb21dbf77`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7def0e2b3dd94a350c82bb6a4903fdfc65d1d3d9772dd8195a5eb14ba766c45`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0b51c8090bf08cc2ae3a9fc340c9b70ba1e077f32b7d7d025b7d9fb472d978`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3653016f515e293fc93892b9e021e05a6a183ad3dcdaf243311513e222534c7`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d1dafd3fbb7403b7f093ed63553863bd9904f6010b1b91f98d9bfba9c4d8bb`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92817327253aaae4d632a75ff38a01dbebfe11f9105c4db828c52f221262ce4`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43bce457643a143e82e49e57d9b8a69a416e254d2439f30d7e4dd25c84e43c0`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 348.1 KB (348138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a0e899ab4c995de79522a5022b8cca4765559a4de2d5c728821d947b497de1`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.3-alpine`

```console
$ docker pull caddy@sha256:7e7286bb77df853f278887dd9159bd643abca8447ad4a0fddb4c48ec00a7e6cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.6.3-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:cf66a65d5667b26ba91fab680b59d421266e5042d4191fcdeab3847b31828bf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17441779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:739163e8bd53961abf96cc4f327498332dd905a59d3314fab80a845e62b58f9b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Thu, 09 Feb 2023 03:18:05 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 09 Feb 2023 03:18:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 09 Feb 2023 03:18:06 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:18:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 09 Feb 2023 03:18:10 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 09 Feb 2023 03:18:10 GMT
ENV XDG_DATA_HOME=/data
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 80
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 443
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 03:18:11 GMT
WORKDIR /srv
# Thu, 09 Feb 2023 03:18:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4cf81513fab9758787dbde95dcab4c054bd04137581b68097595a719ae973c`  
		Last Modified: Thu, 09 Feb 2023 03:18:39 GMT  
		Size: 351.2 KB (351181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c3f44eb3bccaf2f5515331e12d4b940a5f6ad016d27f548e0c739d1f6aba66`  
		Last Modified: Thu, 09 Feb 2023 03:18:39 GMT  
		Size: 7.6 KB (7554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04314ed686e612bbb7606d6bacff938564f9b4f7e0dbc72afacd887b3c88afbd`  
		Last Modified: Thu, 09 Feb 2023 03:18:42 GMT  
		Size: 14.3 MB (14276772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e4444abb42ab384f9685f3b25765ed65d8e07daef954ccf7aa73a524a2177064
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16576623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99391525993d815548f2a8e80455bb1ff1b6dd0a769a0dc2a467cbcc3adbc1ad`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:32 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Fri, 10 Feb 2023 20:49:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:28:54 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 21:28:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Fri, 10 Feb 2023 21:28:56 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 21:28:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 21:28:59 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 21:28:59 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 80
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 443
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 21:29:00 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 21:29:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a400dcba29ff44f8e5bf01493def4f19629aca6d103cb2a66ca87c457f7414`  
		Last Modified: Fri, 10 Feb 2023 21:29:47 GMT  
		Size: 345.8 KB (345811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b946768825eb5ed2fc6f932fdb0b0c552f4c35c39dada07eddd70ce4a535953`  
		Last Modified: Fri, 10 Feb 2023 21:29:47 GMT  
		Size: 7.5 KB (7480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda323f820516b366c61a02ba4cfd00cc3a3b6cc9051c58e7359057dea842d8a`  
		Last Modified: Fri, 10 Feb 2023 21:29:51 GMT  
		Size: 13.6 MB (13606554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0a66f97fe167ebcccd1754f2cc7ed8d5f42595f332f60d75e4efd33c5fa880b9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16362110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0940efa30038d45d9b6cbae2aea1235accdd5e653948a6e40e9c3edf6314d4c6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:37:19 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:37:22 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Fri, 10 Feb 2023 22:37:22 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:37:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:37:26 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:37:27 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:37:27 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:37:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:37:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:37:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:37:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:37:30 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:37:30 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:37:31 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:37:31 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:37:31 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:37:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec2ab4edb1f0a14b28a55f050d62d8e54111075639a0fa8f173448814ba0d00`  
		Last Modified: Fri, 10 Feb 2023 22:38:25 GMT  
		Size: 342.6 KB (342588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0580184dd0082f009564a7a3923731f202cbe4bd8b857dbca2c77da8e7434815`  
		Last Modified: Fri, 10 Feb 2023 22:38:25 GMT  
		Size: 7.5 KB (7479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b2a44f2792add2104a1d53c68f1df95779deaee3ec86717f4fb4efd9aa6aaa`  
		Last Modified: Fri, 10 Feb 2023 22:38:28 GMT  
		Size: 13.6 MB (13591549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:4be5e6cdfb930681cc9c4722b0af67e75e53f0cff56c916c1d618eb39d6f5169
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16126925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:995c31e78c533c3ca73152cb87130dfcb16842dd052ab384df917fb755c5dc43`
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
# Fri, 10 Feb 2023 22:00:37 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:00:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:00:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:00:39 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:00:40 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:00:40 GMT
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
	-	`sha256:6403d7bb9250089f4077bba7631d975f97648fbcd782c992704ff3bccc5ae421`  
		Last Modified: Fri, 10 Feb 2023 22:01:03 GMT  
		Size: 13.1 MB (13059715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:50a289625f0ef1adfc05773b5ec8a30f001be347a84f24e1106e351f230758b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15949909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b11b3ee451004883e1f9089fc132ee1ecc849a2d96ef0ff4731334c8279cfa`
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
# Fri, 10 Feb 2023 22:13:23 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:13:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:13:28 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:13:28 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:13:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:13:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:13:33 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:13:33 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:13:33 GMT
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
	-	`sha256:2ecc7ec17344834a2337d83b9b7be44f97f0c0b55dfea5e1d8af80c8d5c32221`  
		Last Modified: Fri, 10 Feb 2023 22:14:19 GMT  
		Size: 12.8 MB (12774635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:9c69a670bfaa4e7166553c41a7303b114a524eed38924ad0d1d5599e6b7b2463
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16787086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9abb18c28ea7e824ff4385016f24b30d1a455d1b902f8667a1a9300078826a`
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
# Fri, 10 Feb 2023 22:14:19 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:14:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:14:21 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:14:22 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:14:23 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:14:23 GMT
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
	-	`sha256:94fd73a8831c9e57fdf8c430154c9adc56e54610a462128c8f0a1b3937aef704`  
		Last Modified: Fri, 10 Feb 2023 22:15:07 GMT  
		Size: 13.8 MB (13833147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.3-builder`

```console
$ docker pull caddy@sha256:458901eb7e2d1f60ea430e23833e47d4b3ada93d601df57a34674b67675483b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3887; amd64
	-	windows version 10.0.20348.1487; amd64

### `caddy:2.6.3-builder` - linux; amd64

```console
$ docker pull caddy@sha256:b86e1de154ca5d11618a408742e2b6f16f99e55cdc0ee97fe0965da9f1b1572f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131390128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:858147920561fe47255b181692d82558dbab931f4393f33ba8697b9c647f690e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:50:11 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:50:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:23 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:01 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:02 GMT
WORKDIR /go
# Thu, 09 Feb 2023 03:18:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 03:18:17 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 03:18:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 03:18:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 03:18:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f8637abd914a8a62416e027a351293d0472bc4b4f44383c6f425fd0e03861c`  
		Last Modified: Mon, 09 Jan 2023 17:56:43 GMT  
		Size: 284.8 KB (284814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48e7ca896ec974241d86439d34188186e085705e42d914d8b7757c27eea8613`  
		Last Modified: Wed, 11 Jan 2023 00:08:38 GMT  
		Size: 122.3 MB (122328552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f26d270037d8578282b40f86c0a1816fc5d034d6213f7dcab8440056a589309`  
		Last Modified: Wed, 11 Jan 2023 00:08:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807cf12e90d621962959f760ccbca1b77b95c6120884fefcc4385f12614f9e49`  
		Last Modified: Thu, 09 Feb 2023 03:18:55 GMT  
		Size: 4.2 MB (4187743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1e21e6198268a646e1f41d15b44931dc2d1ffaf7448588af3237d7443de8df`  
		Last Modified: Thu, 09 Feb 2023 03:18:54 GMT  
		Size: 1.2 MB (1217832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86c409f0ecb7b6ab12d691c73e32350f6453fc6e477af6fe53ec7946e91ec08`  
		Last Modified: Thu, 09 Feb 2023 03:18:54 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2d6f2baed8a8d6af9014cc57d9488335fd4d9ded609476ce98307a241b55f680
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127387922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad435c186a3c6ffdd4910420eabfef5bbf8a84e247d2473ac2c1394e5ece3781`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:28:28 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:28:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:57:48 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:48 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:49 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:49:43 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:49:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:49:44 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:49:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:49:45 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:49:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:49:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:49:47 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3919da799d44c7be2eecafbf780801f4cd562b289c55ebe566999525497cd24`  
		Last Modified: Mon, 09 Jan 2023 17:37:35 GMT  
		Size: 286.1 KB (286122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c266a9580739a5c56dffcd14ce61144c9f58539d8c927ccd3df332434ad8d57`  
		Last Modified: Wed, 11 Jan 2023 00:11:13 GMT  
		Size: 118.7 MB (118677328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9666a7ae960b29537b5e693ea358a6181a3b9b73110b1099f22596b2dedbe3bd`  
		Last Modified: Wed, 11 Jan 2023 00:10:50 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b71d65a08c2aecf44c515cedf0abefc5f896bd9942291a29ddcf6646452661`  
		Last Modified: Wed, 08 Feb 2023 23:50:58 GMT  
		Size: 4.2 MB (4150629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a427cd9f7efb7c150d196c96034cdc132bf3c26025a87378400da762842a4923`  
		Last Modified: Wed, 08 Feb 2023 23:50:57 GMT  
		Size: 1.2 MB (1166069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278f59186f97ea59dd8a5f727fe7b3e2aa46b384971583b5b277b871a61b2131`  
		Last Modified: Wed, 08 Feb 2023 23:50:57 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:ad4dce5e6c2c07e73c35c50cdc26e110c439a947f626c86482c0bc5165ad8d9e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126503260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be8c29fce7791d265104052e6900b3eca71a13aa0b77861ded3aac664b4e9ae7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:04:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 10 Jan 2023 01:04:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:59:19 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:02:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:02:06 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:02:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:02:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:02:08 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:57:41 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:57:42 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:57:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:57:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:57:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c7609f223a73f5c1097b3b7cb1ea29e1e540da920bc3b48b8672a1d5ef1dc9`  
		Last Modified: Tue, 10 Jan 2023 01:13:57 GMT  
		Size: 285.4 KB (285359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da97c3a81e19449c60385f1e4cf4fd4fc9ffd14d08a26ccb6782cafd2d5d6f66`  
		Last Modified: Wed, 11 Jan 2023 00:15:15 GMT  
		Size: 118.5 MB (118468701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e98750b6aa4570218317d53b00f803a47aff7219e78c594d1666eef08e0258`  
		Last Modified: Wed, 11 Jan 2023 00:14:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ffc027d61bfbcc1c13359e022e0e4e6a5ef7cf40c49a8979e7d2f2a40add601`  
		Last Modified: Wed, 08 Feb 2023 23:58:48 GMT  
		Size: 3.7 MB (3720136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c82d9a2e5d63888f8bbe98b76b4b3565ccc2c8ce45526e794fae5f54d98ba49`  
		Last Modified: Wed, 08 Feb 2023 23:58:48 GMT  
		Size: 1.2 MB (1163326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0730779ca73578c83a210e39877a270c4a66834bd12b23cf515389d07213ac72`  
		Last Modified: Wed, 08 Feb 2023 23:58:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:bddc4b456724f377099c6889de30e23e6b434d71153db528d9746fade979f0c8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125786646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4850c9ee7a87ef514c7c4e3c3773db8494849b1ba453095ffe6fc5df07f158b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:37:51 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:37:52 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:14 GMT
ENV GOLANG_VERSION=1.19.5
# Tue, 10 Jan 2023 23:59:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Jan 2023 23:59:24 GMT
ENV GOPATH=/go
# Tue, 10 Jan 2023 23:59:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:59:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 10 Jan 2023 23:59:25 GMT
WORKDIR /go
# Thu, 09 Feb 2023 03:57:02 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 03:57:02 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 03:57:03 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:57:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 03:57:03 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 03:57:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 03:57:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 03:57:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3aa66ae7ca151fbd33126b15fa4d01bd5ceb35d53de36a8c6c82ecde58b596`  
		Last Modified: Mon, 09 Jan 2023 17:42:45 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491d6e59a2be619159e6630fabdf81f0255c275176cd97d109fa2f417935d6a8`  
		Last Modified: Wed, 11 Jan 2023 00:06:29 GMT  
		Size: 116.9 MB (116882841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4d12be79e26ab534722d5e8e5c9d931ed5ebd84ded16cae4b12390bb543502`  
		Last Modified: Wed, 11 Jan 2023 00:06:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c89dffd73dee99c1e6d53d4ea8cc302fa2089ee3edef14dc51585b33986fc9`  
		Last Modified: Thu, 09 Feb 2023 03:57:40 GMT  
		Size: 4.2 MB (4234011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cfcadb2a14be80b0bad3d94a219fcb7e0889a821a54688bc4ca6f47b905d88`  
		Last Modified: Thu, 09 Feb 2023 03:57:39 GMT  
		Size: 1.1 MB (1123736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b4461ab8f854d2e2000cacc11f5ee723a0888222cbd031ae1d1f0ae14c3e94`  
		Last Modified: Thu, 09 Feb 2023 03:57:39 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:7805a8da1341b4d0a403cd79ce628ded1f59f183d0c9d1a736e8d898370ca860
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126524152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c705e4439b5eac8b98303529a2168b757e4fad96343a01659c151be8647f401f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:13 GMT
ADD file:9a1d27fdc0c915f387f2446c85193d5215b18020b313114f0bf2799efcc1baae in / 
# Mon, 09 Jan 2023 17:05:13 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:34:40 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 21:34:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:42 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:01:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:01:19 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:01:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:01:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:01:20 GMT
WORKDIR /go
# Thu, 09 Feb 2023 06:18:37 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 06:18:37 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 06:18:38 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 06:18:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 06:18:38 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 06:18:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 06:18:42 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 06:18:42 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f45bfda3aa14e255d9eb4c9a108eb3d8c6721946b4aa2e5808e5092242344a1c`  
		Last Modified: Mon, 09 Jan 2023 17:05:56 GMT  
		Size: 3.4 MB (3384562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ab1c47929aa42b49b577230cb740bcf3e8aebc5abb60aabb4e6ee296dc2cad`  
		Last Modified: Mon, 09 Jan 2023 21:44:30 GMT  
		Size: 286.6 KB (286647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ded0f2fb726423b204889105ff334f3133acd9bbd8a5edfddad43e6e904485`  
		Last Modified: Wed, 11 Jan 2023 00:14:05 GMT  
		Size: 117.3 MB (117267319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c616b872c15882d15d49d081ce173bb6fa4e0f36ffead4b1938923db8038bd`  
		Last Modified: Wed, 11 Jan 2023 00:13:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e47ce9bd35950f8803ed14aa1fe38b85865479ec312ffa8b32df18b26add09`  
		Last Modified: Thu, 09 Feb 2023 06:19:42 GMT  
		Size: 4.5 MB (4479174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e8d19e2da6aa4d4205abf9c47ab0c45f001d2f8af00e99eb2bd7fec2852519`  
		Last Modified: Thu, 09 Feb 2023 06:19:41 GMT  
		Size: 1.1 MB (1105889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb53e3916ae4f3ac3cd8e441e2276b18484cf30de7a4f7b9ccb908933cd7502a`  
		Last Modified: Thu, 09 Feb 2023 06:19:41 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3-builder` - linux; s390x

```console
$ docker pull caddy@sha256:3fa0a9eed3f7aaac0dbb713789109e64e4a585c7a9293211ecacc1d944b973be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129575744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a22f7e76fad31ed672b8977ea04a84eb19571daac58c337bd73a5c173ceecc6b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:44 GMT
ADD file:eabe7c3c368e65478b53ac35c1daf3b703f2bca4ecdab2d080a65e8b981d7d4a in / 
# Mon, 09 Jan 2023 17:05:46 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:42:43 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:42:43 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:53 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:56 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:57 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:41:57 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:41:58 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:42:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:42:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:42:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ae982806674c51a962c0fdd6e19f464ebd673df529c5cfb7c1d049e0b618d384`  
		Last Modified: Mon, 09 Jan 2023 17:06:50 GMT  
		Size: 3.2 MB (3170744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a5579d5fa8a33df30a972596fba4f03e76edabd19e57e62163b9c717fc188f`  
		Last Modified: Mon, 09 Jan 2023 17:54:33 GMT  
		Size: 285.0 KB (285022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4535e632f08f4af238fcccc27545520d10696aa3ce5920e33ba5578c3ee0e23`  
		Last Modified: Wed, 11 Jan 2023 00:12:31 GMT  
		Size: 120.8 MB (120785530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7633b4de83c59883de617e4ab5c606af3c556d6de4e45337bc59bff5bf7fe8ee`  
		Last Modified: Wed, 11 Jan 2023 00:12:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54414a7d37854703b1d037b805f6d0a49d2d398794414e3cedd1507c4bff0b82`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 4.2 MB (4163474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1779d1179e942debc68a6641287b6503a7e6949318c9272acb0273d7947d66e7`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 1.2 MB (1170413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597462f6847e463140e07072d10801a4c80c146d229deb04ef5cbc8b6f043464`  
		Last Modified: Wed, 08 Feb 2023 23:42:50 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3-builder` - windows version 10.0.17763.3887; amd64

```console
$ docker pull caddy@sha256:feeef34c537e9ea177fbaddb84e47df2e84a5cce70f7c8e3730e41822897b57e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1893070742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14ec5079fc868b1ce19abdcd6fca0964fae438be489b78914e21eac77dee89b3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 03:01:55 GMT
ENV GIT_VERSION=2.23.0
# Thu, 12 Jan 2023 03:01:56 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 12 Jan 2023 03:01:57 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 12 Jan 2023 03:01:58 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 12 Jan 2023 03:02:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:03:01 GMT
ENV GOPATH=C:\go
# Thu, 12 Jan 2023 03:03:35 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 Jan 2023 03:20:09 GMT
ENV GOLANG_VERSION=1.19.5
# Thu, 12 Jan 2023 03:23:52 GMT
RUN $url = 'https://dl.google.com/go/go1.19.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '167db91a2e40aeb453d3e59d213ecab06f62e1c4a84d13a06ccda1d999961caa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:23:54 GMT
WORKDIR C:\go
# Thu, 12 Jan 2023 05:33:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:19:59 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 00:20:00 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:20:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 00:20:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Feb 2023 00:20:35 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203425975bec1802428fad91a2e5f01172b161062c12eddf729e548bf7e134e0`  
		Last Modified: Thu, 12 Jan 2023 03:48:09 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80e42e19ab862b4adea06f1995e1f5cbb2c11ad8d68ae4a7bb5d0da5d0e6f38`  
		Last Modified: Thu, 12 Jan 2023 03:48:06 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be5d5df8cec6d1386f78a342668c3d2cb809372865459c1b35aa8d5a39a463b`  
		Last Modified: Thu, 12 Jan 2023 03:48:06 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e467d553c4972b55bf8e3d80b16f245e5bb38f28d80b91ca4f9f90c09a6c28d`  
		Last Modified: Thu, 12 Jan 2023 03:48:05 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97054b77b205167acd5a303c8aa82e380f090ff4e2ded81d3425ec78500139d`  
		Last Modified: Thu, 12 Jan 2023 03:48:14 GMT  
		Size: 25.5 MB (25470784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e150d9e1a1da09e17313cb3b6358d2f16cf2919c51e9addf30500de9d03292ef`  
		Last Modified: Thu, 12 Jan 2023 03:48:03 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c0d792e2a7942826a61fdc26b6081ab404122751ff4f4dd8f5b8b0eca21399`  
		Last Modified: Thu, 12 Jan 2023 03:48:03 GMT  
		Size: 324.5 KB (324466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cdd2ff60bbafbd62e677e0798ee562e3c4b291b841c6d0904ca080220e132a`  
		Last Modified: Thu, 12 Jan 2023 03:52:14 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17e6f8c13d649cbaec88dcdd4b1de7b004cf19227fbb4f923bd031b6b57988f`  
		Last Modified: Thu, 12 Jan 2023 03:53:12 GMT  
		Size: 157.7 MB (157659743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29fbb32977b62254a5de7ced98fe2a21e0342aa9db7b3cf32be4013d96b2cd9`  
		Last Modified: Thu, 12 Jan 2023 03:52:14 GMT  
		Size: 1.6 KB (1563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2fbb7e05d875affd4596aa7b87572980a3ab74800cff17a34deb445bed71b8`  
		Last Modified: Thu, 12 Jan 2023 05:36:53 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edae42a55d8aaff06e33b6f9ac104d54771346e5f4f59afd8ce90c794716611a`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb86a1e32dd5f27c1ba5ed4c675ff8c1477230677af11f17c75379385bd990b4`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d846d73e8be9adf7269d7376adebc7a8e8706b560a5f0d67886ab98c1d00c233`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2d31296154ed152465faac00831500590d35be69015063bb3ae3cc3514575d`  
		Last Modified: Thu, 09 Feb 2023 01:17:38 GMT  
		Size: 1.7 MB (1653847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef57a9413d8bab4ab7212470d9ac2b9eafc5efb5dc44aef718c91f935daddce`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3-builder` - windows version 10.0.20348.1487; amd64

```console
$ docker pull caddy@sha256:e288b33447f0b01c2ee0954c57e574b43ce9ed4b56cbd813eca3cb1df8d9f766
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1572061864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c236dcd08d81ed31367d57c62c7e77e2421092030cd5365c6a225b0ad121c6b5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 02:57:40 GMT
ENV GIT_VERSION=2.23.0
# Thu, 12 Jan 2023 02:57:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 12 Jan 2023 02:57:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 12 Jan 2023 02:57:42 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 12 Jan 2023 02:58:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 02:58:23 GMT
ENV GOPATH=C:\go
# Thu, 12 Jan 2023 02:58:47 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 Jan 2023 03:16:17 GMT
ENV GOLANG_VERSION=1.19.5
# Thu, 12 Jan 2023 03:19:43 GMT
RUN $url = 'https://dl.google.com/go/go1.19.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '167db91a2e40aeb453d3e59d213ecab06f62e1c4a84d13a06ccda1d999961caa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:19:45 GMT
WORKDIR C:\go
# Thu, 12 Jan 2023 05:34:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:20:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 00:20:47 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:20:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 00:21:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Feb 2023 00:21:22 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2fc8728d9c7bf65edf893fd902f8b1bd780f93623858960c9db79e39922b169`  
		Last Modified: Thu, 12 Jan 2023 03:47:24 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7935a4c648078e79f67a11bcd5908e251110dd6c5a4ee49a607f332dd25af9`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d257f8b122044547f89f00f58661b25aca97c92f3831e7aaa11975639b6e35d4`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95acaa75c1852ba1320c5db382b01f587badb615b6746b59be27eedcf96ab667`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5201ba65043fa621c187729f18aecf4c549cdfa12cd6d8cab7a901d893f3a8a8`  
		Last Modified: Thu, 12 Jan 2023 03:47:29 GMT  
		Size: 25.7 MB (25702230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a317a349bca5ab28ba7c1ce039928a56390f7e7a8d7ddec07efcc1c9883e5d`  
		Last Modified: Thu, 12 Jan 2023 03:47:18 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8850296b8fbb853a6eb6341f7484cd4bc622e9f679f12c4123eddf08b7f398fb`  
		Last Modified: Thu, 12 Jan 2023 03:47:18 GMT  
		Size: 554.2 KB (554212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80b3d62f45a345eaac7caba0cdc514011cc61ea8f9d7d7b82d1bd4f8f3dbea4`  
		Last Modified: Thu, 12 Jan 2023 03:50:53 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320dc1bc3ac081a72fbca97a699b20068d92c70b3caaec8ca53036ab37509933`  
		Last Modified: Thu, 12 Jan 2023 03:51:58 GMT  
		Size: 157.9 MB (157885976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230636fcbea662dc69129c73285f4376c0b83a3222e8d438ec859d14ee1201b8`  
		Last Modified: Thu, 12 Jan 2023 03:50:53 GMT  
		Size: 1.6 KB (1569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581e22afffddeddb0a4127481e5016946bd3f35379291c6bb1e3b85e92e7acef`  
		Last Modified: Thu, 12 Jan 2023 05:37:10 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13aaa30213dc8e6b5906114a862d8398ac157fd2f8c835767a058069f180a181`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b39a2446c556432e7503cc419fe42c4d14ff3fc744cf6d475136c5058bc18d6`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43ea60403f6819d31f67d7dc2d230def090cb6366c7cd272d99d8d06aac019d`  
		Last Modified: Thu, 09 Feb 2023 01:17:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5970b711fddee53f278567276c42d2b169c5286a5133ba48ce3a599b253b37ab`  
		Last Modified: Thu, 09 Feb 2023 01:17:55 GMT  
		Size: 1.9 MB (1871861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1270e653c78ffbadd8ab6379e16db4c45c20fb148d294ec9654f1d13367fea6`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.3-builder-alpine`

```console
$ docker pull caddy@sha256:e6c08f0694b44abd7ae623da15e368a4828a38cae59c041ab8f55c750fc66351
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.6.3-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:b86e1de154ca5d11618a408742e2b6f16f99e55cdc0ee97fe0965da9f1b1572f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131390128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:858147920561fe47255b181692d82558dbab931f4393f33ba8697b9c647f690e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:50:11 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:50:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:23 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:01 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:02 GMT
WORKDIR /go
# Thu, 09 Feb 2023 03:18:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 03:18:17 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 03:18:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 03:18:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 03:18:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f8637abd914a8a62416e027a351293d0472bc4b4f44383c6f425fd0e03861c`  
		Last Modified: Mon, 09 Jan 2023 17:56:43 GMT  
		Size: 284.8 KB (284814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48e7ca896ec974241d86439d34188186e085705e42d914d8b7757c27eea8613`  
		Last Modified: Wed, 11 Jan 2023 00:08:38 GMT  
		Size: 122.3 MB (122328552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f26d270037d8578282b40f86c0a1816fc5d034d6213f7dcab8440056a589309`  
		Last Modified: Wed, 11 Jan 2023 00:08:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807cf12e90d621962959f760ccbca1b77b95c6120884fefcc4385f12614f9e49`  
		Last Modified: Thu, 09 Feb 2023 03:18:55 GMT  
		Size: 4.2 MB (4187743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1e21e6198268a646e1f41d15b44931dc2d1ffaf7448588af3237d7443de8df`  
		Last Modified: Thu, 09 Feb 2023 03:18:54 GMT  
		Size: 1.2 MB (1217832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86c409f0ecb7b6ab12d691c73e32350f6453fc6e477af6fe53ec7946e91ec08`  
		Last Modified: Thu, 09 Feb 2023 03:18:54 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2d6f2baed8a8d6af9014cc57d9488335fd4d9ded609476ce98307a241b55f680
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127387922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad435c186a3c6ffdd4910420eabfef5bbf8a84e247d2473ac2c1394e5ece3781`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:28:28 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:28:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:57:48 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:48 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:49 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:49:43 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:49:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:49:44 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:49:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:49:45 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:49:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:49:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:49:47 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3919da799d44c7be2eecafbf780801f4cd562b289c55ebe566999525497cd24`  
		Last Modified: Mon, 09 Jan 2023 17:37:35 GMT  
		Size: 286.1 KB (286122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c266a9580739a5c56dffcd14ce61144c9f58539d8c927ccd3df332434ad8d57`  
		Last Modified: Wed, 11 Jan 2023 00:11:13 GMT  
		Size: 118.7 MB (118677328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9666a7ae960b29537b5e693ea358a6181a3b9b73110b1099f22596b2dedbe3bd`  
		Last Modified: Wed, 11 Jan 2023 00:10:50 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b71d65a08c2aecf44c515cedf0abefc5f896bd9942291a29ddcf6646452661`  
		Last Modified: Wed, 08 Feb 2023 23:50:58 GMT  
		Size: 4.2 MB (4150629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a427cd9f7efb7c150d196c96034cdc132bf3c26025a87378400da762842a4923`  
		Last Modified: Wed, 08 Feb 2023 23:50:57 GMT  
		Size: 1.2 MB (1166069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278f59186f97ea59dd8a5f727fe7b3e2aa46b384971583b5b277b871a61b2131`  
		Last Modified: Wed, 08 Feb 2023 23:50:57 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:ad4dce5e6c2c07e73c35c50cdc26e110c439a947f626c86482c0bc5165ad8d9e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126503260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be8c29fce7791d265104052e6900b3eca71a13aa0b77861ded3aac664b4e9ae7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:04:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 10 Jan 2023 01:04:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:59:19 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:02:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:02:06 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:02:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:02:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:02:08 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:57:41 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:57:42 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:57:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:57:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:57:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c7609f223a73f5c1097b3b7cb1ea29e1e540da920bc3b48b8672a1d5ef1dc9`  
		Last Modified: Tue, 10 Jan 2023 01:13:57 GMT  
		Size: 285.4 KB (285359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da97c3a81e19449c60385f1e4cf4fd4fc9ffd14d08a26ccb6782cafd2d5d6f66`  
		Last Modified: Wed, 11 Jan 2023 00:15:15 GMT  
		Size: 118.5 MB (118468701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e98750b6aa4570218317d53b00f803a47aff7219e78c594d1666eef08e0258`  
		Last Modified: Wed, 11 Jan 2023 00:14:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ffc027d61bfbcc1c13359e022e0e4e6a5ef7cf40c49a8979e7d2f2a40add601`  
		Last Modified: Wed, 08 Feb 2023 23:58:48 GMT  
		Size: 3.7 MB (3720136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c82d9a2e5d63888f8bbe98b76b4b3565ccc2c8ce45526e794fae5f54d98ba49`  
		Last Modified: Wed, 08 Feb 2023 23:58:48 GMT  
		Size: 1.2 MB (1163326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0730779ca73578c83a210e39877a270c4a66834bd12b23cf515389d07213ac72`  
		Last Modified: Wed, 08 Feb 2023 23:58:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:bddc4b456724f377099c6889de30e23e6b434d71153db528d9746fade979f0c8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125786646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4850c9ee7a87ef514c7c4e3c3773db8494849b1ba453095ffe6fc5df07f158b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:37:51 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:37:52 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:14 GMT
ENV GOLANG_VERSION=1.19.5
# Tue, 10 Jan 2023 23:59:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Jan 2023 23:59:24 GMT
ENV GOPATH=/go
# Tue, 10 Jan 2023 23:59:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:59:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 10 Jan 2023 23:59:25 GMT
WORKDIR /go
# Thu, 09 Feb 2023 03:57:02 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 03:57:02 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 03:57:03 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:57:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 03:57:03 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 03:57:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 03:57:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 03:57:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3aa66ae7ca151fbd33126b15fa4d01bd5ceb35d53de36a8c6c82ecde58b596`  
		Last Modified: Mon, 09 Jan 2023 17:42:45 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491d6e59a2be619159e6630fabdf81f0255c275176cd97d109fa2f417935d6a8`  
		Last Modified: Wed, 11 Jan 2023 00:06:29 GMT  
		Size: 116.9 MB (116882841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4d12be79e26ab534722d5e8e5c9d931ed5ebd84ded16cae4b12390bb543502`  
		Last Modified: Wed, 11 Jan 2023 00:06:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c89dffd73dee99c1e6d53d4ea8cc302fa2089ee3edef14dc51585b33986fc9`  
		Last Modified: Thu, 09 Feb 2023 03:57:40 GMT  
		Size: 4.2 MB (4234011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cfcadb2a14be80b0bad3d94a219fcb7e0889a821a54688bc4ca6f47b905d88`  
		Last Modified: Thu, 09 Feb 2023 03:57:39 GMT  
		Size: 1.1 MB (1123736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b4461ab8f854d2e2000cacc11f5ee723a0888222cbd031ae1d1f0ae14c3e94`  
		Last Modified: Thu, 09 Feb 2023 03:57:39 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:7805a8da1341b4d0a403cd79ce628ded1f59f183d0c9d1a736e8d898370ca860
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126524152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c705e4439b5eac8b98303529a2168b757e4fad96343a01659c151be8647f401f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:13 GMT
ADD file:9a1d27fdc0c915f387f2446c85193d5215b18020b313114f0bf2799efcc1baae in / 
# Mon, 09 Jan 2023 17:05:13 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:34:40 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 21:34:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:42 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:01:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:01:19 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:01:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:01:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:01:20 GMT
WORKDIR /go
# Thu, 09 Feb 2023 06:18:37 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 06:18:37 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 06:18:38 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 06:18:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 06:18:38 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 06:18:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 06:18:42 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 06:18:42 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f45bfda3aa14e255d9eb4c9a108eb3d8c6721946b4aa2e5808e5092242344a1c`  
		Last Modified: Mon, 09 Jan 2023 17:05:56 GMT  
		Size: 3.4 MB (3384562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ab1c47929aa42b49b577230cb740bcf3e8aebc5abb60aabb4e6ee296dc2cad`  
		Last Modified: Mon, 09 Jan 2023 21:44:30 GMT  
		Size: 286.6 KB (286647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ded0f2fb726423b204889105ff334f3133acd9bbd8a5edfddad43e6e904485`  
		Last Modified: Wed, 11 Jan 2023 00:14:05 GMT  
		Size: 117.3 MB (117267319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c616b872c15882d15d49d081ce173bb6fa4e0f36ffead4b1938923db8038bd`  
		Last Modified: Wed, 11 Jan 2023 00:13:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e47ce9bd35950f8803ed14aa1fe38b85865479ec312ffa8b32df18b26add09`  
		Last Modified: Thu, 09 Feb 2023 06:19:42 GMT  
		Size: 4.5 MB (4479174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e8d19e2da6aa4d4205abf9c47ab0c45f001d2f8af00e99eb2bd7fec2852519`  
		Last Modified: Thu, 09 Feb 2023 06:19:41 GMT  
		Size: 1.1 MB (1105889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb53e3916ae4f3ac3cd8e441e2276b18484cf30de7a4f7b9ccb908933cd7502a`  
		Last Modified: Thu, 09 Feb 2023 06:19:41 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:3fa0a9eed3f7aaac0dbb713789109e64e4a585c7a9293211ecacc1d944b973be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129575744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a22f7e76fad31ed672b8977ea04a84eb19571daac58c337bd73a5c173ceecc6b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:44 GMT
ADD file:eabe7c3c368e65478b53ac35c1daf3b703f2bca4ecdab2d080a65e8b981d7d4a in / 
# Mon, 09 Jan 2023 17:05:46 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:42:43 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:42:43 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:53 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:56 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:57 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:41:57 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:41:58 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:42:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:42:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:42:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ae982806674c51a962c0fdd6e19f464ebd673df529c5cfb7c1d049e0b618d384`  
		Last Modified: Mon, 09 Jan 2023 17:06:50 GMT  
		Size: 3.2 MB (3170744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a5579d5fa8a33df30a972596fba4f03e76edabd19e57e62163b9c717fc188f`  
		Last Modified: Mon, 09 Jan 2023 17:54:33 GMT  
		Size: 285.0 KB (285022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4535e632f08f4af238fcccc27545520d10696aa3ce5920e33ba5578c3ee0e23`  
		Last Modified: Wed, 11 Jan 2023 00:12:31 GMT  
		Size: 120.8 MB (120785530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7633b4de83c59883de617e4ab5c606af3c556d6de4e45337bc59bff5bf7fe8ee`  
		Last Modified: Wed, 11 Jan 2023 00:12:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54414a7d37854703b1d037b805f6d0a49d2d398794414e3cedd1507c4bff0b82`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 4.2 MB (4163474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1779d1179e942debc68a6641287b6503a7e6949318c9272acb0273d7947d66e7`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 1.2 MB (1170413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597462f6847e463140e07072d10801a4c80c146d229deb04ef5cbc8b6f043464`  
		Last Modified: Wed, 08 Feb 2023 23:42:50 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.3-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:4c57090f03b98d1a89618055d77e7e8864830bf83840fd17b1228bfa3cc8db4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `caddy:2.6.3-builder-windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull caddy@sha256:feeef34c537e9ea177fbaddb84e47df2e84a5cce70f7c8e3730e41822897b57e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1893070742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14ec5079fc868b1ce19abdcd6fca0964fae438be489b78914e21eac77dee89b3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 03:01:55 GMT
ENV GIT_VERSION=2.23.0
# Thu, 12 Jan 2023 03:01:56 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 12 Jan 2023 03:01:57 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 12 Jan 2023 03:01:58 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 12 Jan 2023 03:02:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:03:01 GMT
ENV GOPATH=C:\go
# Thu, 12 Jan 2023 03:03:35 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 Jan 2023 03:20:09 GMT
ENV GOLANG_VERSION=1.19.5
# Thu, 12 Jan 2023 03:23:52 GMT
RUN $url = 'https://dl.google.com/go/go1.19.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '167db91a2e40aeb453d3e59d213ecab06f62e1c4a84d13a06ccda1d999961caa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:23:54 GMT
WORKDIR C:\go
# Thu, 12 Jan 2023 05:33:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:19:59 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 00:20:00 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:20:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 00:20:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Feb 2023 00:20:35 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203425975bec1802428fad91a2e5f01172b161062c12eddf729e548bf7e134e0`  
		Last Modified: Thu, 12 Jan 2023 03:48:09 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80e42e19ab862b4adea06f1995e1f5cbb2c11ad8d68ae4a7bb5d0da5d0e6f38`  
		Last Modified: Thu, 12 Jan 2023 03:48:06 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be5d5df8cec6d1386f78a342668c3d2cb809372865459c1b35aa8d5a39a463b`  
		Last Modified: Thu, 12 Jan 2023 03:48:06 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e467d553c4972b55bf8e3d80b16f245e5bb38f28d80b91ca4f9f90c09a6c28d`  
		Last Modified: Thu, 12 Jan 2023 03:48:05 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97054b77b205167acd5a303c8aa82e380f090ff4e2ded81d3425ec78500139d`  
		Last Modified: Thu, 12 Jan 2023 03:48:14 GMT  
		Size: 25.5 MB (25470784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e150d9e1a1da09e17313cb3b6358d2f16cf2919c51e9addf30500de9d03292ef`  
		Last Modified: Thu, 12 Jan 2023 03:48:03 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c0d792e2a7942826a61fdc26b6081ab404122751ff4f4dd8f5b8b0eca21399`  
		Last Modified: Thu, 12 Jan 2023 03:48:03 GMT  
		Size: 324.5 KB (324466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cdd2ff60bbafbd62e677e0798ee562e3c4b291b841c6d0904ca080220e132a`  
		Last Modified: Thu, 12 Jan 2023 03:52:14 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17e6f8c13d649cbaec88dcdd4b1de7b004cf19227fbb4f923bd031b6b57988f`  
		Last Modified: Thu, 12 Jan 2023 03:53:12 GMT  
		Size: 157.7 MB (157659743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29fbb32977b62254a5de7ced98fe2a21e0342aa9db7b3cf32be4013d96b2cd9`  
		Last Modified: Thu, 12 Jan 2023 03:52:14 GMT  
		Size: 1.6 KB (1563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2fbb7e05d875affd4596aa7b87572980a3ab74800cff17a34deb445bed71b8`  
		Last Modified: Thu, 12 Jan 2023 05:36:53 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edae42a55d8aaff06e33b6f9ac104d54771346e5f4f59afd8ce90c794716611a`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb86a1e32dd5f27c1ba5ed4c675ff8c1477230677af11f17c75379385bd990b4`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d846d73e8be9adf7269d7376adebc7a8e8706b560a5f0d67886ab98c1d00c233`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2d31296154ed152465faac00831500590d35be69015063bb3ae3cc3514575d`  
		Last Modified: Thu, 09 Feb 2023 01:17:38 GMT  
		Size: 1.7 MB (1653847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef57a9413d8bab4ab7212470d9ac2b9eafc5efb5dc44aef718c91f935daddce`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.3-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:5016a9ee6f22300f4699ec2ba33c105b273e55c4b6931dcdbe8a7326d9dc037a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1487; amd64

### `caddy:2.6.3-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1487; amd64

```console
$ docker pull caddy@sha256:e288b33447f0b01c2ee0954c57e574b43ce9ed4b56cbd813eca3cb1df8d9f766
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1572061864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c236dcd08d81ed31367d57c62c7e77e2421092030cd5365c6a225b0ad121c6b5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 02:57:40 GMT
ENV GIT_VERSION=2.23.0
# Thu, 12 Jan 2023 02:57:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 12 Jan 2023 02:57:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 12 Jan 2023 02:57:42 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 12 Jan 2023 02:58:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 02:58:23 GMT
ENV GOPATH=C:\go
# Thu, 12 Jan 2023 02:58:47 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 Jan 2023 03:16:17 GMT
ENV GOLANG_VERSION=1.19.5
# Thu, 12 Jan 2023 03:19:43 GMT
RUN $url = 'https://dl.google.com/go/go1.19.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '167db91a2e40aeb453d3e59d213ecab06f62e1c4a84d13a06ccda1d999961caa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:19:45 GMT
WORKDIR C:\go
# Thu, 12 Jan 2023 05:34:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:20:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 00:20:47 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:20:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 00:21:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Feb 2023 00:21:22 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2fc8728d9c7bf65edf893fd902f8b1bd780f93623858960c9db79e39922b169`  
		Last Modified: Thu, 12 Jan 2023 03:47:24 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7935a4c648078e79f67a11bcd5908e251110dd6c5a4ee49a607f332dd25af9`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d257f8b122044547f89f00f58661b25aca97c92f3831e7aaa11975639b6e35d4`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95acaa75c1852ba1320c5db382b01f587badb615b6746b59be27eedcf96ab667`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5201ba65043fa621c187729f18aecf4c549cdfa12cd6d8cab7a901d893f3a8a8`  
		Last Modified: Thu, 12 Jan 2023 03:47:29 GMT  
		Size: 25.7 MB (25702230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a317a349bca5ab28ba7c1ce039928a56390f7e7a8d7ddec07efcc1c9883e5d`  
		Last Modified: Thu, 12 Jan 2023 03:47:18 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8850296b8fbb853a6eb6341f7484cd4bc622e9f679f12c4123eddf08b7f398fb`  
		Last Modified: Thu, 12 Jan 2023 03:47:18 GMT  
		Size: 554.2 KB (554212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80b3d62f45a345eaac7caba0cdc514011cc61ea8f9d7d7b82d1bd4f8f3dbea4`  
		Last Modified: Thu, 12 Jan 2023 03:50:53 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320dc1bc3ac081a72fbca97a699b20068d92c70b3caaec8ca53036ab37509933`  
		Last Modified: Thu, 12 Jan 2023 03:51:58 GMT  
		Size: 157.9 MB (157885976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230636fcbea662dc69129c73285f4376c0b83a3222e8d438ec859d14ee1201b8`  
		Last Modified: Thu, 12 Jan 2023 03:50:53 GMT  
		Size: 1.6 KB (1569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581e22afffddeddb0a4127481e5016946bd3f35379291c6bb1e3b85e92e7acef`  
		Last Modified: Thu, 12 Jan 2023 05:37:10 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13aaa30213dc8e6b5906114a862d8398ac157fd2f8c835767a058069f180a181`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b39a2446c556432e7503cc419fe42c4d14ff3fc744cf6d475136c5058bc18d6`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43ea60403f6819d31f67d7dc2d230def090cb6366c7cd272d99d8d06aac019d`  
		Last Modified: Thu, 09 Feb 2023 01:17:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5970b711fddee53f278567276c42d2b169c5286a5133ba48ce3a599b253b37ab`  
		Last Modified: Thu, 09 Feb 2023 01:17:55 GMT  
		Size: 1.9 MB (1871861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1270e653c78ffbadd8ab6379e16db4c45c20fb148d294ec9654f1d13367fea6`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.3-windowsservercore`

```console
$ docker pull caddy@sha256:0824e61dd8be6c1fa86bcf0faf1d4c5d8a41c047e0d4bf9ec8bbb73f243adaf6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3887; amd64
	-	windows version 10.0.20348.1487; amd64

### `caddy:2.6.3-windowsservercore` - windows version 10.0.17763.3887; amd64

```console
$ docker pull caddy@sha256:935d1f4349cc551dfe9b76d6ba5fe6355414519a3037a7689fe765033ae8dcd6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1723388621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1deb1aecac8501d9afe22abd2fc90f15552c63366f8016ad2e6d1602be5cdf6d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:16:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:16:36 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:17:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:17:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:17:21 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:17:22 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:17:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:17:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:17:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:17:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:17:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:17:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:17:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:17:31 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:17:32 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:17:33 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:17:34 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:17:53 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:17:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47af8a9c9ef8e49d65e53dd207ad0935ce7a2b50b2f253e6a5b037494ae19d0a`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 401.5 KB (401472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5841cb6343add9dd7b89906610425117976b050c0634eedbc5c38302aa024e`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d760049e5c9f1fb1d7ec05a3eea55088808f484912e87cda07f3709363fe3c2c`  
		Last Modified: Thu, 09 Feb 2023 01:16:53 GMT  
		Size: 14.7 MB (14680484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3239225b5bad52e6004b638bd356e7d29e7fded5d31d90541907e1a769a115`  
		Last Modified: Thu, 09 Feb 2023 01:16:49 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6823ad091829bc6d98a58a18b075e20c551bde81d504bdbfda09b5a3d7c5d0`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4873a8802163accb90dd2318bd05ddfa4f94692b2731d6e23095e3bb46b98fd`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabf39e152fd5c18e0c3ac503e054c36e2775512f9fa7bb11b9221442b2bc1fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af12dc4018ba87a8e25003874e2d8e959a25b1c19932553daec8f4c410ebd61f`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fefa1f82e39e2af863b13609d78d966746d852af0cea54dcb17f45a8386c39d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d5b41708aea61714f00bc0f35ea1efc60db85c04ab6754e4d6b4485dc59a28`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a8b1cf8bcc4175323f7feaa280e3122f03aa7f9d35666fcc55c6b7d1e628ae`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c3f865e552649c436d5ffc0f3c83a3b5ba3026b2cff2ab3f381a5cdf2e2f2`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201cfdbfc1583e2ea070418e6aad0ec6604fb52c68117460b1a4c5b511b56ecc`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef83199fb67566ea043dbf7fab6f54754a4d0496655be1157819973573247bb`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45db789a3d9786dea133341e2c9f16e14b23a664297ad7f9a371961a0c21588`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a4e021c112717a1fee7cd62cdc17d41521f3514f10bf8ec30457b95aaf44fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4c0327054bc1f199339822d4074ee176c4184b9357ec28d9250f27f0c12e26`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63a4d912695117a127068d20ceefbaa19e41c8a42d65788d37915d737d998d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:44 GMT  
		Size: 338.6 KB (338620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421719fbbf536a3651d6762e36406f19dd0b5601f4a300d9c47af9ccfa3573d2`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.3-windowsservercore` - windows version 10.0.20348.1487; amd64

```console
$ docker pull caddy@sha256:22cdfda624195707c05f1d681c1cdd97b504f06b282d981718e1b716b2dc6bfb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1401937005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca7c6af6ec202266d95f15726fee733430a631c6c4eddfd9cc7d000b817a0f19`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:18:43 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:18:44 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:19:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:19:16 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:19:17 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:19:18 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:19:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:19:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:19:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:19:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:19:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:19:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:19:26 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:19:27 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:19:29 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:19:30 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:19:47 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:19:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42eb48143612ee855d99c932e324b1bd035c60554117edeaa805402060613c51`  
		Last Modified: Thu, 09 Feb 2023 01:17:17 GMT  
		Size: 635.9 KB (635943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714ae92cb5dac0e72097d35b932125b5ea3f03214de78e03119a4517be6fd10`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a5533d3ddbff5ea35dbb0e11b10fe817ce3ef1a3fd7f44706cb1b6288e0406`  
		Last Modified: Thu, 09 Feb 2023 01:17:20 GMT  
		Size: 14.9 MB (14899830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e59c8f0dc8d987210bdfe89eaded536b0ef8ac727eb7d75b76aea9c296208a`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22bfc3588219a43ce294aab21751b407ae75504bf3ddcee69f42498672b6c46`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f7db57dc0a0b0126433f60d3d0005f9aaa0d405fe63cfc3b4e15388fdfa010`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7b9e3a2510b5ab3b7ac4103d653c8efd12e95b63327d5c5fb81b6ea341e2b5`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4109b3b0ca73b5355a12ee74b7c32b4015a6208fdb279fd0ab60074247e22309`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3c568a1866d44483984b2be40142a55371adf3b8dc991bdb5ab4c45c0be3d4`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6221c7c14444b318e798e231adeeb83ea155c157283e9def018c43415238aa7`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e81980463382095586f78276db5cd808400136543fc1a0f522af1f3eaee034`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f0d8afe85320b7cf4542ad649671660bbb8e74ec3ad3067408e79fb21dbf77`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7def0e2b3dd94a350c82bb6a4903fdfc65d1d3d9772dd8195a5eb14ba766c45`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0b51c8090bf08cc2ae3a9fc340c9b70ba1e077f32b7d7d025b7d9fb472d978`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3653016f515e293fc93892b9e021e05a6a183ad3dcdaf243311513e222534c7`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d1dafd3fbb7403b7f093ed63553863bd9904f6010b1b91f98d9bfba9c4d8bb`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92817327253aaae4d632a75ff38a01dbebfe11f9105c4db828c52f221262ce4`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43bce457643a143e82e49e57d9b8a69a416e254d2439f30d7e4dd25c84e43c0`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 348.1 KB (348138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a0e899ab4c995de79522a5022b8cca4765559a4de2d5c728821d947b497de1`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.3-windowsservercore-1809`

```console
$ docker pull caddy@sha256:6fc3086452e6c85e993bf4b4834c55848a3977b547662cd4ce9fc98a17a495e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `caddy:2.6.3-windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull caddy@sha256:935d1f4349cc551dfe9b76d6ba5fe6355414519a3037a7689fe765033ae8dcd6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1723388621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1deb1aecac8501d9afe22abd2fc90f15552c63366f8016ad2e6d1602be5cdf6d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:16:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:16:36 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:17:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:17:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:17:21 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:17:22 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:17:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:17:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:17:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:17:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:17:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:17:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:17:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:17:31 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:17:32 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:17:33 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:17:34 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:17:53 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:17:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47af8a9c9ef8e49d65e53dd207ad0935ce7a2b50b2f253e6a5b037494ae19d0a`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 401.5 KB (401472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5841cb6343add9dd7b89906610425117976b050c0634eedbc5c38302aa024e`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d760049e5c9f1fb1d7ec05a3eea55088808f484912e87cda07f3709363fe3c2c`  
		Last Modified: Thu, 09 Feb 2023 01:16:53 GMT  
		Size: 14.7 MB (14680484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3239225b5bad52e6004b638bd356e7d29e7fded5d31d90541907e1a769a115`  
		Last Modified: Thu, 09 Feb 2023 01:16:49 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6823ad091829bc6d98a58a18b075e20c551bde81d504bdbfda09b5a3d7c5d0`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4873a8802163accb90dd2318bd05ddfa4f94692b2731d6e23095e3bb46b98fd`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabf39e152fd5c18e0c3ac503e054c36e2775512f9fa7bb11b9221442b2bc1fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af12dc4018ba87a8e25003874e2d8e959a25b1c19932553daec8f4c410ebd61f`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fefa1f82e39e2af863b13609d78d966746d852af0cea54dcb17f45a8386c39d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d5b41708aea61714f00bc0f35ea1efc60db85c04ab6754e4d6b4485dc59a28`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a8b1cf8bcc4175323f7feaa280e3122f03aa7f9d35666fcc55c6b7d1e628ae`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c3f865e552649c436d5ffc0f3c83a3b5ba3026b2cff2ab3f381a5cdf2e2f2`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201cfdbfc1583e2ea070418e6aad0ec6604fb52c68117460b1a4c5b511b56ecc`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef83199fb67566ea043dbf7fab6f54754a4d0496655be1157819973573247bb`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45db789a3d9786dea133341e2c9f16e14b23a664297ad7f9a371961a0c21588`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a4e021c112717a1fee7cd62cdc17d41521f3514f10bf8ec30457b95aaf44fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4c0327054bc1f199339822d4074ee176c4184b9357ec28d9250f27f0c12e26`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63a4d912695117a127068d20ceefbaa19e41c8a42d65788d37915d737d998d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:44 GMT  
		Size: 338.6 KB (338620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421719fbbf536a3651d6762e36406f19dd0b5601f4a300d9c47af9ccfa3573d2`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.3-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:65b3d9f69c1f9e10dae44434f033715465a5e5331b38550f4f47baa12a60a39c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1487; amd64

### `caddy:2.6.3-windowsservercore-ltsc2022` - windows version 10.0.20348.1487; amd64

```console
$ docker pull caddy@sha256:22cdfda624195707c05f1d681c1cdd97b504f06b282d981718e1b716b2dc6bfb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1401937005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca7c6af6ec202266d95f15726fee733430a631c6c4eddfd9cc7d000b817a0f19`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:18:43 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:18:44 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:19:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:19:16 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:19:17 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:19:18 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:19:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:19:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:19:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:19:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:19:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:19:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:19:26 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:19:27 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:19:29 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:19:30 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:19:47 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:19:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42eb48143612ee855d99c932e324b1bd035c60554117edeaa805402060613c51`  
		Last Modified: Thu, 09 Feb 2023 01:17:17 GMT  
		Size: 635.9 KB (635943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714ae92cb5dac0e72097d35b932125b5ea3f03214de78e03119a4517be6fd10`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a5533d3ddbff5ea35dbb0e11b10fe817ce3ef1a3fd7f44706cb1b6288e0406`  
		Last Modified: Thu, 09 Feb 2023 01:17:20 GMT  
		Size: 14.9 MB (14899830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e59c8f0dc8d987210bdfe89eaded536b0ef8ac727eb7d75b76aea9c296208a`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22bfc3588219a43ce294aab21751b407ae75504bf3ddcee69f42498672b6c46`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f7db57dc0a0b0126433f60d3d0005f9aaa0d405fe63cfc3b4e15388fdfa010`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7b9e3a2510b5ab3b7ac4103d653c8efd12e95b63327d5c5fb81b6ea341e2b5`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4109b3b0ca73b5355a12ee74b7c32b4015a6208fdb279fd0ab60074247e22309`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3c568a1866d44483984b2be40142a55371adf3b8dc991bdb5ab4c45c0be3d4`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6221c7c14444b318e798e231adeeb83ea155c157283e9def018c43415238aa7`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e81980463382095586f78276db5cd808400136543fc1a0f522af1f3eaee034`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f0d8afe85320b7cf4542ad649671660bbb8e74ec3ad3067408e79fb21dbf77`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7def0e2b3dd94a350c82bb6a4903fdfc65d1d3d9772dd8195a5eb14ba766c45`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0b51c8090bf08cc2ae3a9fc340c9b70ba1e077f32b7d7d025b7d9fb472d978`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3653016f515e293fc93892b9e021e05a6a183ad3dcdaf243311513e222534c7`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d1dafd3fbb7403b7f093ed63553863bd9904f6010b1b91f98d9bfba9c4d8bb`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92817327253aaae4d632a75ff38a01dbebfe11f9105c4db828c52f221262ce4`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43bce457643a143e82e49e57d9b8a69a416e254d2439f30d7e4dd25c84e43c0`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 348.1 KB (348138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a0e899ab4c995de79522a5022b8cca4765559a4de2d5c728821d947b497de1`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:7e7286bb77df853f278887dd9159bd643abca8447ad4a0fddb4c48ec00a7e6cc
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
$ docker pull caddy@sha256:cf66a65d5667b26ba91fab680b59d421266e5042d4191fcdeab3847b31828bf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17441779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:739163e8bd53961abf96cc4f327498332dd905a59d3314fab80a845e62b58f9b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Thu, 09 Feb 2023 03:18:05 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 09 Feb 2023 03:18:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 09 Feb 2023 03:18:06 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:18:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 09 Feb 2023 03:18:10 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 09 Feb 2023 03:18:10 GMT
ENV XDG_DATA_HOME=/data
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 80
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 443
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 03:18:11 GMT
WORKDIR /srv
# Thu, 09 Feb 2023 03:18:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4cf81513fab9758787dbde95dcab4c054bd04137581b68097595a719ae973c`  
		Last Modified: Thu, 09 Feb 2023 03:18:39 GMT  
		Size: 351.2 KB (351181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c3f44eb3bccaf2f5515331e12d4b940a5f6ad016d27f548e0c739d1f6aba66`  
		Last Modified: Thu, 09 Feb 2023 03:18:39 GMT  
		Size: 7.6 KB (7554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04314ed686e612bbb7606d6bacff938564f9b4f7e0dbc72afacd887b3c88afbd`  
		Last Modified: Thu, 09 Feb 2023 03:18:42 GMT  
		Size: 14.3 MB (14276772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e4444abb42ab384f9685f3b25765ed65d8e07daef954ccf7aa73a524a2177064
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16576623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99391525993d815548f2a8e80455bb1ff1b6dd0a769a0dc2a467cbcc3adbc1ad`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:32 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Fri, 10 Feb 2023 20:49:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:28:54 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 21:28:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Fri, 10 Feb 2023 21:28:56 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 21:28:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 21:28:59 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 21:28:59 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 80
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 443
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 21:29:00 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 21:29:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a400dcba29ff44f8e5bf01493def4f19629aca6d103cb2a66ca87c457f7414`  
		Last Modified: Fri, 10 Feb 2023 21:29:47 GMT  
		Size: 345.8 KB (345811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b946768825eb5ed2fc6f932fdb0b0c552f4c35c39dada07eddd70ce4a535953`  
		Last Modified: Fri, 10 Feb 2023 21:29:47 GMT  
		Size: 7.5 KB (7480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda323f820516b366c61a02ba4cfd00cc3a3b6cc9051c58e7359057dea842d8a`  
		Last Modified: Fri, 10 Feb 2023 21:29:51 GMT  
		Size: 13.6 MB (13606554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0a66f97fe167ebcccd1754f2cc7ed8d5f42595f332f60d75e4efd33c5fa880b9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16362110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0940efa30038d45d9b6cbae2aea1235accdd5e653948a6e40e9c3edf6314d4c6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:37:19 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:37:22 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Fri, 10 Feb 2023 22:37:22 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:37:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:37:26 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:37:27 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:37:27 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:37:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:37:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:37:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:37:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:37:30 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:37:30 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:37:31 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:37:31 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:37:31 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:37:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec2ab4edb1f0a14b28a55f050d62d8e54111075639a0fa8f173448814ba0d00`  
		Last Modified: Fri, 10 Feb 2023 22:38:25 GMT  
		Size: 342.6 KB (342588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0580184dd0082f009564a7a3923731f202cbe4bd8b857dbca2c77da8e7434815`  
		Last Modified: Fri, 10 Feb 2023 22:38:25 GMT  
		Size: 7.5 KB (7479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b2a44f2792add2104a1d53c68f1df95779deaee3ec86717f4fb4efd9aa6aaa`  
		Last Modified: Fri, 10 Feb 2023 22:38:28 GMT  
		Size: 13.6 MB (13591549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:4be5e6cdfb930681cc9c4722b0af67e75e53f0cff56c916c1d618eb39d6f5169
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16126925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:995c31e78c533c3ca73152cb87130dfcb16842dd052ab384df917fb755c5dc43`
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
# Fri, 10 Feb 2023 22:00:37 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:00:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:00:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:00:39 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:00:40 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:00:40 GMT
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
	-	`sha256:6403d7bb9250089f4077bba7631d975f97648fbcd782c992704ff3bccc5ae421`  
		Last Modified: Fri, 10 Feb 2023 22:01:03 GMT  
		Size: 13.1 MB (13059715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:50a289625f0ef1adfc05773b5ec8a30f001be347a84f24e1106e351f230758b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15949909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b11b3ee451004883e1f9089fc132ee1ecc849a2d96ef0ff4731334c8279cfa`
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
# Fri, 10 Feb 2023 22:13:23 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:13:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:13:28 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:13:28 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:13:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:13:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:13:33 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:13:33 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:13:33 GMT
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
	-	`sha256:2ecc7ec17344834a2337d83b9b7be44f97f0c0b55dfea5e1d8af80c8d5c32221`  
		Last Modified: Fri, 10 Feb 2023 22:14:19 GMT  
		Size: 12.8 MB (12774635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:9c69a670bfaa4e7166553c41a7303b114a524eed38924ad0d1d5599e6b7b2463
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16787086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9abb18c28ea7e824ff4385016f24b30d1a455d1b902f8667a1a9300078826a`
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
# Fri, 10 Feb 2023 22:14:19 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:14:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:14:21 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:14:22 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:14:23 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:14:23 GMT
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
	-	`sha256:94fd73a8831c9e57fdf8c430154c9adc56e54610a462128c8f0a1b3937aef704`  
		Last Modified: Fri, 10 Feb 2023 22:15:07 GMT  
		Size: 13.8 MB (13833147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:458901eb7e2d1f60ea430e23833e47d4b3ada93d601df57a34674b67675483b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3887; amd64
	-	windows version 10.0.20348.1487; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:b86e1de154ca5d11618a408742e2b6f16f99e55cdc0ee97fe0965da9f1b1572f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131390128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:858147920561fe47255b181692d82558dbab931f4393f33ba8697b9c647f690e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:50:11 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:50:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:23 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:01 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:02 GMT
WORKDIR /go
# Thu, 09 Feb 2023 03:18:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 03:18:17 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 03:18:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 03:18:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 03:18:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f8637abd914a8a62416e027a351293d0472bc4b4f44383c6f425fd0e03861c`  
		Last Modified: Mon, 09 Jan 2023 17:56:43 GMT  
		Size: 284.8 KB (284814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48e7ca896ec974241d86439d34188186e085705e42d914d8b7757c27eea8613`  
		Last Modified: Wed, 11 Jan 2023 00:08:38 GMT  
		Size: 122.3 MB (122328552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f26d270037d8578282b40f86c0a1816fc5d034d6213f7dcab8440056a589309`  
		Last Modified: Wed, 11 Jan 2023 00:08:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807cf12e90d621962959f760ccbca1b77b95c6120884fefcc4385f12614f9e49`  
		Last Modified: Thu, 09 Feb 2023 03:18:55 GMT  
		Size: 4.2 MB (4187743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1e21e6198268a646e1f41d15b44931dc2d1ffaf7448588af3237d7443de8df`  
		Last Modified: Thu, 09 Feb 2023 03:18:54 GMT  
		Size: 1.2 MB (1217832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86c409f0ecb7b6ab12d691c73e32350f6453fc6e477af6fe53ec7946e91ec08`  
		Last Modified: Thu, 09 Feb 2023 03:18:54 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2d6f2baed8a8d6af9014cc57d9488335fd4d9ded609476ce98307a241b55f680
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127387922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad435c186a3c6ffdd4910420eabfef5bbf8a84e247d2473ac2c1394e5ece3781`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:28:28 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:28:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:57:48 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:48 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:49 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:49:43 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:49:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:49:44 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:49:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:49:45 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:49:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:49:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:49:47 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3919da799d44c7be2eecafbf780801f4cd562b289c55ebe566999525497cd24`  
		Last Modified: Mon, 09 Jan 2023 17:37:35 GMT  
		Size: 286.1 KB (286122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c266a9580739a5c56dffcd14ce61144c9f58539d8c927ccd3df332434ad8d57`  
		Last Modified: Wed, 11 Jan 2023 00:11:13 GMT  
		Size: 118.7 MB (118677328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9666a7ae960b29537b5e693ea358a6181a3b9b73110b1099f22596b2dedbe3bd`  
		Last Modified: Wed, 11 Jan 2023 00:10:50 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b71d65a08c2aecf44c515cedf0abefc5f896bd9942291a29ddcf6646452661`  
		Last Modified: Wed, 08 Feb 2023 23:50:58 GMT  
		Size: 4.2 MB (4150629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a427cd9f7efb7c150d196c96034cdc132bf3c26025a87378400da762842a4923`  
		Last Modified: Wed, 08 Feb 2023 23:50:57 GMT  
		Size: 1.2 MB (1166069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278f59186f97ea59dd8a5f727fe7b3e2aa46b384971583b5b277b871a61b2131`  
		Last Modified: Wed, 08 Feb 2023 23:50:57 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:ad4dce5e6c2c07e73c35c50cdc26e110c439a947f626c86482c0bc5165ad8d9e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126503260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be8c29fce7791d265104052e6900b3eca71a13aa0b77861ded3aac664b4e9ae7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:04:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 10 Jan 2023 01:04:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:59:19 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:02:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:02:06 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:02:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:02:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:02:08 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:57:41 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:57:42 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:57:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:57:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:57:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c7609f223a73f5c1097b3b7cb1ea29e1e540da920bc3b48b8672a1d5ef1dc9`  
		Last Modified: Tue, 10 Jan 2023 01:13:57 GMT  
		Size: 285.4 KB (285359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da97c3a81e19449c60385f1e4cf4fd4fc9ffd14d08a26ccb6782cafd2d5d6f66`  
		Last Modified: Wed, 11 Jan 2023 00:15:15 GMT  
		Size: 118.5 MB (118468701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e98750b6aa4570218317d53b00f803a47aff7219e78c594d1666eef08e0258`  
		Last Modified: Wed, 11 Jan 2023 00:14:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ffc027d61bfbcc1c13359e022e0e4e6a5ef7cf40c49a8979e7d2f2a40add601`  
		Last Modified: Wed, 08 Feb 2023 23:58:48 GMT  
		Size: 3.7 MB (3720136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c82d9a2e5d63888f8bbe98b76b4b3565ccc2c8ce45526e794fae5f54d98ba49`  
		Last Modified: Wed, 08 Feb 2023 23:58:48 GMT  
		Size: 1.2 MB (1163326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0730779ca73578c83a210e39877a270c4a66834bd12b23cf515389d07213ac72`  
		Last Modified: Wed, 08 Feb 2023 23:58:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:bddc4b456724f377099c6889de30e23e6b434d71153db528d9746fade979f0c8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125786646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4850c9ee7a87ef514c7c4e3c3773db8494849b1ba453095ffe6fc5df07f158b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:37:51 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:37:52 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:14 GMT
ENV GOLANG_VERSION=1.19.5
# Tue, 10 Jan 2023 23:59:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Jan 2023 23:59:24 GMT
ENV GOPATH=/go
# Tue, 10 Jan 2023 23:59:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:59:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 10 Jan 2023 23:59:25 GMT
WORKDIR /go
# Thu, 09 Feb 2023 03:57:02 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 03:57:02 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 03:57:03 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:57:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 03:57:03 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 03:57:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 03:57:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 03:57:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3aa66ae7ca151fbd33126b15fa4d01bd5ceb35d53de36a8c6c82ecde58b596`  
		Last Modified: Mon, 09 Jan 2023 17:42:45 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491d6e59a2be619159e6630fabdf81f0255c275176cd97d109fa2f417935d6a8`  
		Last Modified: Wed, 11 Jan 2023 00:06:29 GMT  
		Size: 116.9 MB (116882841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4d12be79e26ab534722d5e8e5c9d931ed5ebd84ded16cae4b12390bb543502`  
		Last Modified: Wed, 11 Jan 2023 00:06:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c89dffd73dee99c1e6d53d4ea8cc302fa2089ee3edef14dc51585b33986fc9`  
		Last Modified: Thu, 09 Feb 2023 03:57:40 GMT  
		Size: 4.2 MB (4234011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cfcadb2a14be80b0bad3d94a219fcb7e0889a821a54688bc4ca6f47b905d88`  
		Last Modified: Thu, 09 Feb 2023 03:57:39 GMT  
		Size: 1.1 MB (1123736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b4461ab8f854d2e2000cacc11f5ee723a0888222cbd031ae1d1f0ae14c3e94`  
		Last Modified: Thu, 09 Feb 2023 03:57:39 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:7805a8da1341b4d0a403cd79ce628ded1f59f183d0c9d1a736e8d898370ca860
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126524152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c705e4439b5eac8b98303529a2168b757e4fad96343a01659c151be8647f401f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:13 GMT
ADD file:9a1d27fdc0c915f387f2446c85193d5215b18020b313114f0bf2799efcc1baae in / 
# Mon, 09 Jan 2023 17:05:13 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:34:40 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 21:34:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:42 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:01:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:01:19 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:01:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:01:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:01:20 GMT
WORKDIR /go
# Thu, 09 Feb 2023 06:18:37 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 06:18:37 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 06:18:38 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 06:18:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 06:18:38 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 06:18:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 06:18:42 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 06:18:42 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f45bfda3aa14e255d9eb4c9a108eb3d8c6721946b4aa2e5808e5092242344a1c`  
		Last Modified: Mon, 09 Jan 2023 17:05:56 GMT  
		Size: 3.4 MB (3384562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ab1c47929aa42b49b577230cb740bcf3e8aebc5abb60aabb4e6ee296dc2cad`  
		Last Modified: Mon, 09 Jan 2023 21:44:30 GMT  
		Size: 286.6 KB (286647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ded0f2fb726423b204889105ff334f3133acd9bbd8a5edfddad43e6e904485`  
		Last Modified: Wed, 11 Jan 2023 00:14:05 GMT  
		Size: 117.3 MB (117267319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c616b872c15882d15d49d081ce173bb6fa4e0f36ffead4b1938923db8038bd`  
		Last Modified: Wed, 11 Jan 2023 00:13:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e47ce9bd35950f8803ed14aa1fe38b85865479ec312ffa8b32df18b26add09`  
		Last Modified: Thu, 09 Feb 2023 06:19:42 GMT  
		Size: 4.5 MB (4479174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e8d19e2da6aa4d4205abf9c47ab0c45f001d2f8af00e99eb2bd7fec2852519`  
		Last Modified: Thu, 09 Feb 2023 06:19:41 GMT  
		Size: 1.1 MB (1105889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb53e3916ae4f3ac3cd8e441e2276b18484cf30de7a4f7b9ccb908933cd7502a`  
		Last Modified: Thu, 09 Feb 2023 06:19:41 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:3fa0a9eed3f7aaac0dbb713789109e64e4a585c7a9293211ecacc1d944b973be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129575744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a22f7e76fad31ed672b8977ea04a84eb19571daac58c337bd73a5c173ceecc6b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:44 GMT
ADD file:eabe7c3c368e65478b53ac35c1daf3b703f2bca4ecdab2d080a65e8b981d7d4a in / 
# Mon, 09 Jan 2023 17:05:46 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:42:43 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:42:43 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:53 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:56 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:57 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:41:57 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:41:58 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:42:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:42:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:42:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ae982806674c51a962c0fdd6e19f464ebd673df529c5cfb7c1d049e0b618d384`  
		Last Modified: Mon, 09 Jan 2023 17:06:50 GMT  
		Size: 3.2 MB (3170744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a5579d5fa8a33df30a972596fba4f03e76edabd19e57e62163b9c717fc188f`  
		Last Modified: Mon, 09 Jan 2023 17:54:33 GMT  
		Size: 285.0 KB (285022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4535e632f08f4af238fcccc27545520d10696aa3ce5920e33ba5578c3ee0e23`  
		Last Modified: Wed, 11 Jan 2023 00:12:31 GMT  
		Size: 120.8 MB (120785530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7633b4de83c59883de617e4ab5c606af3c556d6de4e45337bc59bff5bf7fe8ee`  
		Last Modified: Wed, 11 Jan 2023 00:12:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54414a7d37854703b1d037b805f6d0a49d2d398794414e3cedd1507c4bff0b82`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 4.2 MB (4163474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1779d1179e942debc68a6641287b6503a7e6949318c9272acb0273d7947d66e7`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 1.2 MB (1170413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597462f6847e463140e07072d10801a4c80c146d229deb04ef5cbc8b6f043464`  
		Last Modified: Wed, 08 Feb 2023 23:42:50 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.3887; amd64

```console
$ docker pull caddy@sha256:feeef34c537e9ea177fbaddb84e47df2e84a5cce70f7c8e3730e41822897b57e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1893070742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14ec5079fc868b1ce19abdcd6fca0964fae438be489b78914e21eac77dee89b3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 03:01:55 GMT
ENV GIT_VERSION=2.23.0
# Thu, 12 Jan 2023 03:01:56 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 12 Jan 2023 03:01:57 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 12 Jan 2023 03:01:58 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 12 Jan 2023 03:02:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:03:01 GMT
ENV GOPATH=C:\go
# Thu, 12 Jan 2023 03:03:35 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 Jan 2023 03:20:09 GMT
ENV GOLANG_VERSION=1.19.5
# Thu, 12 Jan 2023 03:23:52 GMT
RUN $url = 'https://dl.google.com/go/go1.19.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '167db91a2e40aeb453d3e59d213ecab06f62e1c4a84d13a06ccda1d999961caa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:23:54 GMT
WORKDIR C:\go
# Thu, 12 Jan 2023 05:33:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:19:59 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 00:20:00 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:20:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 00:20:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Feb 2023 00:20:35 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203425975bec1802428fad91a2e5f01172b161062c12eddf729e548bf7e134e0`  
		Last Modified: Thu, 12 Jan 2023 03:48:09 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80e42e19ab862b4adea06f1995e1f5cbb2c11ad8d68ae4a7bb5d0da5d0e6f38`  
		Last Modified: Thu, 12 Jan 2023 03:48:06 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be5d5df8cec6d1386f78a342668c3d2cb809372865459c1b35aa8d5a39a463b`  
		Last Modified: Thu, 12 Jan 2023 03:48:06 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e467d553c4972b55bf8e3d80b16f245e5bb38f28d80b91ca4f9f90c09a6c28d`  
		Last Modified: Thu, 12 Jan 2023 03:48:05 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97054b77b205167acd5a303c8aa82e380f090ff4e2ded81d3425ec78500139d`  
		Last Modified: Thu, 12 Jan 2023 03:48:14 GMT  
		Size: 25.5 MB (25470784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e150d9e1a1da09e17313cb3b6358d2f16cf2919c51e9addf30500de9d03292ef`  
		Last Modified: Thu, 12 Jan 2023 03:48:03 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c0d792e2a7942826a61fdc26b6081ab404122751ff4f4dd8f5b8b0eca21399`  
		Last Modified: Thu, 12 Jan 2023 03:48:03 GMT  
		Size: 324.5 KB (324466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cdd2ff60bbafbd62e677e0798ee562e3c4b291b841c6d0904ca080220e132a`  
		Last Modified: Thu, 12 Jan 2023 03:52:14 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17e6f8c13d649cbaec88dcdd4b1de7b004cf19227fbb4f923bd031b6b57988f`  
		Last Modified: Thu, 12 Jan 2023 03:53:12 GMT  
		Size: 157.7 MB (157659743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29fbb32977b62254a5de7ced98fe2a21e0342aa9db7b3cf32be4013d96b2cd9`  
		Last Modified: Thu, 12 Jan 2023 03:52:14 GMT  
		Size: 1.6 KB (1563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2fbb7e05d875affd4596aa7b87572980a3ab74800cff17a34deb445bed71b8`  
		Last Modified: Thu, 12 Jan 2023 05:36:53 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edae42a55d8aaff06e33b6f9ac104d54771346e5f4f59afd8ce90c794716611a`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb86a1e32dd5f27c1ba5ed4c675ff8c1477230677af11f17c75379385bd990b4`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d846d73e8be9adf7269d7376adebc7a8e8706b560a5f0d67886ab98c1d00c233`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2d31296154ed152465faac00831500590d35be69015063bb3ae3cc3514575d`  
		Last Modified: Thu, 09 Feb 2023 01:17:38 GMT  
		Size: 1.7 MB (1653847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef57a9413d8bab4ab7212470d9ac2b9eafc5efb5dc44aef718c91f935daddce`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.20348.1487; amd64

```console
$ docker pull caddy@sha256:e288b33447f0b01c2ee0954c57e574b43ce9ed4b56cbd813eca3cb1df8d9f766
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1572061864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c236dcd08d81ed31367d57c62c7e77e2421092030cd5365c6a225b0ad121c6b5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 02:57:40 GMT
ENV GIT_VERSION=2.23.0
# Thu, 12 Jan 2023 02:57:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 12 Jan 2023 02:57:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 12 Jan 2023 02:57:42 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 12 Jan 2023 02:58:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 02:58:23 GMT
ENV GOPATH=C:\go
# Thu, 12 Jan 2023 02:58:47 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 Jan 2023 03:16:17 GMT
ENV GOLANG_VERSION=1.19.5
# Thu, 12 Jan 2023 03:19:43 GMT
RUN $url = 'https://dl.google.com/go/go1.19.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '167db91a2e40aeb453d3e59d213ecab06f62e1c4a84d13a06ccda1d999961caa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:19:45 GMT
WORKDIR C:\go
# Thu, 12 Jan 2023 05:34:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:20:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 00:20:47 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:20:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 00:21:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Feb 2023 00:21:22 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2fc8728d9c7bf65edf893fd902f8b1bd780f93623858960c9db79e39922b169`  
		Last Modified: Thu, 12 Jan 2023 03:47:24 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7935a4c648078e79f67a11bcd5908e251110dd6c5a4ee49a607f332dd25af9`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d257f8b122044547f89f00f58661b25aca97c92f3831e7aaa11975639b6e35d4`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95acaa75c1852ba1320c5db382b01f587badb615b6746b59be27eedcf96ab667`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5201ba65043fa621c187729f18aecf4c549cdfa12cd6d8cab7a901d893f3a8a8`  
		Last Modified: Thu, 12 Jan 2023 03:47:29 GMT  
		Size: 25.7 MB (25702230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a317a349bca5ab28ba7c1ce039928a56390f7e7a8d7ddec07efcc1c9883e5d`  
		Last Modified: Thu, 12 Jan 2023 03:47:18 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8850296b8fbb853a6eb6341f7484cd4bc622e9f679f12c4123eddf08b7f398fb`  
		Last Modified: Thu, 12 Jan 2023 03:47:18 GMT  
		Size: 554.2 KB (554212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80b3d62f45a345eaac7caba0cdc514011cc61ea8f9d7d7b82d1bd4f8f3dbea4`  
		Last Modified: Thu, 12 Jan 2023 03:50:53 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320dc1bc3ac081a72fbca97a699b20068d92c70b3caaec8ca53036ab37509933`  
		Last Modified: Thu, 12 Jan 2023 03:51:58 GMT  
		Size: 157.9 MB (157885976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230636fcbea662dc69129c73285f4376c0b83a3222e8d438ec859d14ee1201b8`  
		Last Modified: Thu, 12 Jan 2023 03:50:53 GMT  
		Size: 1.6 KB (1569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581e22afffddeddb0a4127481e5016946bd3f35379291c6bb1e3b85e92e7acef`  
		Last Modified: Thu, 12 Jan 2023 05:37:10 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13aaa30213dc8e6b5906114a862d8398ac157fd2f8c835767a058069f180a181`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b39a2446c556432e7503cc419fe42c4d14ff3fc744cf6d475136c5058bc18d6`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43ea60403f6819d31f67d7dc2d230def090cb6366c7cd272d99d8d06aac019d`  
		Last Modified: Thu, 09 Feb 2023 01:17:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5970b711fddee53f278567276c42d2b169c5286a5133ba48ce3a599b253b37ab`  
		Last Modified: Thu, 09 Feb 2023 01:17:55 GMT  
		Size: 1.9 MB (1871861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1270e653c78ffbadd8ab6379e16db4c45c20fb148d294ec9654f1d13367fea6`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:e6c08f0694b44abd7ae623da15e368a4828a38cae59c041ab8f55c750fc66351
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
$ docker pull caddy@sha256:b86e1de154ca5d11618a408742e2b6f16f99e55cdc0ee97fe0965da9f1b1572f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131390128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:858147920561fe47255b181692d82558dbab931f4393f33ba8697b9c647f690e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:50:11 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:50:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:23 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:01 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:02 GMT
WORKDIR /go
# Thu, 09 Feb 2023 03:18:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 03:18:17 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 03:18:17 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 03:18:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 03:18:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 03:18:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f8637abd914a8a62416e027a351293d0472bc4b4f44383c6f425fd0e03861c`  
		Last Modified: Mon, 09 Jan 2023 17:56:43 GMT  
		Size: 284.8 KB (284814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48e7ca896ec974241d86439d34188186e085705e42d914d8b7757c27eea8613`  
		Last Modified: Wed, 11 Jan 2023 00:08:38 GMT  
		Size: 122.3 MB (122328552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f26d270037d8578282b40f86c0a1816fc5d034d6213f7dcab8440056a589309`  
		Last Modified: Wed, 11 Jan 2023 00:08:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807cf12e90d621962959f760ccbca1b77b95c6120884fefcc4385f12614f9e49`  
		Last Modified: Thu, 09 Feb 2023 03:18:55 GMT  
		Size: 4.2 MB (4187743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1e21e6198268a646e1f41d15b44931dc2d1ffaf7448588af3237d7443de8df`  
		Last Modified: Thu, 09 Feb 2023 03:18:54 GMT  
		Size: 1.2 MB (1217832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86c409f0ecb7b6ab12d691c73e32350f6453fc6e477af6fe53ec7946e91ec08`  
		Last Modified: Thu, 09 Feb 2023 03:18:54 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2d6f2baed8a8d6af9014cc57d9488335fd4d9ded609476ce98307a241b55f680
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127387922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad435c186a3c6ffdd4910420eabfef5bbf8a84e247d2473ac2c1394e5ece3781`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:28:28 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:28:28 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:57:48 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:48 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:48 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:49 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:49 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:49:43 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:49:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:49:44 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:49:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:49:45 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:49:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:49:47 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:49:47 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3919da799d44c7be2eecafbf780801f4cd562b289c55ebe566999525497cd24`  
		Last Modified: Mon, 09 Jan 2023 17:37:35 GMT  
		Size: 286.1 KB (286122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c266a9580739a5c56dffcd14ce61144c9f58539d8c927ccd3df332434ad8d57`  
		Last Modified: Wed, 11 Jan 2023 00:11:13 GMT  
		Size: 118.7 MB (118677328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9666a7ae960b29537b5e693ea358a6181a3b9b73110b1099f22596b2dedbe3bd`  
		Last Modified: Wed, 11 Jan 2023 00:10:50 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b71d65a08c2aecf44c515cedf0abefc5f896bd9942291a29ddcf6646452661`  
		Last Modified: Wed, 08 Feb 2023 23:50:58 GMT  
		Size: 4.2 MB (4150629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a427cd9f7efb7c150d196c96034cdc132bf3c26025a87378400da762842a4923`  
		Last Modified: Wed, 08 Feb 2023 23:50:57 GMT  
		Size: 1.2 MB (1166069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278f59186f97ea59dd8a5f727fe7b3e2aa46b384971583b5b277b871a61b2131`  
		Last Modified: Wed, 08 Feb 2023 23:50:57 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:ad4dce5e6c2c07e73c35c50cdc26e110c439a947f626c86482c0bc5165ad8d9e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126503260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be8c29fce7791d265104052e6900b3eca71a13aa0b77861ded3aac664b4e9ae7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 10 Jan 2023 01:04:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 10 Jan 2023 01:04:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:59:19 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:02:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:02:06 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:02:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:02:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:02:08 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:57:41 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:57:42 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:57:42 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:57:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:57:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:57:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c7609f223a73f5c1097b3b7cb1ea29e1e540da920bc3b48b8672a1d5ef1dc9`  
		Last Modified: Tue, 10 Jan 2023 01:13:57 GMT  
		Size: 285.4 KB (285359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da97c3a81e19449c60385f1e4cf4fd4fc9ffd14d08a26ccb6782cafd2d5d6f66`  
		Last Modified: Wed, 11 Jan 2023 00:15:15 GMT  
		Size: 118.5 MB (118468701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e98750b6aa4570218317d53b00f803a47aff7219e78c594d1666eef08e0258`  
		Last Modified: Wed, 11 Jan 2023 00:14:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ffc027d61bfbcc1c13359e022e0e4e6a5ef7cf40c49a8979e7d2f2a40add601`  
		Last Modified: Wed, 08 Feb 2023 23:58:48 GMT  
		Size: 3.7 MB (3720136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c82d9a2e5d63888f8bbe98b76b4b3565ccc2c8ce45526e794fae5f54d98ba49`  
		Last Modified: Wed, 08 Feb 2023 23:58:48 GMT  
		Size: 1.2 MB (1163326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0730779ca73578c83a210e39877a270c4a66834bd12b23cf515389d07213ac72`  
		Last Modified: Wed, 08 Feb 2023 23:58:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:bddc4b456724f377099c6889de30e23e6b434d71153db528d9746fade979f0c8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125786646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4850c9ee7a87ef514c7c4e3c3773db8494849b1ba453095ffe6fc5df07f158b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:37:51 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:37:52 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:14 GMT
ENV GOLANG_VERSION=1.19.5
# Tue, 10 Jan 2023 23:59:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 10 Jan 2023 23:59:24 GMT
ENV GOPATH=/go
# Tue, 10 Jan 2023 23:59:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:59:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 10 Jan 2023 23:59:25 GMT
WORKDIR /go
# Thu, 09 Feb 2023 03:57:02 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 03:57:02 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 03:57:03 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:57:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 03:57:03 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 03:57:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 03:57:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 03:57:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3aa66ae7ca151fbd33126b15fa4d01bd5ceb35d53de36a8c6c82ecde58b596`  
		Last Modified: Mon, 09 Jan 2023 17:42:45 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491d6e59a2be619159e6630fabdf81f0255c275176cd97d109fa2f417935d6a8`  
		Last Modified: Wed, 11 Jan 2023 00:06:29 GMT  
		Size: 116.9 MB (116882841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4d12be79e26ab534722d5e8e5c9d931ed5ebd84ded16cae4b12390bb543502`  
		Last Modified: Wed, 11 Jan 2023 00:06:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c89dffd73dee99c1e6d53d4ea8cc302fa2089ee3edef14dc51585b33986fc9`  
		Last Modified: Thu, 09 Feb 2023 03:57:40 GMT  
		Size: 4.2 MB (4234011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cfcadb2a14be80b0bad3d94a219fcb7e0889a821a54688bc4ca6f47b905d88`  
		Last Modified: Thu, 09 Feb 2023 03:57:39 GMT  
		Size: 1.1 MB (1123736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b4461ab8f854d2e2000cacc11f5ee723a0888222cbd031ae1d1f0ae14c3e94`  
		Last Modified: Thu, 09 Feb 2023 03:57:39 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:7805a8da1341b4d0a403cd79ce628ded1f59f183d0c9d1a736e8d898370ca860
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126524152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c705e4439b5eac8b98303529a2168b757e4fad96343a01659c151be8647f401f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:13 GMT
ADD file:9a1d27fdc0c915f387f2446c85193d5215b18020b313114f0bf2799efcc1baae in / 
# Mon, 09 Jan 2023 17:05:13 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:34:40 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 21:34:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:42 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:01:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:01:19 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:01:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:01:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:01:20 GMT
WORKDIR /go
# Thu, 09 Feb 2023 06:18:37 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 09 Feb 2023 06:18:37 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 06:18:38 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 06:18:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 06:18:38 GMT
ENV XCADDY_SETCAP=1
# Thu, 09 Feb 2023 06:18:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Feb 2023 06:18:42 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Feb 2023 06:18:42 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f45bfda3aa14e255d9eb4c9a108eb3d8c6721946b4aa2e5808e5092242344a1c`  
		Last Modified: Mon, 09 Jan 2023 17:05:56 GMT  
		Size: 3.4 MB (3384562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ab1c47929aa42b49b577230cb740bcf3e8aebc5abb60aabb4e6ee296dc2cad`  
		Last Modified: Mon, 09 Jan 2023 21:44:30 GMT  
		Size: 286.6 KB (286647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ded0f2fb726423b204889105ff334f3133acd9bbd8a5edfddad43e6e904485`  
		Last Modified: Wed, 11 Jan 2023 00:14:05 GMT  
		Size: 117.3 MB (117267319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c616b872c15882d15d49d081ce173bb6fa4e0f36ffead4b1938923db8038bd`  
		Last Modified: Wed, 11 Jan 2023 00:13:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e47ce9bd35950f8803ed14aa1fe38b85865479ec312ffa8b32df18b26add09`  
		Last Modified: Thu, 09 Feb 2023 06:19:42 GMT  
		Size: 4.5 MB (4479174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e8d19e2da6aa4d4205abf9c47ab0c45f001d2f8af00e99eb2bd7fec2852519`  
		Last Modified: Thu, 09 Feb 2023 06:19:41 GMT  
		Size: 1.1 MB (1105889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb53e3916ae4f3ac3cd8e441e2276b18484cf30de7a4f7b9ccb908933cd7502a`  
		Last Modified: Thu, 09 Feb 2023 06:19:41 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:3fa0a9eed3f7aaac0dbb713789109e64e4a585c7a9293211ecacc1d944b973be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129575744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a22f7e76fad31ed672b8977ea04a84eb19571daac58c337bd73a5c173ceecc6b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:44 GMT
ADD file:eabe7c3c368e65478b53ac35c1daf3b703f2bca4ecdab2d080a65e8b981d7d4a in / 
# Mon, 09 Jan 2023 17:05:46 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:42:43 GMT
RUN apk add --no-cache ca-certificates
# Mon, 09 Jan 2023 17:42:43 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Jan 2023 23:58:53 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:00:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.5.src.tar.gz'; 		sha256='8e486e8e85a281fc5ce3f0bedc5b9d2dbf6276d7db0b25d3ec034f313da0375f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 11 Jan 2023 00:00:56 GMT
ENV GOPATH=/go
# Wed, 11 Jan 2023 00:00:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 00:00:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 11 Jan 2023 00:00:57 GMT
WORKDIR /go
# Wed, 08 Feb 2023 23:41:57 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 08 Feb 2023 23:41:58 GMT
ENV CADDY_VERSION=v2.6.3
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 08 Feb 2023 23:41:58 GMT
ENV XCADDY_SETCAP=1
# Wed, 08 Feb 2023 23:42:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 08 Feb 2023 23:42:00 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 08 Feb 2023 23:42:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:ae982806674c51a962c0fdd6e19f464ebd673df529c5cfb7c1d049e0b618d384`  
		Last Modified: Mon, 09 Jan 2023 17:06:50 GMT  
		Size: 3.2 MB (3170744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a5579d5fa8a33df30a972596fba4f03e76edabd19e57e62163b9c717fc188f`  
		Last Modified: Mon, 09 Jan 2023 17:54:33 GMT  
		Size: 285.0 KB (285022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4535e632f08f4af238fcccc27545520d10696aa3ce5920e33ba5578c3ee0e23`  
		Last Modified: Wed, 11 Jan 2023 00:12:31 GMT  
		Size: 120.8 MB (120785530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7633b4de83c59883de617e4ab5c606af3c556d6de4e45337bc59bff5bf7fe8ee`  
		Last Modified: Wed, 11 Jan 2023 00:12:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54414a7d37854703b1d037b805f6d0a49d2d398794414e3cedd1507c4bff0b82`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 4.2 MB (4163474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1779d1179e942debc68a6641287b6503a7e6949318c9272acb0273d7947d66e7`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 1.2 MB (1170413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597462f6847e463140e07072d10801a4c80c146d229deb04ef5cbc8b6f043464`  
		Last Modified: Wed, 08 Feb 2023 23:42:50 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:4c57090f03b98d1a89618055d77e7e8864830bf83840fd17b1228bfa3cc8db4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull caddy@sha256:feeef34c537e9ea177fbaddb84e47df2e84a5cce70f7c8e3730e41822897b57e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1893070742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14ec5079fc868b1ce19abdcd6fca0964fae438be489b78914e21eac77dee89b3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 03:01:55 GMT
ENV GIT_VERSION=2.23.0
# Thu, 12 Jan 2023 03:01:56 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 12 Jan 2023 03:01:57 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 12 Jan 2023 03:01:58 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 12 Jan 2023 03:02:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:03:01 GMT
ENV GOPATH=C:\go
# Thu, 12 Jan 2023 03:03:35 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 Jan 2023 03:20:09 GMT
ENV GOLANG_VERSION=1.19.5
# Thu, 12 Jan 2023 03:23:52 GMT
RUN $url = 'https://dl.google.com/go/go1.19.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '167db91a2e40aeb453d3e59d213ecab06f62e1c4a84d13a06ccda1d999961caa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:23:54 GMT
WORKDIR C:\go
# Thu, 12 Jan 2023 05:33:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:19:59 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 00:20:00 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:20:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 00:20:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Feb 2023 00:20:35 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203425975bec1802428fad91a2e5f01172b161062c12eddf729e548bf7e134e0`  
		Last Modified: Thu, 12 Jan 2023 03:48:09 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80e42e19ab862b4adea06f1995e1f5cbb2c11ad8d68ae4a7bb5d0da5d0e6f38`  
		Last Modified: Thu, 12 Jan 2023 03:48:06 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be5d5df8cec6d1386f78a342668c3d2cb809372865459c1b35aa8d5a39a463b`  
		Last Modified: Thu, 12 Jan 2023 03:48:06 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e467d553c4972b55bf8e3d80b16f245e5bb38f28d80b91ca4f9f90c09a6c28d`  
		Last Modified: Thu, 12 Jan 2023 03:48:05 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97054b77b205167acd5a303c8aa82e380f090ff4e2ded81d3425ec78500139d`  
		Last Modified: Thu, 12 Jan 2023 03:48:14 GMT  
		Size: 25.5 MB (25470784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e150d9e1a1da09e17313cb3b6358d2f16cf2919c51e9addf30500de9d03292ef`  
		Last Modified: Thu, 12 Jan 2023 03:48:03 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c0d792e2a7942826a61fdc26b6081ab404122751ff4f4dd8f5b8b0eca21399`  
		Last Modified: Thu, 12 Jan 2023 03:48:03 GMT  
		Size: 324.5 KB (324466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cdd2ff60bbafbd62e677e0798ee562e3c4b291b841c6d0904ca080220e132a`  
		Last Modified: Thu, 12 Jan 2023 03:52:14 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17e6f8c13d649cbaec88dcdd4b1de7b004cf19227fbb4f923bd031b6b57988f`  
		Last Modified: Thu, 12 Jan 2023 03:53:12 GMT  
		Size: 157.7 MB (157659743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29fbb32977b62254a5de7ced98fe2a21e0342aa9db7b3cf32be4013d96b2cd9`  
		Last Modified: Thu, 12 Jan 2023 03:52:14 GMT  
		Size: 1.6 KB (1563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2fbb7e05d875affd4596aa7b87572980a3ab74800cff17a34deb445bed71b8`  
		Last Modified: Thu, 12 Jan 2023 05:36:53 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edae42a55d8aaff06e33b6f9ac104d54771346e5f4f59afd8ce90c794716611a`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb86a1e32dd5f27c1ba5ed4c675ff8c1477230677af11f17c75379385bd990b4`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d846d73e8be9adf7269d7376adebc7a8e8706b560a5f0d67886ab98c1d00c233`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2d31296154ed152465faac00831500590d35be69015063bb3ae3cc3514575d`  
		Last Modified: Thu, 09 Feb 2023 01:17:38 GMT  
		Size: 1.7 MB (1653847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef57a9413d8bab4ab7212470d9ac2b9eafc5efb5dc44aef718c91f935daddce`  
		Last Modified: Thu, 09 Feb 2023 01:17:37 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:5016a9ee6f22300f4699ec2ba33c105b273e55c4b6931dcdbe8a7326d9dc037a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1487; amd64

### `caddy:builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1487; amd64

```console
$ docker pull caddy@sha256:e288b33447f0b01c2ee0954c57e574b43ce9ed4b56cbd813eca3cb1df8d9f766
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1572061864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c236dcd08d81ed31367d57c62c7e77e2421092030cd5365c6a225b0ad121c6b5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 02:57:40 GMT
ENV GIT_VERSION=2.23.0
# Thu, 12 Jan 2023 02:57:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 12 Jan 2023 02:57:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 12 Jan 2023 02:57:42 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 12 Jan 2023 02:58:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 02:58:23 GMT
ENV GOPATH=C:\go
# Thu, 12 Jan 2023 02:58:47 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 Jan 2023 03:16:17 GMT
ENV GOLANG_VERSION=1.19.5
# Thu, 12 Jan 2023 03:19:43 GMT
RUN $url = 'https://dl.google.com/go/go1.19.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '167db91a2e40aeb453d3e59d213ecab06f62e1c4a84d13a06ccda1d999961caa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 03:19:45 GMT
WORKDIR C:\go
# Thu, 12 Jan 2023 05:34:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:20:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 09 Feb 2023 00:20:47 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:20:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Feb 2023 00:21:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Feb 2023 00:21:22 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2fc8728d9c7bf65edf893fd902f8b1bd780f93623858960c9db79e39922b169`  
		Last Modified: Thu, 12 Jan 2023 03:47:24 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7935a4c648078e79f67a11bcd5908e251110dd6c5a4ee49a607f332dd25af9`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d257f8b122044547f89f00f58661b25aca97c92f3831e7aaa11975639b6e35d4`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95acaa75c1852ba1320c5db382b01f587badb615b6746b59be27eedcf96ab667`  
		Last Modified: Thu, 12 Jan 2023 03:47:20 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5201ba65043fa621c187729f18aecf4c549cdfa12cd6d8cab7a901d893f3a8a8`  
		Last Modified: Thu, 12 Jan 2023 03:47:29 GMT  
		Size: 25.7 MB (25702230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a317a349bca5ab28ba7c1ce039928a56390f7e7a8d7ddec07efcc1c9883e5d`  
		Last Modified: Thu, 12 Jan 2023 03:47:18 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8850296b8fbb853a6eb6341f7484cd4bc622e9f679f12c4123eddf08b7f398fb`  
		Last Modified: Thu, 12 Jan 2023 03:47:18 GMT  
		Size: 554.2 KB (554212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80b3d62f45a345eaac7caba0cdc514011cc61ea8f9d7d7b82d1bd4f8f3dbea4`  
		Last Modified: Thu, 12 Jan 2023 03:50:53 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320dc1bc3ac081a72fbca97a699b20068d92c70b3caaec8ca53036ab37509933`  
		Last Modified: Thu, 12 Jan 2023 03:51:58 GMT  
		Size: 157.9 MB (157885976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230636fcbea662dc69129c73285f4376c0b83a3222e8d438ec859d14ee1201b8`  
		Last Modified: Thu, 12 Jan 2023 03:50:53 GMT  
		Size: 1.6 KB (1569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581e22afffddeddb0a4127481e5016946bd3f35379291c6bb1e3b85e92e7acef`  
		Last Modified: Thu, 12 Jan 2023 05:37:10 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13aaa30213dc8e6b5906114a862d8398ac157fd2f8c835767a058069f180a181`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b39a2446c556432e7503cc419fe42c4d14ff3fc744cf6d475136c5058bc18d6`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43ea60403f6819d31f67d7dc2d230def090cb6366c7cd272d99d8d06aac019d`  
		Last Modified: Thu, 09 Feb 2023 01:17:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5970b711fddee53f278567276c42d2b169c5286a5133ba48ce3a599b253b37ab`  
		Last Modified: Thu, 09 Feb 2023 01:17:55 GMT  
		Size: 1.9 MB (1871861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1270e653c78ffbadd8ab6379e16db4c45c20fb148d294ec9654f1d13367fea6`  
		Last Modified: Thu, 09 Feb 2023 01:17:54 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:d34a689107f831d1fb6dfb92ce4cff1569e409e5b6dcd2d671d4ffee8b112b76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3887; amd64
	-	windows version 10.0.20348.1487; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:cf66a65d5667b26ba91fab680b59d421266e5042d4191fcdeab3847b31828bf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17441779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:739163e8bd53961abf96cc4f327498332dd905a59d3314fab80a845e62b58f9b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Thu, 09 Feb 2023 03:18:05 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 09 Feb 2023 03:18:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 09 Feb 2023 03:18:06 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 03:18:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 09 Feb 2023 03:18:10 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 09 Feb 2023 03:18:10 GMT
ENV XDG_DATA_HOME=/data
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 03:18:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 03:18:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 80
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 443
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 03:18:11 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 03:18:11 GMT
WORKDIR /srv
# Thu, 09 Feb 2023 03:18:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4cf81513fab9758787dbde95dcab4c054bd04137581b68097595a719ae973c`  
		Last Modified: Thu, 09 Feb 2023 03:18:39 GMT  
		Size: 351.2 KB (351181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c3f44eb3bccaf2f5515331e12d4b940a5f6ad016d27f548e0c739d1f6aba66`  
		Last Modified: Thu, 09 Feb 2023 03:18:39 GMT  
		Size: 7.6 KB (7554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04314ed686e612bbb7606d6bacff938564f9b4f7e0dbc72afacd887b3c88afbd`  
		Last Modified: Thu, 09 Feb 2023 03:18:42 GMT  
		Size: 14.3 MB (14276772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e4444abb42ab384f9685f3b25765ed65d8e07daef954ccf7aa73a524a2177064
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16576623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99391525993d815548f2a8e80455bb1ff1b6dd0a769a0dc2a467cbcc3adbc1ad`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:32 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Fri, 10 Feb 2023 20:49:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:28:54 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 21:28:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Fri, 10 Feb 2023 21:28:56 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 21:28:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 21:28:59 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 21:28:59 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 21:28:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 21:29:00 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 80
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 443
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 21:29:00 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 21:29:00 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 21:29:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a400dcba29ff44f8e5bf01493def4f19629aca6d103cb2a66ca87c457f7414`  
		Last Modified: Fri, 10 Feb 2023 21:29:47 GMT  
		Size: 345.8 KB (345811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b946768825eb5ed2fc6f932fdb0b0c552f4c35c39dada07eddd70ce4a535953`  
		Last Modified: Fri, 10 Feb 2023 21:29:47 GMT  
		Size: 7.5 KB (7480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda323f820516b366c61a02ba4cfd00cc3a3b6cc9051c58e7359057dea842d8a`  
		Last Modified: Fri, 10 Feb 2023 21:29:51 GMT  
		Size: 13.6 MB (13606554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0a66f97fe167ebcccd1754f2cc7ed8d5f42595f332f60d75e4efd33c5fa880b9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16362110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0940efa30038d45d9b6cbae2aea1235accdd5e653948a6e40e9c3edf6314d4c6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:37:19 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:37:22 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Fri, 10 Feb 2023 22:37:22 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:37:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:37:26 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:37:27 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:37:27 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:37:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:37:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:37:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:37:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:37:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:37:30 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:37:30 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:37:31 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:37:31 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:37:31 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:37:32 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec2ab4edb1f0a14b28a55f050d62d8e54111075639a0fa8f173448814ba0d00`  
		Last Modified: Fri, 10 Feb 2023 22:38:25 GMT  
		Size: 342.6 KB (342588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0580184dd0082f009564a7a3923731f202cbe4bd8b857dbca2c77da8e7434815`  
		Last Modified: Fri, 10 Feb 2023 22:38:25 GMT  
		Size: 7.5 KB (7479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b2a44f2792add2104a1d53c68f1df95779deaee3ec86717f4fb4efd9aa6aaa`  
		Last Modified: Fri, 10 Feb 2023 22:38:28 GMT  
		Size: 13.6 MB (13591549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:4be5e6cdfb930681cc9c4722b0af67e75e53f0cff56c916c1d618eb39d6f5169
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16126925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:995c31e78c533c3ca73152cb87130dfcb16842dd052ab384df917fb755c5dc43`
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
# Fri, 10 Feb 2023 22:00:37 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:00:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:00:39 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:00:39 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:00:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:00:40 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:00:40 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:00:40 GMT
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
	-	`sha256:6403d7bb9250089f4077bba7631d975f97648fbcd782c992704ff3bccc5ae421`  
		Last Modified: Fri, 10 Feb 2023 22:01:03 GMT  
		Size: 13.1 MB (13059715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:50a289625f0ef1adfc05773b5ec8a30f001be347a84f24e1106e351f230758b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15949909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b11b3ee451004883e1f9089fc132ee1ecc849a2d96ef0ff4731334c8279cfa`
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
# Fri, 10 Feb 2023 22:13:23 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:13:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:13:28 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:13:28 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:13:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:13:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:13:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:13:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:13:32 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:13:33 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:13:33 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:13:33 GMT
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
	-	`sha256:2ecc7ec17344834a2337d83b9b7be44f97f0c0b55dfea5e1d8af80c8d5c32221`  
		Last Modified: Fri, 10 Feb 2023 22:14:19 GMT  
		Size: 12.8 MB (12774635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:9c69a670bfaa4e7166553c41a7303b114a524eed38924ad0d1d5599e6b7b2463
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16787086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9abb18c28ea7e824ff4385016f24b30d1a455d1b902f8667a1a9300078826a`
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
# Fri, 10 Feb 2023 22:14:19 GMT
ENV CADDY_VERSION=v2.6.3
# Fri, 10 Feb 2023 22:14:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='788fd38ad7b600f0b4bf6d0493da1b319f9b9fcb9099693b4fefed9ab6d8f007fb438ae082c46dc12abc4dacb467d7dbdf4cc200819aa4a502d8b47b805fea1b' ;; 		armhf)   binArch='armv6'; checksum='a5b3ab1b8d8e637c87ca2b5ed0e9bed28d4fe3fc214aad94212253098cd6d121453f3c325d2b27ec87bb84300daf2a9f2145948a7bf85573ca3f90ea9bca4c18' ;; 		armv7)   binArch='armv7'; checksum='4e060e33ffcaf60bd70216618d71379be0add74ee9ede7867934ff61b1412915e468c7a9a478fa302ae7c270fbb0d9e6609afcf52841cf6ea9394e11a8216741' ;; 		aarch64) binArch='arm64'; checksum='eafd3842a1df5900d46f4b0db0bcca2cc598ecd5beb555e14a15e0df9984158de3b46f1595d3bd4264d7094a0681be1f38c0dbad4e125fc3ab0481881636199a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1b898890e1d9e46b93b740ac1af9d96232f7fbab1e0bbc94505626e7f6ce00150ed8c7b5117f076e8c11664c65fa4e39bea34e48ef75efd1a14c30d9b477e3ed' ;; 		s390x)   binArch='s390x'; checksum='5c1c4fcf13078a464aa6a15edc407b87f2dfd6da284abba8d895efcfe195a8fd123da1e29c1c70629d1118fdf590e4c8970d3351623eac4da1cdd31a3b75a8b3' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 10 Feb 2023 22:14:21 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 10 Feb 2023 22:14:22 GMT
ENV XDG_DATA_HOME=/data
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 10 Feb 2023 22:14:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 80
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 443
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 443/udp
# Fri, 10 Feb 2023 22:14:23 GMT
EXPOSE 2019
# Fri, 10 Feb 2023 22:14:23 GMT
WORKDIR /srv
# Fri, 10 Feb 2023 22:14:23 GMT
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
	-	`sha256:94fd73a8831c9e57fdf8c430154c9adc56e54610a462128c8f0a1b3937aef704`  
		Last Modified: Fri, 10 Feb 2023 22:15:07 GMT  
		Size: 13.8 MB (13833147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.3887; amd64

```console
$ docker pull caddy@sha256:935d1f4349cc551dfe9b76d6ba5fe6355414519a3037a7689fe765033ae8dcd6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1723388621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1deb1aecac8501d9afe22abd2fc90f15552c63366f8016ad2e6d1602be5cdf6d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:16:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:16:36 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:17:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:17:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:17:21 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:17:22 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:17:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:17:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:17:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:17:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:17:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:17:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:17:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:17:31 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:17:32 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:17:33 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:17:34 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:17:53 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:17:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47af8a9c9ef8e49d65e53dd207ad0935ce7a2b50b2f253e6a5b037494ae19d0a`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 401.5 KB (401472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5841cb6343add9dd7b89906610425117976b050c0634eedbc5c38302aa024e`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d760049e5c9f1fb1d7ec05a3eea55088808f484912e87cda07f3709363fe3c2c`  
		Last Modified: Thu, 09 Feb 2023 01:16:53 GMT  
		Size: 14.7 MB (14680484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3239225b5bad52e6004b638bd356e7d29e7fded5d31d90541907e1a769a115`  
		Last Modified: Thu, 09 Feb 2023 01:16:49 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6823ad091829bc6d98a58a18b075e20c551bde81d504bdbfda09b5a3d7c5d0`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4873a8802163accb90dd2318bd05ddfa4f94692b2731d6e23095e3bb46b98fd`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabf39e152fd5c18e0c3ac503e054c36e2775512f9fa7bb11b9221442b2bc1fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af12dc4018ba87a8e25003874e2d8e959a25b1c19932553daec8f4c410ebd61f`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fefa1f82e39e2af863b13609d78d966746d852af0cea54dcb17f45a8386c39d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d5b41708aea61714f00bc0f35ea1efc60db85c04ab6754e4d6b4485dc59a28`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a8b1cf8bcc4175323f7feaa280e3122f03aa7f9d35666fcc55c6b7d1e628ae`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c3f865e552649c436d5ffc0f3c83a3b5ba3026b2cff2ab3f381a5cdf2e2f2`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201cfdbfc1583e2ea070418e6aad0ec6604fb52c68117460b1a4c5b511b56ecc`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef83199fb67566ea043dbf7fab6f54754a4d0496655be1157819973573247bb`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45db789a3d9786dea133341e2c9f16e14b23a664297ad7f9a371961a0c21588`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a4e021c112717a1fee7cd62cdc17d41521f3514f10bf8ec30457b95aaf44fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4c0327054bc1f199339822d4074ee176c4184b9357ec28d9250f27f0c12e26`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63a4d912695117a127068d20ceefbaa19e41c8a42d65788d37915d737d998d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:44 GMT  
		Size: 338.6 KB (338620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421719fbbf536a3651d6762e36406f19dd0b5601f4a300d9c47af9ccfa3573d2`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.20348.1487; amd64

```console
$ docker pull caddy@sha256:22cdfda624195707c05f1d681c1cdd97b504f06b282d981718e1b716b2dc6bfb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1401937005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca7c6af6ec202266d95f15726fee733430a631c6c4eddfd9cc7d000b817a0f19`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:18:43 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:18:44 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:19:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:19:16 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:19:17 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:19:18 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:19:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:19:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:19:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:19:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:19:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:19:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:19:26 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:19:27 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:19:29 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:19:30 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:19:47 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:19:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42eb48143612ee855d99c932e324b1bd035c60554117edeaa805402060613c51`  
		Last Modified: Thu, 09 Feb 2023 01:17:17 GMT  
		Size: 635.9 KB (635943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714ae92cb5dac0e72097d35b932125b5ea3f03214de78e03119a4517be6fd10`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a5533d3ddbff5ea35dbb0e11b10fe817ce3ef1a3fd7f44706cb1b6288e0406`  
		Last Modified: Thu, 09 Feb 2023 01:17:20 GMT  
		Size: 14.9 MB (14899830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e59c8f0dc8d987210bdfe89eaded536b0ef8ac727eb7d75b76aea9c296208a`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22bfc3588219a43ce294aab21751b407ae75504bf3ddcee69f42498672b6c46`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f7db57dc0a0b0126433f60d3d0005f9aaa0d405fe63cfc3b4e15388fdfa010`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7b9e3a2510b5ab3b7ac4103d653c8efd12e95b63327d5c5fb81b6ea341e2b5`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4109b3b0ca73b5355a12ee74b7c32b4015a6208fdb279fd0ab60074247e22309`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3c568a1866d44483984b2be40142a55371adf3b8dc991bdb5ab4c45c0be3d4`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6221c7c14444b318e798e231adeeb83ea155c157283e9def018c43415238aa7`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e81980463382095586f78276db5cd808400136543fc1a0f522af1f3eaee034`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f0d8afe85320b7cf4542ad649671660bbb8e74ec3ad3067408e79fb21dbf77`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7def0e2b3dd94a350c82bb6a4903fdfc65d1d3d9772dd8195a5eb14ba766c45`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0b51c8090bf08cc2ae3a9fc340c9b70ba1e077f32b7d7d025b7d9fb472d978`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3653016f515e293fc93892b9e021e05a6a183ad3dcdaf243311513e222534c7`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d1dafd3fbb7403b7f093ed63553863bd9904f6010b1b91f98d9bfba9c4d8bb`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92817327253aaae4d632a75ff38a01dbebfe11f9105c4db828c52f221262ce4`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43bce457643a143e82e49e57d9b8a69a416e254d2439f30d7e4dd25c84e43c0`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 348.1 KB (348138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a0e899ab4c995de79522a5022b8cca4765559a4de2d5c728821d947b497de1`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:0824e61dd8be6c1fa86bcf0faf1d4c5d8a41c047e0d4bf9ec8bbb73f243adaf6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3887; amd64
	-	windows version 10.0.20348.1487; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.3887; amd64

```console
$ docker pull caddy@sha256:935d1f4349cc551dfe9b76d6ba5fe6355414519a3037a7689fe765033ae8dcd6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1723388621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1deb1aecac8501d9afe22abd2fc90f15552c63366f8016ad2e6d1602be5cdf6d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:16:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:16:36 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:17:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:17:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:17:21 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:17:22 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:17:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:17:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:17:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:17:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:17:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:17:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:17:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:17:31 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:17:32 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:17:33 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:17:34 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:17:53 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:17:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47af8a9c9ef8e49d65e53dd207ad0935ce7a2b50b2f253e6a5b037494ae19d0a`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 401.5 KB (401472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5841cb6343add9dd7b89906610425117976b050c0634eedbc5c38302aa024e`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d760049e5c9f1fb1d7ec05a3eea55088808f484912e87cda07f3709363fe3c2c`  
		Last Modified: Thu, 09 Feb 2023 01:16:53 GMT  
		Size: 14.7 MB (14680484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3239225b5bad52e6004b638bd356e7d29e7fded5d31d90541907e1a769a115`  
		Last Modified: Thu, 09 Feb 2023 01:16:49 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6823ad091829bc6d98a58a18b075e20c551bde81d504bdbfda09b5a3d7c5d0`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4873a8802163accb90dd2318bd05ddfa4f94692b2731d6e23095e3bb46b98fd`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabf39e152fd5c18e0c3ac503e054c36e2775512f9fa7bb11b9221442b2bc1fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af12dc4018ba87a8e25003874e2d8e959a25b1c19932553daec8f4c410ebd61f`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fefa1f82e39e2af863b13609d78d966746d852af0cea54dcb17f45a8386c39d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d5b41708aea61714f00bc0f35ea1efc60db85c04ab6754e4d6b4485dc59a28`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a8b1cf8bcc4175323f7feaa280e3122f03aa7f9d35666fcc55c6b7d1e628ae`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c3f865e552649c436d5ffc0f3c83a3b5ba3026b2cff2ab3f381a5cdf2e2f2`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201cfdbfc1583e2ea070418e6aad0ec6604fb52c68117460b1a4c5b511b56ecc`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef83199fb67566ea043dbf7fab6f54754a4d0496655be1157819973573247bb`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45db789a3d9786dea133341e2c9f16e14b23a664297ad7f9a371961a0c21588`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a4e021c112717a1fee7cd62cdc17d41521f3514f10bf8ec30457b95aaf44fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4c0327054bc1f199339822d4074ee176c4184b9357ec28d9250f27f0c12e26`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63a4d912695117a127068d20ceefbaa19e41c8a42d65788d37915d737d998d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:44 GMT  
		Size: 338.6 KB (338620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421719fbbf536a3651d6762e36406f19dd0b5601f4a300d9c47af9ccfa3573d2`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.20348.1487; amd64

```console
$ docker pull caddy@sha256:22cdfda624195707c05f1d681c1cdd97b504f06b282d981718e1b716b2dc6bfb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1401937005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca7c6af6ec202266d95f15726fee733430a631c6c4eddfd9cc7d000b817a0f19`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:18:43 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:18:44 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:19:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:19:16 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:19:17 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:19:18 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:19:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:19:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:19:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:19:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:19:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:19:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:19:26 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:19:27 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:19:29 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:19:30 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:19:47 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:19:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42eb48143612ee855d99c932e324b1bd035c60554117edeaa805402060613c51`  
		Last Modified: Thu, 09 Feb 2023 01:17:17 GMT  
		Size: 635.9 KB (635943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714ae92cb5dac0e72097d35b932125b5ea3f03214de78e03119a4517be6fd10`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a5533d3ddbff5ea35dbb0e11b10fe817ce3ef1a3fd7f44706cb1b6288e0406`  
		Last Modified: Thu, 09 Feb 2023 01:17:20 GMT  
		Size: 14.9 MB (14899830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e59c8f0dc8d987210bdfe89eaded536b0ef8ac727eb7d75b76aea9c296208a`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22bfc3588219a43ce294aab21751b407ae75504bf3ddcee69f42498672b6c46`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f7db57dc0a0b0126433f60d3d0005f9aaa0d405fe63cfc3b4e15388fdfa010`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7b9e3a2510b5ab3b7ac4103d653c8efd12e95b63327d5c5fb81b6ea341e2b5`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4109b3b0ca73b5355a12ee74b7c32b4015a6208fdb279fd0ab60074247e22309`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3c568a1866d44483984b2be40142a55371adf3b8dc991bdb5ab4c45c0be3d4`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6221c7c14444b318e798e231adeeb83ea155c157283e9def018c43415238aa7`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e81980463382095586f78276db5cd808400136543fc1a0f522af1f3eaee034`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f0d8afe85320b7cf4542ad649671660bbb8e74ec3ad3067408e79fb21dbf77`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7def0e2b3dd94a350c82bb6a4903fdfc65d1d3d9772dd8195a5eb14ba766c45`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0b51c8090bf08cc2ae3a9fc340c9b70ba1e077f32b7d7d025b7d9fb472d978`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3653016f515e293fc93892b9e021e05a6a183ad3dcdaf243311513e222534c7`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d1dafd3fbb7403b7f093ed63553863bd9904f6010b1b91f98d9bfba9c4d8bb`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92817327253aaae4d632a75ff38a01dbebfe11f9105c4db828c52f221262ce4`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43bce457643a143e82e49e57d9b8a69a416e254d2439f30d7e4dd25c84e43c0`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 348.1 KB (348138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a0e899ab4c995de79522a5022b8cca4765559a4de2d5c728821d947b497de1`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:6fc3086452e6c85e993bf4b4834c55848a3977b547662cd4ce9fc98a17a495e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull caddy@sha256:935d1f4349cc551dfe9b76d6ba5fe6355414519a3037a7689fe765033ae8dcd6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1723388621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1deb1aecac8501d9afe22abd2fc90f15552c63366f8016ad2e6d1602be5cdf6d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:16:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:16:36 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:17:19 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:17:20 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:17:21 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:17:22 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:17:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:17:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:17:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:17:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:17:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:17:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:17:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:17:31 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:17:32 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:17:33 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:17:34 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:17:53 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:17:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47af8a9c9ef8e49d65e53dd207ad0935ce7a2b50b2f253e6a5b037494ae19d0a`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 401.5 KB (401472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5841cb6343add9dd7b89906610425117976b050c0634eedbc5c38302aa024e`  
		Last Modified: Thu, 09 Feb 2023 01:16:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d760049e5c9f1fb1d7ec05a3eea55088808f484912e87cda07f3709363fe3c2c`  
		Last Modified: Thu, 09 Feb 2023 01:16:53 GMT  
		Size: 14.7 MB (14680484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3239225b5bad52e6004b638bd356e7d29e7fded5d31d90541907e1a769a115`  
		Last Modified: Thu, 09 Feb 2023 01:16:49 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6823ad091829bc6d98a58a18b075e20c551bde81d504bdbfda09b5a3d7c5d0`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4873a8802163accb90dd2318bd05ddfa4f94692b2731d6e23095e3bb46b98fd`  
		Last Modified: Thu, 09 Feb 2023 01:16:48 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabf39e152fd5c18e0c3ac503e054c36e2775512f9fa7bb11b9221442b2bc1fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af12dc4018ba87a8e25003874e2d8e959a25b1c19932553daec8f4c410ebd61f`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fefa1f82e39e2af863b13609d78d966746d852af0cea54dcb17f45a8386c39d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:47 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d5b41708aea61714f00bc0f35ea1efc60db85c04ab6754e4d6b4485dc59a28`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a8b1cf8bcc4175323f7feaa280e3122f03aa7f9d35666fcc55c6b7d1e628ae`  
		Last Modified: Thu, 09 Feb 2023 01:16:46 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6c3f865e552649c436d5ffc0f3c83a3b5ba3026b2cff2ab3f381a5cdf2e2f2`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201cfdbfc1583e2ea070418e6aad0ec6604fb52c68117460b1a4c5b511b56ecc`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef83199fb67566ea043dbf7fab6f54754a4d0496655be1157819973573247bb`  
		Last Modified: Thu, 09 Feb 2023 01:16:45 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45db789a3d9786dea133341e2c9f16e14b23a664297ad7f9a371961a0c21588`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a4e021c112717a1fee7cd62cdc17d41521f3514f10bf8ec30457b95aaf44fa`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4c0327054bc1f199339822d4074ee176c4184b9357ec28d9250f27f0c12e26`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63a4d912695117a127068d20ceefbaa19e41c8a42d65788d37915d737d998d6`  
		Last Modified: Thu, 09 Feb 2023 01:16:44 GMT  
		Size: 338.6 KB (338620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421719fbbf536a3651d6762e36406f19dd0b5601f4a300d9c47af9ccfa3573d2`  
		Last Modified: Thu, 09 Feb 2023 01:16:43 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:65b3d9f69c1f9e10dae44434f033715465a5e5331b38550f4f47baa12a60a39c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1487; amd64

### `caddy:windowsservercore-ltsc2022` - windows version 10.0.20348.1487; amd64

```console
$ docker pull caddy@sha256:22cdfda624195707c05f1d681c1cdd97b504f06b282d981718e1b716b2dc6bfb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1401937005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca7c6af6ec202266d95f15726fee733430a631c6c4eddfd9cc7d000b817a0f19`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Feb 2023 00:18:43 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 09 Feb 2023 00:18:44 GMT
ENV CADDY_VERSION=v2.6.3
# Thu, 09 Feb 2023 00:19:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.3/caddy_2.6.3_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('5529a43f9d91b02bc4b8dc89e3c60b59395d1725079a46e8477a105ecb809da54e4ffed5698f4083dba397745c160511c07630d38c2d2695380c75ffb7e6afd1')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 09 Feb 2023 00:19:16 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 09 Feb 2023 00:19:17 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 09 Feb 2023 00:19:18 GMT
LABEL org.opencontainers.image.version=v2.6.3
# Thu, 09 Feb 2023 00:19:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 09 Feb 2023 00:19:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 09 Feb 2023 00:19:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 09 Feb 2023 00:19:22 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 09 Feb 2023 00:19:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 09 Feb 2023 00:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 09 Feb 2023 00:19:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 09 Feb 2023 00:19:26 GMT
EXPOSE 80
# Thu, 09 Feb 2023 00:19:27 GMT
EXPOSE 443
# Thu, 09 Feb 2023 00:19:29 GMT
EXPOSE 443/udp
# Thu, 09 Feb 2023 00:19:30 GMT
EXPOSE 2019
# Thu, 09 Feb 2023 00:19:47 GMT
RUN caddy version
# Thu, 09 Feb 2023 00:19:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42eb48143612ee855d99c932e324b1bd035c60554117edeaa805402060613c51`  
		Last Modified: Thu, 09 Feb 2023 01:17:17 GMT  
		Size: 635.9 KB (635943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b714ae92cb5dac0e72097d35b932125b5ea3f03214de78e03119a4517be6fd10`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a5533d3ddbff5ea35dbb0e11b10fe817ce3ef1a3fd7f44706cb1b6288e0406`  
		Last Modified: Thu, 09 Feb 2023 01:17:20 GMT  
		Size: 14.9 MB (14899830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e59c8f0dc8d987210bdfe89eaded536b0ef8ac727eb7d75b76aea9c296208a`  
		Last Modified: Thu, 09 Feb 2023 01:17:16 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22bfc3588219a43ce294aab21751b407ae75504bf3ddcee69f42498672b6c46`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f7db57dc0a0b0126433f60d3d0005f9aaa0d405fe63cfc3b4e15388fdfa010`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7b9e3a2510b5ab3b7ac4103d653c8efd12e95b63327d5c5fb81b6ea341e2b5`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4109b3b0ca73b5355a12ee74b7c32b4015a6208fdb279fd0ab60074247e22309`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3c568a1866d44483984b2be40142a55371adf3b8dc991bdb5ab4c45c0be3d4`  
		Last Modified: Thu, 09 Feb 2023 01:17:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6221c7c14444b318e798e231adeeb83ea155c157283e9def018c43415238aa7`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e81980463382095586f78276db5cd808400136543fc1a0f522af1f3eaee034`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f0d8afe85320b7cf4542ad649671660bbb8e74ec3ad3067408e79fb21dbf77`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7def0e2b3dd94a350c82bb6a4903fdfc65d1d3d9772dd8195a5eb14ba766c45`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0b51c8090bf08cc2ae3a9fc340c9b70ba1e077f32b7d7d025b7d9fb472d978`  
		Last Modified: Thu, 09 Feb 2023 01:17:12 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3653016f515e293fc93892b9e021e05a6a183ad3dcdaf243311513e222534c7`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d1dafd3fbb7403b7f093ed63553863bd9904f6010b1b91f98d9bfba9c4d8bb`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92817327253aaae4d632a75ff38a01dbebfe11f9105c4db828c52f221262ce4`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43bce457643a143e82e49e57d9b8a69a416e254d2439f30d7e4dd25c84e43c0`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 348.1 KB (348138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a0e899ab4c995de79522a5022b8cca4765559a4de2d5c728821d947b497de1`  
		Last Modified: Thu, 09 Feb 2023 01:17:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
