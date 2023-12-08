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
-	[`caddy:2.7.6`](#caddy276)
-	[`caddy:2.7.6-alpine`](#caddy276-alpine)
-	[`caddy:2.7.6-builder`](#caddy276-builder)
-	[`caddy:2.7.6-builder-alpine`](#caddy276-builder-alpine)
-	[`caddy:2.7.6-builder-windowsservercore-1809`](#caddy276-builder-windowsservercore-1809)
-	[`caddy:2.7.6-builder-windowsservercore-ltsc2022`](#caddy276-builder-windowsservercore-ltsc2022)
-	[`caddy:2.7.6-windowsservercore`](#caddy276-windowsservercore)
-	[`caddy:2.7.6-windowsservercore-1809`](#caddy276-windowsservercore-1809)
-	[`caddy:2.7.6-windowsservercore-ltsc2022`](#caddy276-windowsservercore-ltsc2022)
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
$ docker pull caddy@sha256:9eb928f0a3142d0a38e6d457f7696c08c13e070d49d6499cc5b0afe644ecb281
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.5122; amd64
	-	windows version 10.0.20348.2113; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:0eff0e7322c718fc65b783418531f1e75c7f27f1a3877823378737e91296ee8c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18474760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3791fd914060b4c02165b77f6f2c6e4516be2e77a6a8bd8ffab228253f75f47`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:32:06 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 06:32:07 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 06:32:07 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 06:32:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 06:32:10 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 06:32:10 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 06:32:10 GMT
EXPOSE 80
# Fri, 01 Dec 2023 06:32:11 GMT
EXPOSE 443
# Fri, 01 Dec 2023 06:32:11 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 06:32:11 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 06:32:11 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 06:32:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08886dfc0722c4ed2cb6a70c285a33fe35aec069435868488356dde320b4d21c`  
		Last Modified: Fri, 01 Dec 2023 06:32:30 GMT  
		Size: 350.8 KB (350845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0132c3b72c65b40cace6033d219e1e6d680bb85808270b77a5189c509c10bc0`  
		Last Modified: Fri, 01 Dec 2023 06:32:29 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2ecdf85e2f8f19fc737312e7157f0141b45020324fcf01f4e92bbe707d8983`  
		Last Modified: Fri, 01 Dec 2023 06:32:32 GMT  
		Size: 14.7 MB (14713987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e05dc14b4b6c6dbdcfbdbe28c73e86cafc5287fa13d4f51fdfdfad7b51b8936d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17423853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3acb342ef8cbce6055e45fdabe7e8b60e98cab9d0aa967e362098333633440ff`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:39:01 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 00:39:02 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 00:39:03 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 00:39:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 00:39:05 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 00:39:05 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 00:39:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 00:39:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 00:39:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 80
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 443
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 00:39:06 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 00:39:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc24e4ccf558b6e992efaaa7a735322be11fe99ce19e722eee6ae70bb76515d`  
		Last Modified: Fri, 01 Dec 2023 00:39:21 GMT  
		Size: 347.6 KB (347632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cd6f3873930f7c6aa4ee5d06ef24c77a840fec6f0211e9572fbe0f43c04e1f`  
		Last Modified: Fri, 01 Dec 2023 00:39:21 GMT  
		Size: 7.5 KB (7508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c51a919a8bb024456b258f25a71adb53a14e30c7134e81fac343c44dbf7230c`  
		Last Modified: Fri, 01 Dec 2023 00:39:23 GMT  
		Size: 13.9 MB (13921843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:c3be58f3d1b5614d2a5e7bff50bc07567044bb119ec0f286c94df8169efc313b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17156415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194c773f5747022fdb5fc8d32e8dafcafd61f37e52238ad53627e3309c2fb4cb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:19:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 03:19:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 03:19:15 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 03:19:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 03:19:19 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 03:19:19 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 03:19:20 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 03:19:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 03:19:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 03:19:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 03:19:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 03:19:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 03:19:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 03:19:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 03:19:22 GMT
EXPOSE 80
# Fri, 01 Dec 2023 03:19:22 GMT
EXPOSE 443
# Fri, 01 Dec 2023 03:19:23 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 03:19:23 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 03:19:23 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 03:19:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803b34e1f84b29ca968d2fbf85c278608566c34dfd1742e088c6483685957029`  
		Last Modified: Fri, 01 Dec 2023 03:19:48 GMT  
		Size: 344.5 KB (344464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bbcb291a405e073d645e52039b6f84fa5071645ceb53988f99d384fbc6c4c1`  
		Last Modified: Fri, 01 Dec 2023 03:19:48 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d0aed5710d79e6bba64ce3cf139d40c4e2c3003d1feec3776b18919e3a1423`  
		Last Modified: Fri, 01 Dec 2023 03:19:50 GMT  
		Size: 13.9 MB (13903440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e7f68eb0f76a55ada8be1bb5213e5bbbcb0727fa8d4051f6f3edf1275bc2dc40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17274998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9487e6591f483b0f0d5fe25a89d069485fa10bb97a06ef07085f28b86995977c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:11:08 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 03:11:09 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 03:11:10 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 03:11:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 03:11:11 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 03:11:11 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 80
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 443
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 03:11:12 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 03:11:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e383270d6915b6b427f49a75d657d5a0403fcd47a5f89cd30e85143ca54c22`  
		Last Modified: Fri, 01 Dec 2023 03:11:28 GMT  
		Size: 360.7 KB (360655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27e927f808292c7b306432ed3ee61ecc6b7f637b8ccbdf5cb2d6bdc24649858`  
		Last Modified: Fri, 01 Dec 2023 03:11:28 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dab02cb145c1d5336977666f796446f69abbbfa721ab7a71525867eb3edfbc`  
		Last Modified: Fri, 01 Dec 2023 03:11:30 GMT  
		Size: 13.6 MB (13573804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:3f9f202dc07f3bb097e0e78330d59f52c488ff4ba3b4aa4a569f1a28c9db95f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.1 MB (17058981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:126d26f69982d49f88bac36f166a92d251494018b25e2e255972b98f38f495f8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:42:19 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 05:42:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 05:42:52 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 05:42:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 05:43:00 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 05:43:20 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 05:43:24 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 05:43:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 05:43:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 05:43:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 05:43:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 05:43:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 05:43:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 05:43:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 05:43:45 GMT
EXPOSE 80
# Fri, 01 Dec 2023 05:43:46 GMT
EXPOSE 443
# Fri, 01 Dec 2023 05:43:46 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 05:43:47 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 05:43:48 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 05:43:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce4bc2907f69809c3086f118895d7e5c8683349557239c0ce79dfbda0ce3768`  
		Last Modified: Fri, 01 Dec 2023 05:44:17 GMT  
		Size: 362.2 KB (362185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef8889b660799cb5b3c54f8771b4a37ad12c12f245aa74e4af501a899449137`  
		Last Modified: Fri, 01 Dec 2023 05:44:17 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681f2bb9965ff577316200c634bfb7e7db0d5b2ba971441db97e1405e3c0fc6b`  
		Last Modified: Fri, 01 Dec 2023 05:44:19 GMT  
		Size: 13.3 MB (13340969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:159a339dbc4d0e8279faad422e0a871d82adcc6736b9c4ac4c4b252c3dbee6a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.8 MB (17825031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0c61727c246c9eedd4c40bc927993a89531560cc027902c6f00b8f288f96b77`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:22:31 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 08:22:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 08:22:32 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 08:22:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 08:22:37 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 08:22:37 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 08:22:38 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 08:22:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 80
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 443
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 08:22:38 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 08:22:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20bbe0abb0a3f63718aa78742832077ad86b8ae86d70ce3ebcece342ec022c6`  
		Last Modified: Fri, 01 Dec 2023 08:23:07 GMT  
		Size: 354.9 KB (354948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1497491e477a92a5e82d0d68588396a3414c6e703fdc68c82c768ad6b18b28`  
		Last Modified: Fri, 01 Dec 2023 08:23:07 GMT  
		Size: 7.5 KB (7502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539ac3a1bb2d355499d388b4de966f9148263d5603f2db92aeba42084d02b3cf`  
		Last Modified: Fri, 01 Dec 2023 08:23:09 GMT  
		Size: 14.2 MB (14245127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:38df49f40c98b8d866440b7fec4635fcf669f4c138fd001b95f457b42e4e2265
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2073433228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7105669fddc0d611982501b46d56df54a820ca14cd7e3a3c62c02ef1bd40fc2e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:30:07 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Nov 2023 05:30:07 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:31:22 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Nov 2023 05:31:23 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Nov 2023 05:31:24 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Nov 2023 05:31:25 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 16 Nov 2023 05:31:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Nov 2023 05:31:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Nov 2023 05:31:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Nov 2023 05:31:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Nov 2023 05:31:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Nov 2023 05:31:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Nov 2023 05:31:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Nov 2023 05:31:32 GMT
EXPOSE 80
# Thu, 16 Nov 2023 05:31:33 GMT
EXPOSE 443
# Thu, 16 Nov 2023 05:31:34 GMT
EXPOSE 443/udp
# Thu, 16 Nov 2023 05:31:35 GMT
EXPOSE 2019
# Thu, 16 Nov 2023 05:32:33 GMT
RUN caddy version
# Thu, 16 Nov 2023 05:32:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d66ae500a331057bbb6b25a0c0e5718f2491209d7330f70b1203472b199bd5b`  
		Last Modified: Thu, 16 Nov 2023 05:37:31 GMT  
		Size: 451.2 KB (451175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec48b5261067a4b4643799633487cce5b6ee11cce36314b8a6b22964fd46ba4`  
		Last Modified: Thu, 16 Nov 2023 05:37:30 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bc40730815ee35e950756a15aa93561edd0f272d34d30de69bb8d7f58b1d8e`  
		Last Modified: Thu, 16 Nov 2023 05:37:34 GMT  
		Size: 15.3 MB (15273771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfce8b69f4cadeeaa9fcc771a3a5b374fc4a3c8c41c1a42a7878c1cad861645c`  
		Last Modified: Thu, 16 Nov 2023 05:37:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdd09852c86166de537f8b5f5b78eca092cfb95e9e2e1194c84a7a05334e5c4`  
		Last Modified: Thu, 16 Nov 2023 05:37:29 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f15c2b10239537d18dc39c5208acb0c8fc7bc25d6cd95cb59ed8e8aaf8b73be`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa35da536891cce8df35bca524d15b1b7465d4fc14354a1a15a2fa39d71a4a88`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654652f0bb6c82a0e1fd51010fd587112527866df3c9748cf9ed4414e70ee612`  
		Last Modified: Thu, 16 Nov 2023 05:37:29 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0fcd5cbdfe3f968d65ba5dcece2d017de82a3a4ec737745bd5560697735689`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9396734c66d2d27545fdeb2c33a462651a3807dfcbd04b590a01ace722161a21`  
		Last Modified: Thu, 16 Nov 2023 05:37:27 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a14586579bd1d9d9a9162b0678a119c826a7be5039b5419e90b82c772b33677`  
		Last Modified: Thu, 16 Nov 2023 05:37:27 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c773c8968545d0fca628d03a3b588ca4798423090cadd666d023cee5065235a5`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce86207f89519b9df4526afc22e743fef4a6266614fb8e082e975bf0f01862f`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7392ec7da7419f69c0413116467249934c403f42b53ff6090608481e1ba7985a`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73d1eee374e37176384bade9abdbe65d5aed23b976c507b3b88b17c758761f`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d556f28b534238f3c8497a928caa36428f1d333a69cabf15b4fc3d80aa7f3f9f`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd0eba7ede6da63115506e40bf2b6990915e5fba916e919c6525f447018bbd9`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf5b269f798b76bfba9ad2e27b5aab7bebe448007c818230643c16d6cf761af`  
		Last Modified: Thu, 16 Nov 2023 05:37:25 GMT  
		Size: 252.7 KB (252713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c70c9a3deaf4a41d4192a9248f3fd5ccfadb54792687f31f63a17f46e5134c`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:7a86ad9fb59b43cc97f50c3516b4153bb228276c026e4c802c4a213b0fe1c20f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1902803411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03625f7f4ec599de5399e0e9d5f36d3c2052adeb06f8349ef7a96e3777ddf4e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 09 Nov 2023 06:47:20 GMT
RUN Install update 10.0.20348.2113
# Thu, 16 Nov 2023 01:36:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:33:15 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Nov 2023 05:33:16 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:33:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Nov 2023 05:33:45 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Nov 2023 05:33:46 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Nov 2023 05:33:47 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 16 Nov 2023 05:33:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Nov 2023 05:33:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Nov 2023 05:33:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Nov 2023 05:33:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Nov 2023 05:33:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Nov 2023 05:33:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Nov 2023 05:33:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Nov 2023 05:33:54 GMT
EXPOSE 80
# Thu, 16 Nov 2023 05:33:55 GMT
EXPOSE 443
# Thu, 16 Nov 2023 05:33:56 GMT
EXPOSE 443/udp
# Thu, 16 Nov 2023 05:33:57 GMT
EXPOSE 2019
# Thu, 16 Nov 2023 05:34:33 GMT
RUN caddy version
# Thu, 16 Nov 2023 05:34:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7989ef2c4cfb06d845746a3c3660481ea84d3f5c8216041855ce528f0ac4015c`  
		Last Modified: Tue, 14 Nov 2023 20:43:13 GMT  
		Size: 498.2 MB (498182566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbeb193d02c2ca7f9a9ea438fbf1bcdb6ea4a6fea626713330fd1ebb514424f`  
		Last Modified: Thu, 16 Nov 2023 02:25:14 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b269b5ac8d8c6baa501ca9b38fa715170022416aa7332a2d155a06529882b84a`  
		Last Modified: Thu, 16 Nov 2023 05:37:59 GMT  
		Size: 458.2 KB (458201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f982a236809063ef75b5db6a226207448d936d7791ede196115611649805c5`  
		Last Modified: Thu, 16 Nov 2023 05:37:58 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2783cb5dad5df996a48a9ebf989a6136c91f524f421bfff9e71ab764da46fd04`  
		Last Modified: Thu, 16 Nov 2023 05:38:01 GMT  
		Size: 15.3 MB (15269735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa26255a8f194a0aa31a8fd0c48e7dfba117358880abeaf7ad3c5f54a6be87d`  
		Last Modified: Thu, 16 Nov 2023 05:37:57 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706b8120af6e900b1d0dea48743c4fd50b63c785dbe02b5ccd4af53e68ebefff`  
		Last Modified: Thu, 16 Nov 2023 05:37:57 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c12376eb1027b4892f92b1b8dd45b1e05d78f365c2886ded9202ffbaab80e9`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a29b9f98e523c3477366f98e560b8638fb5c3f0a7a8c76c9a417a33b4d44804`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a9a2fb5b49cb3e38b64f06a755f57ec37b8b5eaf2152fe9e38ae9c8cb3b593`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53a0ea77b4fcc256276d31401de856267c72aeac7fefeeb6fbe655340bb4cf4`  
		Last Modified: Thu, 16 Nov 2023 05:37:55 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d80b783b85d05309ef9fe97740b873bd9092c13b53eea3d83adf6197cbe798`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9454c6602eef29f64927e75d96b8f26d7cf0c6c089afa91e260207675216501`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f23d9fc021e786b83141dd57c2a10dc279d17eacad254ec81d7922372d17876`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55a4267cea49483a79cbee8908d3daf6af4fb6fa1af94e350072034f128c5a1`  
		Last Modified: Thu, 16 Nov 2023 05:37:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9723590c56e28022e6ee055495ee5826c7ea085d2a8b7255d471b35bb27e9a6c`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b39c632f1f53a232721260e3ebcc755559883edb0272949f2d965799d62ef5`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3deb93ce29c0157e6c6b82bbad0ffb2102a833ea54672c93c05843899eac3bc`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09fe12ffad65804e54e566d7b3256d98268c5e943a40282d44bab50d3fb6a04`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517e7fd42cd9750ca7ef5a68df02e2bdc3be404dbd69681f36c7b0acb1562550`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 270.1 KB (270069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0727df29cc57ce0bb7db3c73852d6eaceb439603493f2e3ceb07ce2f8e8e4e99`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:9821d1ef822957bf0ac22f9c6e26ad6a3198604f29b3b79194acba7ccaff4532
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
$ docker pull caddy@sha256:0eff0e7322c718fc65b783418531f1e75c7f27f1a3877823378737e91296ee8c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18474760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3791fd914060b4c02165b77f6f2c6e4516be2e77a6a8bd8ffab228253f75f47`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:32:06 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 06:32:07 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 06:32:07 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 06:32:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 06:32:10 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 06:32:10 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 06:32:10 GMT
EXPOSE 80
# Fri, 01 Dec 2023 06:32:11 GMT
EXPOSE 443
# Fri, 01 Dec 2023 06:32:11 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 06:32:11 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 06:32:11 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 06:32:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08886dfc0722c4ed2cb6a70c285a33fe35aec069435868488356dde320b4d21c`  
		Last Modified: Fri, 01 Dec 2023 06:32:30 GMT  
		Size: 350.8 KB (350845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0132c3b72c65b40cace6033d219e1e6d680bb85808270b77a5189c509c10bc0`  
		Last Modified: Fri, 01 Dec 2023 06:32:29 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2ecdf85e2f8f19fc737312e7157f0141b45020324fcf01f4e92bbe707d8983`  
		Last Modified: Fri, 01 Dec 2023 06:32:32 GMT  
		Size: 14.7 MB (14713987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e05dc14b4b6c6dbdcfbdbe28c73e86cafc5287fa13d4f51fdfdfad7b51b8936d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17423853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3acb342ef8cbce6055e45fdabe7e8b60e98cab9d0aa967e362098333633440ff`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:39:01 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 00:39:02 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 00:39:03 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 00:39:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 00:39:05 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 00:39:05 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 00:39:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 00:39:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 00:39:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 80
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 443
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 00:39:06 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 00:39:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc24e4ccf558b6e992efaaa7a735322be11fe99ce19e722eee6ae70bb76515d`  
		Last Modified: Fri, 01 Dec 2023 00:39:21 GMT  
		Size: 347.6 KB (347632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cd6f3873930f7c6aa4ee5d06ef24c77a840fec6f0211e9572fbe0f43c04e1f`  
		Last Modified: Fri, 01 Dec 2023 00:39:21 GMT  
		Size: 7.5 KB (7508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c51a919a8bb024456b258f25a71adb53a14e30c7134e81fac343c44dbf7230c`  
		Last Modified: Fri, 01 Dec 2023 00:39:23 GMT  
		Size: 13.9 MB (13921843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:c3be58f3d1b5614d2a5e7bff50bc07567044bb119ec0f286c94df8169efc313b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17156415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194c773f5747022fdb5fc8d32e8dafcafd61f37e52238ad53627e3309c2fb4cb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:19:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 03:19:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 03:19:15 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 03:19:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 03:19:19 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 03:19:19 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 03:19:20 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 03:19:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 03:19:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 03:19:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 03:19:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 03:19:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 03:19:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 03:19:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 03:19:22 GMT
EXPOSE 80
# Fri, 01 Dec 2023 03:19:22 GMT
EXPOSE 443
# Fri, 01 Dec 2023 03:19:23 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 03:19:23 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 03:19:23 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 03:19:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803b34e1f84b29ca968d2fbf85c278608566c34dfd1742e088c6483685957029`  
		Last Modified: Fri, 01 Dec 2023 03:19:48 GMT  
		Size: 344.5 KB (344464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bbcb291a405e073d645e52039b6f84fa5071645ceb53988f99d384fbc6c4c1`  
		Last Modified: Fri, 01 Dec 2023 03:19:48 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d0aed5710d79e6bba64ce3cf139d40c4e2c3003d1feec3776b18919e3a1423`  
		Last Modified: Fri, 01 Dec 2023 03:19:50 GMT  
		Size: 13.9 MB (13903440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e7f68eb0f76a55ada8be1bb5213e5bbbcb0727fa8d4051f6f3edf1275bc2dc40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17274998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9487e6591f483b0f0d5fe25a89d069485fa10bb97a06ef07085f28b86995977c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:11:08 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 03:11:09 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 03:11:10 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 03:11:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 03:11:11 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 03:11:11 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 80
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 443
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 03:11:12 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 03:11:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e383270d6915b6b427f49a75d657d5a0403fcd47a5f89cd30e85143ca54c22`  
		Last Modified: Fri, 01 Dec 2023 03:11:28 GMT  
		Size: 360.7 KB (360655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27e927f808292c7b306432ed3ee61ecc6b7f637b8ccbdf5cb2d6bdc24649858`  
		Last Modified: Fri, 01 Dec 2023 03:11:28 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dab02cb145c1d5336977666f796446f69abbbfa721ab7a71525867eb3edfbc`  
		Last Modified: Fri, 01 Dec 2023 03:11:30 GMT  
		Size: 13.6 MB (13573804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:3f9f202dc07f3bb097e0e78330d59f52c488ff4ba3b4aa4a569f1a28c9db95f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.1 MB (17058981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:126d26f69982d49f88bac36f166a92d251494018b25e2e255972b98f38f495f8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:42:19 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 05:42:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 05:42:52 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 05:42:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 05:43:00 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 05:43:20 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 05:43:24 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 05:43:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 05:43:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 05:43:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 05:43:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 05:43:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 05:43:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 05:43:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 05:43:45 GMT
EXPOSE 80
# Fri, 01 Dec 2023 05:43:46 GMT
EXPOSE 443
# Fri, 01 Dec 2023 05:43:46 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 05:43:47 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 05:43:48 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 05:43:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce4bc2907f69809c3086f118895d7e5c8683349557239c0ce79dfbda0ce3768`  
		Last Modified: Fri, 01 Dec 2023 05:44:17 GMT  
		Size: 362.2 KB (362185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef8889b660799cb5b3c54f8771b4a37ad12c12f245aa74e4af501a899449137`  
		Last Modified: Fri, 01 Dec 2023 05:44:17 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681f2bb9965ff577316200c634bfb7e7db0d5b2ba971441db97e1405e3c0fc6b`  
		Last Modified: Fri, 01 Dec 2023 05:44:19 GMT  
		Size: 13.3 MB (13340969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:159a339dbc4d0e8279faad422e0a871d82adcc6736b9c4ac4c4b252c3dbee6a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.8 MB (17825031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0c61727c246c9eedd4c40bc927993a89531560cc027902c6f00b8f288f96b77`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:22:31 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 08:22:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 08:22:32 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 08:22:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 08:22:37 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 08:22:37 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 08:22:38 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 08:22:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 80
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 443
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 08:22:38 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 08:22:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20bbe0abb0a3f63718aa78742832077ad86b8ae86d70ce3ebcece342ec022c6`  
		Last Modified: Fri, 01 Dec 2023 08:23:07 GMT  
		Size: 354.9 KB (354948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1497491e477a92a5e82d0d68588396a3414c6e703fdc68c82c768ad6b18b28`  
		Last Modified: Fri, 01 Dec 2023 08:23:07 GMT  
		Size: 7.5 KB (7502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539ac3a1bb2d355499d388b4de966f9148263d5603f2db92aeba42084d02b3cf`  
		Last Modified: Fri, 01 Dec 2023 08:23:09 GMT  
		Size: 14.2 MB (14245127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:dfd9af513214974c6a77e5e89c7cd3c6d2ddddb226bd21f95118958d47c0c537
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.5122; amd64
	-	windows version 10.0.20348.2113; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:fd75db17630bfaadeef0d2ee65994b5714e8b50b680116e62063b53f58ee8494
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76963250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c15f2632afa610125145b4eeb7cd15cfd6eb2789f9806d851ebe5254b2e0b4aa`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:46:23 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 03:46:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:25:52 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:26:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:26:02 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:26:02 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:26:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:26:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:26:03 GMT
WORKDIR /go
# Tue, 05 Dec 2023 20:48:59 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 20:48:59 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 20:48:59 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 20:48:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 20:48:59 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 20:49:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 20:49:01 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 20:49:01 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501dced60f86be38cc73d3c038f7db4afeee65726f7e422aacf09244539ebf1`  
		Last Modified: Fri, 01 Dec 2023 03:50:39 GMT  
		Size: 284.7 KB (284697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63d189496f5f03c835c9c85df2db6920546d36a1701f6b5ad15f800c671605d`  
		Last Modified: Tue, 05 Dec 2023 20:31:27 GMT  
		Size: 67.0 MB (67003308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aeb88dd0f3e06a57abc08c781b85c89d138194918c469aea9a1bed9753d2ed0`  
		Last Modified: Tue, 05 Dec 2023 20:31:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40ff2505fd8d96e76bddb63b05c2d42815db1dabe0093ec8f8f53be403b0d01`  
		Last Modified: Tue, 05 Dec 2023 20:49:17 GMT  
		Size: 5.0 MB (4970029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3868d63c7cd554f20832e0aff9559fa0cdd7cdbaa4de14e8043fefd0ebfde5`  
		Last Modified: Tue, 05 Dec 2023 20:49:16 GMT  
		Size: 1.3 MB (1302235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a2748825cf9745fffb7f4807c0b6fd474a0221d0d19177142c3f952e10ac78`  
		Last Modified: Tue, 05 Dec 2023 20:49:16 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2c90abb7280a71391618e8552a4faa4e66eb61f80d02402126d25f1365cf063f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75409540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a539589e36806b442a969b2dcf589a62915dde0f6bee440eb73fda5d315a9dd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:53:48 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 00:53:48 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:49:18 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:49:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:49:36 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:49:36 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:49:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:49:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:49:37 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:11:53 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:11:53 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:11:53 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:11:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:11:53 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:11:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:11:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:11:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e7ba0492eb25e7f21078441d7cdc65088836bc1984bc4a14cd3e9cd75cbf32`  
		Last Modified: Fri, 01 Dec 2023 01:00:23 GMT  
		Size: 284.9 KB (284884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de60bcfc919bc6b53554a040a5a58936a8d2e2bf66b2872b69d7a3164e35923f`  
		Last Modified: Tue, 05 Dec 2023 20:54:54 GMT  
		Size: 65.8 MB (65764248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e61f3b09467cb2b97e65a90f25e38cba8acfcd387d168214a949b59bf8c09a`  
		Last Modified: Tue, 05 Dec 2023 20:54:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7827ddd1dfa7654d070274e573dbfcc8fb5ac2ef73888f8b0563e0672811ad`  
		Last Modified: Tue, 05 Dec 2023 21:12:11 GMT  
		Size: 5.0 MB (4964331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f919a9a90cd0240dfd228f8b093cb51b08bf03eabc0326cfe303219b37469f5`  
		Last Modified: Tue, 05 Dec 2023 21:12:11 GMT  
		Size: 1.2 MB (1248647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66464a5ea9ace101c6914e8c5da3a953cb5a9b372ffc562f6a7ab2bcc2b9c0a6`  
		Last Modified: Tue, 05 Dec 2023 21:12:11 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:f65daee5179d36a392c0d931a02c5c400f99b4470bd68e3f326d6828bd8f3fb6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74707169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53077f2480efa131c1c20460899eb69b049d624d249a844e4e1c3bd88aa28d12`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:44:57 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 08:44:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:58:01 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:58:16 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:58:16 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:58:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:58:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:58:17 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:22:31 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:22:31 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:22:31 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:22:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:22:31 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:22:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:22:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:22:32 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a824ff289f1a3c765a444079137b8b7f1cee80348faa53e1ba4c960b73ed2a`  
		Last Modified: Fri, 01 Dec 2023 08:49:42 GMT  
		Size: 284.1 KB (284079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4989177b4ed66b7e9f9e8c4bfce82720b582e24b735d6628effa75d81c5718fc`  
		Last Modified: Tue, 05 Dec 2023 21:04:43 GMT  
		Size: 65.8 MB (65764197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f9b58eae167c54d3faa3eeffd480cdae7e8b4841eb816a86cfdd01f8ae29ef`  
		Last Modified: Tue, 05 Dec 2023 21:04:29 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4cd1a3aab8fc02791b1e19f81b7de1bd691c10a7c942acc7e733221bf12888`  
		Last Modified: Tue, 05 Dec 2023 21:22:47 GMT  
		Size: 4.5 MB (4511237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3a92f0249b45814852e4e987e1a6304bcfb211077150ab43415b31d929f4af`  
		Last Modified: Tue, 05 Dec 2023 21:22:47 GMT  
		Size: 1.2 MB (1246087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3152bffd7f15885d0e72b0adabc22f46542f569db908b69d63eb29addd5e950`  
		Last Modified: Tue, 05 Dec 2023 21:22:47 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:977753f53683eb84ddc7477e5a743e0e1e4e2a001f20edfa0f01d43359d85dc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73981644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0f601640aa519cb421e86cd75a6ad6223541d58cfe80b27b699a23a2585ce70`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:43:53 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 03:18:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:16:18 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:16:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:16:28 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:16:28 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:16:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:16:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:16:28 GMT
WORKDIR /go
# Tue, 05 Dec 2023 20:38:16 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 20:38:16 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 20:38:16 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 20:38:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 20:38:16 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 20:38:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 20:38:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 20:38:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a63ed24dc22a348b35d99b5ec9dc67ff66563b539875e5c8ab2d870b3991ac`  
		Last Modified: Fri, 01 Dec 2023 02:44:03 GMT  
		Size: 286.3 KB (286307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f00641dffc5c2a149049ee9046bb24cfc7de534b7495a0f27784a4fff0fadc`  
		Last Modified: Tue, 05 Dec 2023 20:21:00 GMT  
		Size: 64.1 MB (64094844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452682ba77e89fc55be3a168358f5f43bccad93ecdd3d53b4dec7fff6915128b`  
		Last Modified: Tue, 05 Dec 2023 20:20:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3fe1e12507f8c4a2731393eebfc5ab973aa344b0daceec525560b812b26f60`  
		Last Modified: Tue, 05 Dec 2023 20:38:33 GMT  
		Size: 5.1 MB (5068450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb3c2fad921714e69ace0b18d8f72eb2566d50bc92ff9e9dd125ec383131eb9`  
		Last Modified: Tue, 05 Dec 2023 20:38:32 GMT  
		Size: 1.2 MB (1198449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9c40c8a39fcf5ab6fa64b1c2e1dd5d0b5c1f6b4d9c11ed9481644fe94f1cbf`  
		Last Modified: Tue, 05 Dec 2023 20:38:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:50de875c68ad6aeffc5eb2dd0942d219481fe70c55088657bbe724abd05f7c49
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74206489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7029045647c7331bb58455d58f274c3e4356d86729c097b8d3cfe35717b3b9d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:37:34 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 06:37:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:38:14 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:38:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:38:37 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:38:38 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:38:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:38:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:38:41 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:04:33 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:04:34 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:04:35 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:04:35 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:04:35 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:04:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:04:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:04:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692dbecd5e141c462ab06ef113ec964b525e7564d734890cc1d5b1dbf33ee34e`  
		Last Modified: Fri, 01 Dec 2023 06:43:30 GMT  
		Size: 286.7 KB (286661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc89a0f2d97ecfd4d20235e72227fc24aa79a64509fe9ea64702db658f2ad26d`  
		Last Modified: Tue, 05 Dec 2023 20:46:23 GMT  
		Size: 64.1 MB (64115804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d76f2c2e2bbb4190b1865ddafdc8cb88adee4c79d7d5ba23e69696e9610889`  
		Last Modified: Tue, 05 Dec 2023 20:46:11 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e0ec0f713ee657d6aa159fab65c05939480b5ca50a8e3dc4b1a9a6578160f7`  
		Last Modified: Tue, 05 Dec 2023 21:04:57 GMT  
		Size: 5.3 MB (5268970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e164016cca4964643911960baccae8beaa47cc5086bbe3ebfd14183d5204a8`  
		Last Modified: Tue, 05 Dec 2023 21:04:56 GMT  
		Size: 1.2 MB (1186171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2932f0ef681ac7135c1e7ff9332dd4c154c1f793d04fda438db30a1573bacc8b`  
		Last Modified: Tue, 05 Dec 2023 21:04:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:98d5d7af77acd9cc1b74499ba61056fb599a17742331f51a0fffa89ef56bb114
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76098838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d4f342a39bbb58bda0421e578348bf6d047bf7125db5c42216b2ba9b6d5040d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:14:49 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 08:14:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:44:16 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:44:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:45:03 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:45:04 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:45:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:45:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:45:05 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:14:29 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:14:29 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:14:29 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:14:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:14:30 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:14:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:14:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:14:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab563e8d41683e124df048aa9b564b0e8e1021e85213666971a015df51d5e48`  
		Last Modified: Fri, 01 Dec 2023 08:20:46 GMT  
		Size: 285.1 KB (285090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d44aea4caa072a45cb44ab86f401c76153b599207fb3cc311f44308e9b5da13`  
		Last Modified: Tue, 05 Dec 2023 20:57:00 GMT  
		Size: 66.2 MB (66218626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef66858f73257b9fd43395b7e2758cdaa72267303442d3a5dbef122796530c5`  
		Last Modified: Tue, 05 Dec 2023 20:56:49 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5261478888d8f0caaf878da0629c62f928bbbff35e7f873c1a463c6e39c0bd37`  
		Last Modified: Tue, 05 Dec 2023 21:14:53 GMT  
		Size: 5.1 MB (5114717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade58cb7b8ea422e0ab68cb58091d9adc84172a8de51990bb80269c07c5bd556`  
		Last Modified: Tue, 05 Dec 2023 21:14:53 GMT  
		Size: 1.3 MB (1262391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7f47ab035030fe8af075c6b5ebf045cd6bd32bef0700d8cc656ba7204685b7`  
		Last Modified: Tue, 05 Dec 2023 21:14:52 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:a4a6967f69e81e55f736b4e5d91bab0e44ce577821e0336b8b8ef7456679e1c1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2154296990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14a551f4e77e9632ddd054915a37f355befe0b5201417194368482bc6a54949d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 02:47:03 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Nov 2023 02:47:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Nov 2023 02:47:05 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Nov 2023 02:47:06 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Nov 2023 02:48:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:48:31 GMT
ENV GOPATH=C:\go
# Thu, 16 Nov 2023 02:49:41 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 05 Dec 2023 20:18:04 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:21:11 GMT
RUN $url = 'https://dl.google.com/go/go1.21.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'bbe603cde7c9dee658f45164b4d06de1eff6e6e6b800100824e7c00d56a9a92f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 05 Dec 2023 20:21:13 GMT
WORKDIR C:\go
# Tue, 05 Dec 2023 20:59:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 05 Dec 2023 20:59:30 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 20:59:31 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 20:59:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:00:49 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 05 Dec 2023 21:00:50 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e901367fac1450f509d3118ada9e004e3613844ebdf91861147a093483930a4`  
		Last Modified: Thu, 16 Nov 2023 03:11:57 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e08004205bd077d8f22b013c70dc2f10796c64fced1eb9927e0055daff2d05d`  
		Last Modified: Thu, 16 Nov 2023 03:11:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebc5048afc68ef48e2f2136545e2cccf26bb29eb4926bf4259b370ad55b4e7a`  
		Last Modified: Thu, 16 Nov 2023 03:11:55 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f50fe5c7ef21648f3eaa4304932877a116fcb910b8e9095c779a2fbe6d57f7e`  
		Last Modified: Thu, 16 Nov 2023 03:11:55 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76fe0e37750041d4ede2a0ca3b5245cfe075c3eb2ee27d7ce72ee8c3d7b20cc`  
		Last Modified: Thu, 16 Nov 2023 03:12:00 GMT  
		Size: 25.5 MB (25537512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8097bb9b8778d15dbf89d899653bf1634ec17554e5d84ef1ccfcac8ebf86afe2`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b542d31e914d67da86cc5701cdc282ab664dc1170507e3802e22ab3026436a90`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 263.2 KB (263200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86acdf7d3955fb44136bac433a30ccbbb97863120f270af32659dd65446666c7`  
		Last Modified: Tue, 05 Dec 2023 20:39:22 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1abe126c354944b7db8aa724d8f757167f7c3b36d39f976ef3b1b0d1b1b65ab`  
		Last Modified: Tue, 05 Dec 2023 20:39:41 GMT  
		Size: 69.4 MB (69361283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6338af096e09067ad482a0f4a6df1d1eee5b5595a64ca5f367b94ce27903e284`  
		Last Modified: Tue, 05 Dec 2023 20:39:22 GMT  
		Size: 1.5 KB (1529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0adc218b27ef5639384c060fb663de3bd74374279d3fd525aa281f63a754779`  
		Last Modified: Tue, 05 Dec 2023 21:02:06 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c21053b248805df7ad888734f5cd1df5a6b426111512d5a6b7530060e7f30b2`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57f384772c293e1d97326febf9e29d6bfef6eb9da2b053b6ad1e0ebea539508`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a2cba3fcdba1e3612614837be0fed9e3b7670483867a14203a15d395aa4179`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b447549db21db40db8a08cddb7d529bbd6e183aba676f13e2a3a5ff034fb67f8`  
		Last Modified: Tue, 05 Dec 2023 21:02:04 GMT  
		Size: 1.7 MB (1685436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408a12340d35fbfeee8cc5bdec3421ede796686f2b22d693863de08da6d51c91`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:081774d66d26fdb1b8b89fc90aeb9a72c559c0690770f153fa4ca3f1d5450e43
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1983623458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af2bcbcbf997ed6d0e17a2acebd1f65d19dbb6868d0523c306342bcc37644dd6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 09 Nov 2023 06:47:20 GMT
RUN Install update 10.0.20348.2113
# Thu, 16 Nov 2023 01:36:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 02:43:34 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Nov 2023 02:43:35 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Nov 2023 02:43:36 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Nov 2023 02:43:37 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Nov 2023 02:44:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:44:11 GMT
ENV GOPATH=C:\go
# Thu, 16 Nov 2023 02:44:30 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 05 Dec 2023 20:15:35 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:17:49 GMT
RUN $url = 'https://dl.google.com/go/go1.21.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'bbe603cde7c9dee658f45164b4d06de1eff6e6e6b800100824e7c00d56a9a92f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 05 Dec 2023 20:17:50 GMT
WORKDIR C:\go
# Tue, 05 Dec 2023 21:00:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 05 Dec 2023 21:00:58 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:00:59 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:01:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:01:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 05 Dec 2023 21:01:26 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7989ef2c4cfb06d845746a3c3660481ea84d3f5c8216041855ce528f0ac4015c`  
		Last Modified: Tue, 14 Nov 2023 20:43:13 GMT  
		Size: 498.2 MB (498182566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbeb193d02c2ca7f9a9ea438fbf1bcdb6ea4a6fea626713330fd1ebb514424f`  
		Last Modified: Thu, 16 Nov 2023 02:25:14 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b1d4a557f047b695f94452d9707061981d7fae4239c674b332282b8291963c`  
		Last Modified: Thu, 16 Nov 2023 03:11:20 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45549c207f14d769cba7c36b66157ec213bbc32ce57d685d8e2c407cf3987bb`  
		Last Modified: Thu, 16 Nov 2023 03:11:18 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c674717e06bf8cb25d5887393ef9568ee0ab6390966b9666808e836e9bd471d`  
		Last Modified: Thu, 16 Nov 2023 03:11:18 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2227badcd9f5f2b70b3d2ffd1c18887498f413c07802bfb334e8dc7b2d2acc`  
		Last Modified: Thu, 16 Nov 2023 03:11:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9f3b5e90a2e6028cf194e870b24a7158f875f18b81f4f9137a5db3ea1f79ac`  
		Last Modified: Thu, 16 Nov 2023 03:11:23 GMT  
		Size: 25.5 MB (25536225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7811a5416dcd19193a5b3ab9327607bf845f7ff77f95d3e20abdfb7435c32ae0`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5931209e960a94616639ea72e4d3ad9dc9cb554790ce930152c73bdc1449c034`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 266.6 KB (266600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a70f603a2fb4e76edd3165b62a179fb8f6410e265f5ae4a3732ee68e610034b`  
		Last Modified: Tue, 05 Dec 2023 20:38:48 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e37840dec3a6665ce48520be8b2c51b654359765bee5ab0780ee74746f0eb2`  
		Last Modified: Tue, 05 Dec 2023 20:39:08 GMT  
		Size: 69.3 MB (69342960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d16ae54757acda093616d24735d4c92d4676649bec49807fc35de90d15e15c`  
		Last Modified: Tue, 05 Dec 2023 20:38:48 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5744d01eddd2ef9d9673fdb0f0e48203fad1b01f2b14899a3ec6393c4548e75`  
		Last Modified: Tue, 05 Dec 2023 21:02:23 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35bb848667aa413b6ce6c309a4c2169635b0740dc335b9b39413a00627c01ab`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78369d5e83dd4f4ca5558a32848f3515e191b15f8427ea166a4f6327694ff9db`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2ae381a5e49194e43b26ac8036b1da5d2af930f7516796c476bcdb9c8125e3`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09db71960c4c717ed44d2694cf77f248223822e163297046010868c3ebf0767`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.7 MB (1677926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9dfae036c2fe0cfcd2e4f5a9acc265c45af769542844b9b617b62ec3ebd591`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:3e0232193d2e16a551210bb7cf4da86b6d0bf45cb70508c343c680065d7c440e
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
$ docker pull caddy@sha256:fd75db17630bfaadeef0d2ee65994b5714e8b50b680116e62063b53f58ee8494
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76963250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c15f2632afa610125145b4eeb7cd15cfd6eb2789f9806d851ebe5254b2e0b4aa`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:46:23 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 03:46:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:25:52 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:26:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:26:02 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:26:02 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:26:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:26:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:26:03 GMT
WORKDIR /go
# Tue, 05 Dec 2023 20:48:59 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 20:48:59 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 20:48:59 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 20:48:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 20:48:59 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 20:49:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 20:49:01 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 20:49:01 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501dced60f86be38cc73d3c038f7db4afeee65726f7e422aacf09244539ebf1`  
		Last Modified: Fri, 01 Dec 2023 03:50:39 GMT  
		Size: 284.7 KB (284697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63d189496f5f03c835c9c85df2db6920546d36a1701f6b5ad15f800c671605d`  
		Last Modified: Tue, 05 Dec 2023 20:31:27 GMT  
		Size: 67.0 MB (67003308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aeb88dd0f3e06a57abc08c781b85c89d138194918c469aea9a1bed9753d2ed0`  
		Last Modified: Tue, 05 Dec 2023 20:31:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40ff2505fd8d96e76bddb63b05c2d42815db1dabe0093ec8f8f53be403b0d01`  
		Last Modified: Tue, 05 Dec 2023 20:49:17 GMT  
		Size: 5.0 MB (4970029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3868d63c7cd554f20832e0aff9559fa0cdd7cdbaa4de14e8043fefd0ebfde5`  
		Last Modified: Tue, 05 Dec 2023 20:49:16 GMT  
		Size: 1.3 MB (1302235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a2748825cf9745fffb7f4807c0b6fd474a0221d0d19177142c3f952e10ac78`  
		Last Modified: Tue, 05 Dec 2023 20:49:16 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2c90abb7280a71391618e8552a4faa4e66eb61f80d02402126d25f1365cf063f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75409540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a539589e36806b442a969b2dcf589a62915dde0f6bee440eb73fda5d315a9dd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:53:48 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 00:53:48 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:49:18 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:49:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:49:36 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:49:36 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:49:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:49:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:49:37 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:11:53 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:11:53 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:11:53 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:11:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:11:53 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:11:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:11:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:11:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e7ba0492eb25e7f21078441d7cdc65088836bc1984bc4a14cd3e9cd75cbf32`  
		Last Modified: Fri, 01 Dec 2023 01:00:23 GMT  
		Size: 284.9 KB (284884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de60bcfc919bc6b53554a040a5a58936a8d2e2bf66b2872b69d7a3164e35923f`  
		Last Modified: Tue, 05 Dec 2023 20:54:54 GMT  
		Size: 65.8 MB (65764248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e61f3b09467cb2b97e65a90f25e38cba8acfcd387d168214a949b59bf8c09a`  
		Last Modified: Tue, 05 Dec 2023 20:54:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7827ddd1dfa7654d070274e573dbfcc8fb5ac2ef73888f8b0563e0672811ad`  
		Last Modified: Tue, 05 Dec 2023 21:12:11 GMT  
		Size: 5.0 MB (4964331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f919a9a90cd0240dfd228f8b093cb51b08bf03eabc0326cfe303219b37469f5`  
		Last Modified: Tue, 05 Dec 2023 21:12:11 GMT  
		Size: 1.2 MB (1248647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66464a5ea9ace101c6914e8c5da3a953cb5a9b372ffc562f6a7ab2bcc2b9c0a6`  
		Last Modified: Tue, 05 Dec 2023 21:12:11 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:f65daee5179d36a392c0d931a02c5c400f99b4470bd68e3f326d6828bd8f3fb6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74707169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53077f2480efa131c1c20460899eb69b049d624d249a844e4e1c3bd88aa28d12`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:44:57 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 08:44:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:58:01 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:58:16 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:58:16 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:58:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:58:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:58:17 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:22:31 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:22:31 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:22:31 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:22:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:22:31 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:22:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:22:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:22:32 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a824ff289f1a3c765a444079137b8b7f1cee80348faa53e1ba4c960b73ed2a`  
		Last Modified: Fri, 01 Dec 2023 08:49:42 GMT  
		Size: 284.1 KB (284079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4989177b4ed66b7e9f9e8c4bfce82720b582e24b735d6628effa75d81c5718fc`  
		Last Modified: Tue, 05 Dec 2023 21:04:43 GMT  
		Size: 65.8 MB (65764197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f9b58eae167c54d3faa3eeffd480cdae7e8b4841eb816a86cfdd01f8ae29ef`  
		Last Modified: Tue, 05 Dec 2023 21:04:29 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4cd1a3aab8fc02791b1e19f81b7de1bd691c10a7c942acc7e733221bf12888`  
		Last Modified: Tue, 05 Dec 2023 21:22:47 GMT  
		Size: 4.5 MB (4511237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3a92f0249b45814852e4e987e1a6304bcfb211077150ab43415b31d929f4af`  
		Last Modified: Tue, 05 Dec 2023 21:22:47 GMT  
		Size: 1.2 MB (1246087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3152bffd7f15885d0e72b0adabc22f46542f569db908b69d63eb29addd5e950`  
		Last Modified: Tue, 05 Dec 2023 21:22:47 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:977753f53683eb84ddc7477e5a743e0e1e4e2a001f20edfa0f01d43359d85dc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73981644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0f601640aa519cb421e86cd75a6ad6223541d58cfe80b27b699a23a2585ce70`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:43:53 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 03:18:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:16:18 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:16:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:16:28 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:16:28 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:16:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:16:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:16:28 GMT
WORKDIR /go
# Tue, 05 Dec 2023 20:38:16 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 20:38:16 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 20:38:16 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 20:38:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 20:38:16 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 20:38:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 20:38:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 20:38:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a63ed24dc22a348b35d99b5ec9dc67ff66563b539875e5c8ab2d870b3991ac`  
		Last Modified: Fri, 01 Dec 2023 02:44:03 GMT  
		Size: 286.3 KB (286307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f00641dffc5c2a149049ee9046bb24cfc7de534b7495a0f27784a4fff0fadc`  
		Last Modified: Tue, 05 Dec 2023 20:21:00 GMT  
		Size: 64.1 MB (64094844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452682ba77e89fc55be3a168358f5f43bccad93ecdd3d53b4dec7fff6915128b`  
		Last Modified: Tue, 05 Dec 2023 20:20:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3fe1e12507f8c4a2731393eebfc5ab973aa344b0daceec525560b812b26f60`  
		Last Modified: Tue, 05 Dec 2023 20:38:33 GMT  
		Size: 5.1 MB (5068450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb3c2fad921714e69ace0b18d8f72eb2566d50bc92ff9e9dd125ec383131eb9`  
		Last Modified: Tue, 05 Dec 2023 20:38:32 GMT  
		Size: 1.2 MB (1198449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9c40c8a39fcf5ab6fa64b1c2e1dd5d0b5c1f6b4d9c11ed9481644fe94f1cbf`  
		Last Modified: Tue, 05 Dec 2023 20:38:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:50de875c68ad6aeffc5eb2dd0942d219481fe70c55088657bbe724abd05f7c49
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74206489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7029045647c7331bb58455d58f274c3e4356d86729c097b8d3cfe35717b3b9d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:37:34 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 06:37:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:38:14 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:38:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:38:37 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:38:38 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:38:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:38:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:38:41 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:04:33 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:04:34 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:04:35 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:04:35 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:04:35 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:04:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:04:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:04:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692dbecd5e141c462ab06ef113ec964b525e7564d734890cc1d5b1dbf33ee34e`  
		Last Modified: Fri, 01 Dec 2023 06:43:30 GMT  
		Size: 286.7 KB (286661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc89a0f2d97ecfd4d20235e72227fc24aa79a64509fe9ea64702db658f2ad26d`  
		Last Modified: Tue, 05 Dec 2023 20:46:23 GMT  
		Size: 64.1 MB (64115804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d76f2c2e2bbb4190b1865ddafdc8cb88adee4c79d7d5ba23e69696e9610889`  
		Last Modified: Tue, 05 Dec 2023 20:46:11 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e0ec0f713ee657d6aa159fab65c05939480b5ca50a8e3dc4b1a9a6578160f7`  
		Last Modified: Tue, 05 Dec 2023 21:04:57 GMT  
		Size: 5.3 MB (5268970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e164016cca4964643911960baccae8beaa47cc5086bbe3ebfd14183d5204a8`  
		Last Modified: Tue, 05 Dec 2023 21:04:56 GMT  
		Size: 1.2 MB (1186171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2932f0ef681ac7135c1e7ff9332dd4c154c1f793d04fda438db30a1573bacc8b`  
		Last Modified: Tue, 05 Dec 2023 21:04:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:98d5d7af77acd9cc1b74499ba61056fb599a17742331f51a0fffa89ef56bb114
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76098838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d4f342a39bbb58bda0421e578348bf6d047bf7125db5c42216b2ba9b6d5040d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:14:49 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 08:14:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:44:16 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:44:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:45:03 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:45:04 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:45:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:45:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:45:05 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:14:29 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:14:29 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:14:29 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:14:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:14:30 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:14:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:14:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:14:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab563e8d41683e124df048aa9b564b0e8e1021e85213666971a015df51d5e48`  
		Last Modified: Fri, 01 Dec 2023 08:20:46 GMT  
		Size: 285.1 KB (285090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d44aea4caa072a45cb44ab86f401c76153b599207fb3cc311f44308e9b5da13`  
		Last Modified: Tue, 05 Dec 2023 20:57:00 GMT  
		Size: 66.2 MB (66218626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef66858f73257b9fd43395b7e2758cdaa72267303442d3a5dbef122796530c5`  
		Last Modified: Tue, 05 Dec 2023 20:56:49 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5261478888d8f0caaf878da0629c62f928bbbff35e7f873c1a463c6e39c0bd37`  
		Last Modified: Tue, 05 Dec 2023 21:14:53 GMT  
		Size: 5.1 MB (5114717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade58cb7b8ea422e0ab68cb58091d9adc84172a8de51990bb80269c07c5bd556`  
		Last Modified: Tue, 05 Dec 2023 21:14:53 GMT  
		Size: 1.3 MB (1262391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7f47ab035030fe8af075c6b5ebf045cd6bd32bef0700d8cc656ba7204685b7`  
		Last Modified: Tue, 05 Dec 2023 21:14:52 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:9a3cb11cfc419a512a550298d752bbf00ea5dc0b4daa8993ab10db26d145fda9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:a4a6967f69e81e55f736b4e5d91bab0e44ce577821e0336b8b8ef7456679e1c1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2154296990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14a551f4e77e9632ddd054915a37f355befe0b5201417194368482bc6a54949d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 02:47:03 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Nov 2023 02:47:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Nov 2023 02:47:05 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Nov 2023 02:47:06 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Nov 2023 02:48:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:48:31 GMT
ENV GOPATH=C:\go
# Thu, 16 Nov 2023 02:49:41 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 05 Dec 2023 20:18:04 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:21:11 GMT
RUN $url = 'https://dl.google.com/go/go1.21.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'bbe603cde7c9dee658f45164b4d06de1eff6e6e6b800100824e7c00d56a9a92f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 05 Dec 2023 20:21:13 GMT
WORKDIR C:\go
# Tue, 05 Dec 2023 20:59:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 05 Dec 2023 20:59:30 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 20:59:31 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 20:59:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:00:49 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 05 Dec 2023 21:00:50 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e901367fac1450f509d3118ada9e004e3613844ebdf91861147a093483930a4`  
		Last Modified: Thu, 16 Nov 2023 03:11:57 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e08004205bd077d8f22b013c70dc2f10796c64fced1eb9927e0055daff2d05d`  
		Last Modified: Thu, 16 Nov 2023 03:11:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebc5048afc68ef48e2f2136545e2cccf26bb29eb4926bf4259b370ad55b4e7a`  
		Last Modified: Thu, 16 Nov 2023 03:11:55 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f50fe5c7ef21648f3eaa4304932877a116fcb910b8e9095c779a2fbe6d57f7e`  
		Last Modified: Thu, 16 Nov 2023 03:11:55 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76fe0e37750041d4ede2a0ca3b5245cfe075c3eb2ee27d7ce72ee8c3d7b20cc`  
		Last Modified: Thu, 16 Nov 2023 03:12:00 GMT  
		Size: 25.5 MB (25537512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8097bb9b8778d15dbf89d899653bf1634ec17554e5d84ef1ccfcac8ebf86afe2`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b542d31e914d67da86cc5701cdc282ab664dc1170507e3802e22ab3026436a90`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 263.2 KB (263200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86acdf7d3955fb44136bac433a30ccbbb97863120f270af32659dd65446666c7`  
		Last Modified: Tue, 05 Dec 2023 20:39:22 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1abe126c354944b7db8aa724d8f757167f7c3b36d39f976ef3b1b0d1b1b65ab`  
		Last Modified: Tue, 05 Dec 2023 20:39:41 GMT  
		Size: 69.4 MB (69361283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6338af096e09067ad482a0f4a6df1d1eee5b5595a64ca5f367b94ce27903e284`  
		Last Modified: Tue, 05 Dec 2023 20:39:22 GMT  
		Size: 1.5 KB (1529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0adc218b27ef5639384c060fb663de3bd74374279d3fd525aa281f63a754779`  
		Last Modified: Tue, 05 Dec 2023 21:02:06 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c21053b248805df7ad888734f5cd1df5a6b426111512d5a6b7530060e7f30b2`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57f384772c293e1d97326febf9e29d6bfef6eb9da2b053b6ad1e0ebea539508`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a2cba3fcdba1e3612614837be0fed9e3b7670483867a14203a15d395aa4179`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b447549db21db40db8a08cddb7d529bbd6e183aba676f13e2a3a5ff034fb67f8`  
		Last Modified: Tue, 05 Dec 2023 21:02:04 GMT  
		Size: 1.7 MB (1685436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408a12340d35fbfeee8cc5bdec3421ede796686f2b22d693863de08da6d51c91`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:b98db9d0f32752a5a646d4009012af66a84d26002c3605d6fe3da6769aede98d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2113; amd64

### `caddy:2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:081774d66d26fdb1b8b89fc90aeb9a72c559c0690770f153fa4ca3f1d5450e43
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1983623458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af2bcbcbf997ed6d0e17a2acebd1f65d19dbb6868d0523c306342bcc37644dd6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 09 Nov 2023 06:47:20 GMT
RUN Install update 10.0.20348.2113
# Thu, 16 Nov 2023 01:36:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 02:43:34 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Nov 2023 02:43:35 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Nov 2023 02:43:36 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Nov 2023 02:43:37 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Nov 2023 02:44:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:44:11 GMT
ENV GOPATH=C:\go
# Thu, 16 Nov 2023 02:44:30 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 05 Dec 2023 20:15:35 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:17:49 GMT
RUN $url = 'https://dl.google.com/go/go1.21.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'bbe603cde7c9dee658f45164b4d06de1eff6e6e6b800100824e7c00d56a9a92f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 05 Dec 2023 20:17:50 GMT
WORKDIR C:\go
# Tue, 05 Dec 2023 21:00:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 05 Dec 2023 21:00:58 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:00:59 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:01:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:01:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 05 Dec 2023 21:01:26 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7989ef2c4cfb06d845746a3c3660481ea84d3f5c8216041855ce528f0ac4015c`  
		Last Modified: Tue, 14 Nov 2023 20:43:13 GMT  
		Size: 498.2 MB (498182566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbeb193d02c2ca7f9a9ea438fbf1bcdb6ea4a6fea626713330fd1ebb514424f`  
		Last Modified: Thu, 16 Nov 2023 02:25:14 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b1d4a557f047b695f94452d9707061981d7fae4239c674b332282b8291963c`  
		Last Modified: Thu, 16 Nov 2023 03:11:20 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45549c207f14d769cba7c36b66157ec213bbc32ce57d685d8e2c407cf3987bb`  
		Last Modified: Thu, 16 Nov 2023 03:11:18 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c674717e06bf8cb25d5887393ef9568ee0ab6390966b9666808e836e9bd471d`  
		Last Modified: Thu, 16 Nov 2023 03:11:18 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2227badcd9f5f2b70b3d2ffd1c18887498f413c07802bfb334e8dc7b2d2acc`  
		Last Modified: Thu, 16 Nov 2023 03:11:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9f3b5e90a2e6028cf194e870b24a7158f875f18b81f4f9137a5db3ea1f79ac`  
		Last Modified: Thu, 16 Nov 2023 03:11:23 GMT  
		Size: 25.5 MB (25536225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7811a5416dcd19193a5b3ab9327607bf845f7ff77f95d3e20abdfb7435c32ae0`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5931209e960a94616639ea72e4d3ad9dc9cb554790ce930152c73bdc1449c034`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 266.6 KB (266600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a70f603a2fb4e76edd3165b62a179fb8f6410e265f5ae4a3732ee68e610034b`  
		Last Modified: Tue, 05 Dec 2023 20:38:48 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e37840dec3a6665ce48520be8b2c51b654359765bee5ab0780ee74746f0eb2`  
		Last Modified: Tue, 05 Dec 2023 20:39:08 GMT  
		Size: 69.3 MB (69342960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d16ae54757acda093616d24735d4c92d4676649bec49807fc35de90d15e15c`  
		Last Modified: Tue, 05 Dec 2023 20:38:48 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5744d01eddd2ef9d9673fdb0f0e48203fad1b01f2b14899a3ec6393c4548e75`  
		Last Modified: Tue, 05 Dec 2023 21:02:23 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35bb848667aa413b6ce6c309a4c2169635b0740dc335b9b39413a00627c01ab`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78369d5e83dd4f4ca5558a32848f3515e191b15f8427ea166a4f6327694ff9db`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2ae381a5e49194e43b26ac8036b1da5d2af930f7516796c476bcdb9c8125e3`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09db71960c4c717ed44d2694cf77f248223822e163297046010868c3ebf0767`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.7 MB (1677926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9dfae036c2fe0cfcd2e4f5a9acc265c45af769542844b9b617b62ec3ebd591`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:b2a860f9d095b10b5613cfd76162decff7840f5881e3c5ecf4e01d29d829c405
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.5122; amd64
	-	windows version 10.0.20348.2113; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:38df49f40c98b8d866440b7fec4635fcf669f4c138fd001b95f457b42e4e2265
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2073433228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7105669fddc0d611982501b46d56df54a820ca14cd7e3a3c62c02ef1bd40fc2e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:30:07 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Nov 2023 05:30:07 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:31:22 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Nov 2023 05:31:23 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Nov 2023 05:31:24 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Nov 2023 05:31:25 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 16 Nov 2023 05:31:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Nov 2023 05:31:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Nov 2023 05:31:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Nov 2023 05:31:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Nov 2023 05:31:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Nov 2023 05:31:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Nov 2023 05:31:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Nov 2023 05:31:32 GMT
EXPOSE 80
# Thu, 16 Nov 2023 05:31:33 GMT
EXPOSE 443
# Thu, 16 Nov 2023 05:31:34 GMT
EXPOSE 443/udp
# Thu, 16 Nov 2023 05:31:35 GMT
EXPOSE 2019
# Thu, 16 Nov 2023 05:32:33 GMT
RUN caddy version
# Thu, 16 Nov 2023 05:32:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d66ae500a331057bbb6b25a0c0e5718f2491209d7330f70b1203472b199bd5b`  
		Last Modified: Thu, 16 Nov 2023 05:37:31 GMT  
		Size: 451.2 KB (451175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec48b5261067a4b4643799633487cce5b6ee11cce36314b8a6b22964fd46ba4`  
		Last Modified: Thu, 16 Nov 2023 05:37:30 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bc40730815ee35e950756a15aa93561edd0f272d34d30de69bb8d7f58b1d8e`  
		Last Modified: Thu, 16 Nov 2023 05:37:34 GMT  
		Size: 15.3 MB (15273771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfce8b69f4cadeeaa9fcc771a3a5b374fc4a3c8c41c1a42a7878c1cad861645c`  
		Last Modified: Thu, 16 Nov 2023 05:37:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdd09852c86166de537f8b5f5b78eca092cfb95e9e2e1194c84a7a05334e5c4`  
		Last Modified: Thu, 16 Nov 2023 05:37:29 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f15c2b10239537d18dc39c5208acb0c8fc7bc25d6cd95cb59ed8e8aaf8b73be`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa35da536891cce8df35bca524d15b1b7465d4fc14354a1a15a2fa39d71a4a88`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654652f0bb6c82a0e1fd51010fd587112527866df3c9748cf9ed4414e70ee612`  
		Last Modified: Thu, 16 Nov 2023 05:37:29 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0fcd5cbdfe3f968d65ba5dcece2d017de82a3a4ec737745bd5560697735689`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9396734c66d2d27545fdeb2c33a462651a3807dfcbd04b590a01ace722161a21`  
		Last Modified: Thu, 16 Nov 2023 05:37:27 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a14586579bd1d9d9a9162b0678a119c826a7be5039b5419e90b82c772b33677`  
		Last Modified: Thu, 16 Nov 2023 05:37:27 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c773c8968545d0fca628d03a3b588ca4798423090cadd666d023cee5065235a5`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce86207f89519b9df4526afc22e743fef4a6266614fb8e082e975bf0f01862f`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7392ec7da7419f69c0413116467249934c403f42b53ff6090608481e1ba7985a`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73d1eee374e37176384bade9abdbe65d5aed23b976c507b3b88b17c758761f`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d556f28b534238f3c8497a928caa36428f1d333a69cabf15b4fc3d80aa7f3f9f`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd0eba7ede6da63115506e40bf2b6990915e5fba916e919c6525f447018bbd9`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf5b269f798b76bfba9ad2e27b5aab7bebe448007c818230643c16d6cf761af`  
		Last Modified: Thu, 16 Nov 2023 05:37:25 GMT  
		Size: 252.7 KB (252713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c70c9a3deaf4a41d4192a9248f3fd5ccfadb54792687f31f63a17f46e5134c`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:7a86ad9fb59b43cc97f50c3516b4153bb228276c026e4c802c4a213b0fe1c20f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1902803411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03625f7f4ec599de5399e0e9d5f36d3c2052adeb06f8349ef7a96e3777ddf4e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 09 Nov 2023 06:47:20 GMT
RUN Install update 10.0.20348.2113
# Thu, 16 Nov 2023 01:36:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:33:15 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Nov 2023 05:33:16 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:33:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Nov 2023 05:33:45 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Nov 2023 05:33:46 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Nov 2023 05:33:47 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 16 Nov 2023 05:33:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Nov 2023 05:33:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Nov 2023 05:33:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Nov 2023 05:33:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Nov 2023 05:33:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Nov 2023 05:33:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Nov 2023 05:33:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Nov 2023 05:33:54 GMT
EXPOSE 80
# Thu, 16 Nov 2023 05:33:55 GMT
EXPOSE 443
# Thu, 16 Nov 2023 05:33:56 GMT
EXPOSE 443/udp
# Thu, 16 Nov 2023 05:33:57 GMT
EXPOSE 2019
# Thu, 16 Nov 2023 05:34:33 GMT
RUN caddy version
# Thu, 16 Nov 2023 05:34:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7989ef2c4cfb06d845746a3c3660481ea84d3f5c8216041855ce528f0ac4015c`  
		Last Modified: Tue, 14 Nov 2023 20:43:13 GMT  
		Size: 498.2 MB (498182566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbeb193d02c2ca7f9a9ea438fbf1bcdb6ea4a6fea626713330fd1ebb514424f`  
		Last Modified: Thu, 16 Nov 2023 02:25:14 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b269b5ac8d8c6baa501ca9b38fa715170022416aa7332a2d155a06529882b84a`  
		Last Modified: Thu, 16 Nov 2023 05:37:59 GMT  
		Size: 458.2 KB (458201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f982a236809063ef75b5db6a226207448d936d7791ede196115611649805c5`  
		Last Modified: Thu, 16 Nov 2023 05:37:58 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2783cb5dad5df996a48a9ebf989a6136c91f524f421bfff9e71ab764da46fd04`  
		Last Modified: Thu, 16 Nov 2023 05:38:01 GMT  
		Size: 15.3 MB (15269735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa26255a8f194a0aa31a8fd0c48e7dfba117358880abeaf7ad3c5f54a6be87d`  
		Last Modified: Thu, 16 Nov 2023 05:37:57 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706b8120af6e900b1d0dea48743c4fd50b63c785dbe02b5ccd4af53e68ebefff`  
		Last Modified: Thu, 16 Nov 2023 05:37:57 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c12376eb1027b4892f92b1b8dd45b1e05d78f365c2886ded9202ffbaab80e9`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a29b9f98e523c3477366f98e560b8638fb5c3f0a7a8c76c9a417a33b4d44804`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a9a2fb5b49cb3e38b64f06a755f57ec37b8b5eaf2152fe9e38ae9c8cb3b593`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53a0ea77b4fcc256276d31401de856267c72aeac7fefeeb6fbe655340bb4cf4`  
		Last Modified: Thu, 16 Nov 2023 05:37:55 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d80b783b85d05309ef9fe97740b873bd9092c13b53eea3d83adf6197cbe798`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9454c6602eef29f64927e75d96b8f26d7cf0c6c089afa91e260207675216501`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f23d9fc021e786b83141dd57c2a10dc279d17eacad254ec81d7922372d17876`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55a4267cea49483a79cbee8908d3daf6af4fb6fa1af94e350072034f128c5a1`  
		Last Modified: Thu, 16 Nov 2023 05:37:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9723590c56e28022e6ee055495ee5826c7ea085d2a8b7255d471b35bb27e9a6c`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b39c632f1f53a232721260e3ebcc755559883edb0272949f2d965799d62ef5`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3deb93ce29c0157e6c6b82bbad0ffb2102a833ea54672c93c05843899eac3bc`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09fe12ffad65804e54e566d7b3256d98268c5e943a40282d44bab50d3fb6a04`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517e7fd42cd9750ca7ef5a68df02e2bdc3be404dbd69681f36c7b0acb1562550`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 270.1 KB (270069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0727df29cc57ce0bb7db3c73852d6eaceb439603493f2e3ceb07ce2f8e8e4e99`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:2e8fbf0e299d85c14b2ac578c2ff6ee6f32e2e0c7dbd4afd5f683286575971d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:38df49f40c98b8d866440b7fec4635fcf669f4c138fd001b95f457b42e4e2265
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2073433228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7105669fddc0d611982501b46d56df54a820ca14cd7e3a3c62c02ef1bd40fc2e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:30:07 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Nov 2023 05:30:07 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:31:22 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Nov 2023 05:31:23 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Nov 2023 05:31:24 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Nov 2023 05:31:25 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 16 Nov 2023 05:31:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Nov 2023 05:31:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Nov 2023 05:31:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Nov 2023 05:31:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Nov 2023 05:31:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Nov 2023 05:31:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Nov 2023 05:31:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Nov 2023 05:31:32 GMT
EXPOSE 80
# Thu, 16 Nov 2023 05:31:33 GMT
EXPOSE 443
# Thu, 16 Nov 2023 05:31:34 GMT
EXPOSE 443/udp
# Thu, 16 Nov 2023 05:31:35 GMT
EXPOSE 2019
# Thu, 16 Nov 2023 05:32:33 GMT
RUN caddy version
# Thu, 16 Nov 2023 05:32:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d66ae500a331057bbb6b25a0c0e5718f2491209d7330f70b1203472b199bd5b`  
		Last Modified: Thu, 16 Nov 2023 05:37:31 GMT  
		Size: 451.2 KB (451175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec48b5261067a4b4643799633487cce5b6ee11cce36314b8a6b22964fd46ba4`  
		Last Modified: Thu, 16 Nov 2023 05:37:30 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bc40730815ee35e950756a15aa93561edd0f272d34d30de69bb8d7f58b1d8e`  
		Last Modified: Thu, 16 Nov 2023 05:37:34 GMT  
		Size: 15.3 MB (15273771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfce8b69f4cadeeaa9fcc771a3a5b374fc4a3c8c41c1a42a7878c1cad861645c`  
		Last Modified: Thu, 16 Nov 2023 05:37:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdd09852c86166de537f8b5f5b78eca092cfb95e9e2e1194c84a7a05334e5c4`  
		Last Modified: Thu, 16 Nov 2023 05:37:29 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f15c2b10239537d18dc39c5208acb0c8fc7bc25d6cd95cb59ed8e8aaf8b73be`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa35da536891cce8df35bca524d15b1b7465d4fc14354a1a15a2fa39d71a4a88`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654652f0bb6c82a0e1fd51010fd587112527866df3c9748cf9ed4414e70ee612`  
		Last Modified: Thu, 16 Nov 2023 05:37:29 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0fcd5cbdfe3f968d65ba5dcece2d017de82a3a4ec737745bd5560697735689`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9396734c66d2d27545fdeb2c33a462651a3807dfcbd04b590a01ace722161a21`  
		Last Modified: Thu, 16 Nov 2023 05:37:27 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a14586579bd1d9d9a9162b0678a119c826a7be5039b5419e90b82c772b33677`  
		Last Modified: Thu, 16 Nov 2023 05:37:27 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c773c8968545d0fca628d03a3b588ca4798423090cadd666d023cee5065235a5`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce86207f89519b9df4526afc22e743fef4a6266614fb8e082e975bf0f01862f`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7392ec7da7419f69c0413116467249934c403f42b53ff6090608481e1ba7985a`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73d1eee374e37176384bade9abdbe65d5aed23b976c507b3b88b17c758761f`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d556f28b534238f3c8497a928caa36428f1d333a69cabf15b4fc3d80aa7f3f9f`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd0eba7ede6da63115506e40bf2b6990915e5fba916e919c6525f447018bbd9`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf5b269f798b76bfba9ad2e27b5aab7bebe448007c818230643c16d6cf761af`  
		Last Modified: Thu, 16 Nov 2023 05:37:25 GMT  
		Size: 252.7 KB (252713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c70c9a3deaf4a41d4192a9248f3fd5ccfadb54792687f31f63a17f46e5134c`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:7302fa54b56c8f2363f0caf1ac496c297c9eda88207a05836e5e06c40272769b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2113; amd64

### `caddy:2-windowsservercore-ltsc2022` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:7a86ad9fb59b43cc97f50c3516b4153bb228276c026e4c802c4a213b0fe1c20f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1902803411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03625f7f4ec599de5399e0e9d5f36d3c2052adeb06f8349ef7a96e3777ddf4e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 09 Nov 2023 06:47:20 GMT
RUN Install update 10.0.20348.2113
# Thu, 16 Nov 2023 01:36:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:33:15 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Nov 2023 05:33:16 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:33:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Nov 2023 05:33:45 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Nov 2023 05:33:46 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Nov 2023 05:33:47 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 16 Nov 2023 05:33:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Nov 2023 05:33:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Nov 2023 05:33:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Nov 2023 05:33:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Nov 2023 05:33:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Nov 2023 05:33:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Nov 2023 05:33:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Nov 2023 05:33:54 GMT
EXPOSE 80
# Thu, 16 Nov 2023 05:33:55 GMT
EXPOSE 443
# Thu, 16 Nov 2023 05:33:56 GMT
EXPOSE 443/udp
# Thu, 16 Nov 2023 05:33:57 GMT
EXPOSE 2019
# Thu, 16 Nov 2023 05:34:33 GMT
RUN caddy version
# Thu, 16 Nov 2023 05:34:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7989ef2c4cfb06d845746a3c3660481ea84d3f5c8216041855ce528f0ac4015c`  
		Last Modified: Tue, 14 Nov 2023 20:43:13 GMT  
		Size: 498.2 MB (498182566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbeb193d02c2ca7f9a9ea438fbf1bcdb6ea4a6fea626713330fd1ebb514424f`  
		Last Modified: Thu, 16 Nov 2023 02:25:14 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b269b5ac8d8c6baa501ca9b38fa715170022416aa7332a2d155a06529882b84a`  
		Last Modified: Thu, 16 Nov 2023 05:37:59 GMT  
		Size: 458.2 KB (458201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f982a236809063ef75b5db6a226207448d936d7791ede196115611649805c5`  
		Last Modified: Thu, 16 Nov 2023 05:37:58 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2783cb5dad5df996a48a9ebf989a6136c91f524f421bfff9e71ab764da46fd04`  
		Last Modified: Thu, 16 Nov 2023 05:38:01 GMT  
		Size: 15.3 MB (15269735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa26255a8f194a0aa31a8fd0c48e7dfba117358880abeaf7ad3c5f54a6be87d`  
		Last Modified: Thu, 16 Nov 2023 05:37:57 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706b8120af6e900b1d0dea48743c4fd50b63c785dbe02b5ccd4af53e68ebefff`  
		Last Modified: Thu, 16 Nov 2023 05:37:57 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c12376eb1027b4892f92b1b8dd45b1e05d78f365c2886ded9202ffbaab80e9`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a29b9f98e523c3477366f98e560b8638fb5c3f0a7a8c76c9a417a33b4d44804`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a9a2fb5b49cb3e38b64f06a755f57ec37b8b5eaf2152fe9e38ae9c8cb3b593`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53a0ea77b4fcc256276d31401de856267c72aeac7fefeeb6fbe655340bb4cf4`  
		Last Modified: Thu, 16 Nov 2023 05:37:55 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d80b783b85d05309ef9fe97740b873bd9092c13b53eea3d83adf6197cbe798`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9454c6602eef29f64927e75d96b8f26d7cf0c6c089afa91e260207675216501`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f23d9fc021e786b83141dd57c2a10dc279d17eacad254ec81d7922372d17876`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55a4267cea49483a79cbee8908d3daf6af4fb6fa1af94e350072034f128c5a1`  
		Last Modified: Thu, 16 Nov 2023 05:37:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9723590c56e28022e6ee055495ee5826c7ea085d2a8b7255d471b35bb27e9a6c`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b39c632f1f53a232721260e3ebcc755559883edb0272949f2d965799d62ef5`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3deb93ce29c0157e6c6b82bbad0ffb2102a833ea54672c93c05843899eac3bc`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09fe12ffad65804e54e566d7b3256d98268c5e943a40282d44bab50d3fb6a04`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517e7fd42cd9750ca7ef5a68df02e2bdc3be404dbd69681f36c7b0acb1562550`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 270.1 KB (270069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0727df29cc57ce0bb7db3c73852d6eaceb439603493f2e3ceb07ce2f8e8e4e99`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7`

```console
$ docker pull caddy@sha256:9eb928f0a3142d0a38e6d457f7696c08c13e070d49d6499cc5b0afe644ecb281
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.5122; amd64
	-	windows version 10.0.20348.2113; amd64

### `caddy:2.7` - linux; amd64

```console
$ docker pull caddy@sha256:0eff0e7322c718fc65b783418531f1e75c7f27f1a3877823378737e91296ee8c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18474760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3791fd914060b4c02165b77f6f2c6e4516be2e77a6a8bd8ffab228253f75f47`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:32:06 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 06:32:07 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 06:32:07 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 06:32:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 06:32:10 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 06:32:10 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 06:32:10 GMT
EXPOSE 80
# Fri, 01 Dec 2023 06:32:11 GMT
EXPOSE 443
# Fri, 01 Dec 2023 06:32:11 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 06:32:11 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 06:32:11 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 06:32:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08886dfc0722c4ed2cb6a70c285a33fe35aec069435868488356dde320b4d21c`  
		Last Modified: Fri, 01 Dec 2023 06:32:30 GMT  
		Size: 350.8 KB (350845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0132c3b72c65b40cace6033d219e1e6d680bb85808270b77a5189c509c10bc0`  
		Last Modified: Fri, 01 Dec 2023 06:32:29 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2ecdf85e2f8f19fc737312e7157f0141b45020324fcf01f4e92bbe707d8983`  
		Last Modified: Fri, 01 Dec 2023 06:32:32 GMT  
		Size: 14.7 MB (14713987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e05dc14b4b6c6dbdcfbdbe28c73e86cafc5287fa13d4f51fdfdfad7b51b8936d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17423853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3acb342ef8cbce6055e45fdabe7e8b60e98cab9d0aa967e362098333633440ff`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:39:01 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 00:39:02 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 00:39:03 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 00:39:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 00:39:05 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 00:39:05 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 00:39:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 00:39:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 00:39:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 80
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 443
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 00:39:06 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 00:39:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc24e4ccf558b6e992efaaa7a735322be11fe99ce19e722eee6ae70bb76515d`  
		Last Modified: Fri, 01 Dec 2023 00:39:21 GMT  
		Size: 347.6 KB (347632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cd6f3873930f7c6aa4ee5d06ef24c77a840fec6f0211e9572fbe0f43c04e1f`  
		Last Modified: Fri, 01 Dec 2023 00:39:21 GMT  
		Size: 7.5 KB (7508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c51a919a8bb024456b258f25a71adb53a14e30c7134e81fac343c44dbf7230c`  
		Last Modified: Fri, 01 Dec 2023 00:39:23 GMT  
		Size: 13.9 MB (13921843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - linux; arm variant v7

```console
$ docker pull caddy@sha256:c3be58f3d1b5614d2a5e7bff50bc07567044bb119ec0f286c94df8169efc313b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17156415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194c773f5747022fdb5fc8d32e8dafcafd61f37e52238ad53627e3309c2fb4cb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:19:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 03:19:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 03:19:15 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 03:19:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 03:19:19 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 03:19:19 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 03:19:20 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 03:19:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 03:19:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 03:19:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 03:19:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 03:19:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 03:19:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 03:19:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 03:19:22 GMT
EXPOSE 80
# Fri, 01 Dec 2023 03:19:22 GMT
EXPOSE 443
# Fri, 01 Dec 2023 03:19:23 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 03:19:23 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 03:19:23 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 03:19:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803b34e1f84b29ca968d2fbf85c278608566c34dfd1742e088c6483685957029`  
		Last Modified: Fri, 01 Dec 2023 03:19:48 GMT  
		Size: 344.5 KB (344464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bbcb291a405e073d645e52039b6f84fa5071645ceb53988f99d384fbc6c4c1`  
		Last Modified: Fri, 01 Dec 2023 03:19:48 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d0aed5710d79e6bba64ce3cf139d40c4e2c3003d1feec3776b18919e3a1423`  
		Last Modified: Fri, 01 Dec 2023 03:19:50 GMT  
		Size: 13.9 MB (13903440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e7f68eb0f76a55ada8be1bb5213e5bbbcb0727fa8d4051f6f3edf1275bc2dc40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17274998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9487e6591f483b0f0d5fe25a89d069485fa10bb97a06ef07085f28b86995977c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:11:08 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 03:11:09 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 03:11:10 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 03:11:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 03:11:11 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 03:11:11 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 80
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 443
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 03:11:12 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 03:11:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e383270d6915b6b427f49a75d657d5a0403fcd47a5f89cd30e85143ca54c22`  
		Last Modified: Fri, 01 Dec 2023 03:11:28 GMT  
		Size: 360.7 KB (360655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27e927f808292c7b306432ed3ee61ecc6b7f637b8ccbdf5cb2d6bdc24649858`  
		Last Modified: Fri, 01 Dec 2023 03:11:28 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dab02cb145c1d5336977666f796446f69abbbfa721ab7a71525867eb3edfbc`  
		Last Modified: Fri, 01 Dec 2023 03:11:30 GMT  
		Size: 13.6 MB (13573804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - linux; ppc64le

```console
$ docker pull caddy@sha256:3f9f202dc07f3bb097e0e78330d59f52c488ff4ba3b4aa4a569f1a28c9db95f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.1 MB (17058981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:126d26f69982d49f88bac36f166a92d251494018b25e2e255972b98f38f495f8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:42:19 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 05:42:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 05:42:52 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 05:42:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 05:43:00 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 05:43:20 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 05:43:24 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 05:43:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 05:43:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 05:43:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 05:43:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 05:43:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 05:43:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 05:43:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 05:43:45 GMT
EXPOSE 80
# Fri, 01 Dec 2023 05:43:46 GMT
EXPOSE 443
# Fri, 01 Dec 2023 05:43:46 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 05:43:47 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 05:43:48 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 05:43:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce4bc2907f69809c3086f118895d7e5c8683349557239c0ce79dfbda0ce3768`  
		Last Modified: Fri, 01 Dec 2023 05:44:17 GMT  
		Size: 362.2 KB (362185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef8889b660799cb5b3c54f8771b4a37ad12c12f245aa74e4af501a899449137`  
		Last Modified: Fri, 01 Dec 2023 05:44:17 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681f2bb9965ff577316200c634bfb7e7db0d5b2ba971441db97e1405e3c0fc6b`  
		Last Modified: Fri, 01 Dec 2023 05:44:19 GMT  
		Size: 13.3 MB (13340969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - linux; s390x

```console
$ docker pull caddy@sha256:159a339dbc4d0e8279faad422e0a871d82adcc6736b9c4ac4c4b252c3dbee6a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.8 MB (17825031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0c61727c246c9eedd4c40bc927993a89531560cc027902c6f00b8f288f96b77`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:22:31 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 08:22:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 08:22:32 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 08:22:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 08:22:37 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 08:22:37 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 08:22:38 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 08:22:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 80
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 443
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 08:22:38 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 08:22:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20bbe0abb0a3f63718aa78742832077ad86b8ae86d70ce3ebcece342ec022c6`  
		Last Modified: Fri, 01 Dec 2023 08:23:07 GMT  
		Size: 354.9 KB (354948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1497491e477a92a5e82d0d68588396a3414c6e703fdc68c82c768ad6b18b28`  
		Last Modified: Fri, 01 Dec 2023 08:23:07 GMT  
		Size: 7.5 KB (7502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539ac3a1bb2d355499d388b4de966f9148263d5603f2db92aeba42084d02b3cf`  
		Last Modified: Fri, 01 Dec 2023 08:23:09 GMT  
		Size: 14.2 MB (14245127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:38df49f40c98b8d866440b7fec4635fcf669f4c138fd001b95f457b42e4e2265
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2073433228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7105669fddc0d611982501b46d56df54a820ca14cd7e3a3c62c02ef1bd40fc2e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:30:07 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Nov 2023 05:30:07 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:31:22 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Nov 2023 05:31:23 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Nov 2023 05:31:24 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Nov 2023 05:31:25 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 16 Nov 2023 05:31:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Nov 2023 05:31:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Nov 2023 05:31:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Nov 2023 05:31:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Nov 2023 05:31:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Nov 2023 05:31:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Nov 2023 05:31:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Nov 2023 05:31:32 GMT
EXPOSE 80
# Thu, 16 Nov 2023 05:31:33 GMT
EXPOSE 443
# Thu, 16 Nov 2023 05:31:34 GMT
EXPOSE 443/udp
# Thu, 16 Nov 2023 05:31:35 GMT
EXPOSE 2019
# Thu, 16 Nov 2023 05:32:33 GMT
RUN caddy version
# Thu, 16 Nov 2023 05:32:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d66ae500a331057bbb6b25a0c0e5718f2491209d7330f70b1203472b199bd5b`  
		Last Modified: Thu, 16 Nov 2023 05:37:31 GMT  
		Size: 451.2 KB (451175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec48b5261067a4b4643799633487cce5b6ee11cce36314b8a6b22964fd46ba4`  
		Last Modified: Thu, 16 Nov 2023 05:37:30 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bc40730815ee35e950756a15aa93561edd0f272d34d30de69bb8d7f58b1d8e`  
		Last Modified: Thu, 16 Nov 2023 05:37:34 GMT  
		Size: 15.3 MB (15273771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfce8b69f4cadeeaa9fcc771a3a5b374fc4a3c8c41c1a42a7878c1cad861645c`  
		Last Modified: Thu, 16 Nov 2023 05:37:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdd09852c86166de537f8b5f5b78eca092cfb95e9e2e1194c84a7a05334e5c4`  
		Last Modified: Thu, 16 Nov 2023 05:37:29 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f15c2b10239537d18dc39c5208acb0c8fc7bc25d6cd95cb59ed8e8aaf8b73be`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa35da536891cce8df35bca524d15b1b7465d4fc14354a1a15a2fa39d71a4a88`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654652f0bb6c82a0e1fd51010fd587112527866df3c9748cf9ed4414e70ee612`  
		Last Modified: Thu, 16 Nov 2023 05:37:29 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0fcd5cbdfe3f968d65ba5dcece2d017de82a3a4ec737745bd5560697735689`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9396734c66d2d27545fdeb2c33a462651a3807dfcbd04b590a01ace722161a21`  
		Last Modified: Thu, 16 Nov 2023 05:37:27 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a14586579bd1d9d9a9162b0678a119c826a7be5039b5419e90b82c772b33677`  
		Last Modified: Thu, 16 Nov 2023 05:37:27 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c773c8968545d0fca628d03a3b588ca4798423090cadd666d023cee5065235a5`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce86207f89519b9df4526afc22e743fef4a6266614fb8e082e975bf0f01862f`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7392ec7da7419f69c0413116467249934c403f42b53ff6090608481e1ba7985a`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73d1eee374e37176384bade9abdbe65d5aed23b976c507b3b88b17c758761f`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d556f28b534238f3c8497a928caa36428f1d333a69cabf15b4fc3d80aa7f3f9f`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd0eba7ede6da63115506e40bf2b6990915e5fba916e919c6525f447018bbd9`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf5b269f798b76bfba9ad2e27b5aab7bebe448007c818230643c16d6cf761af`  
		Last Modified: Thu, 16 Nov 2023 05:37:25 GMT  
		Size: 252.7 KB (252713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c70c9a3deaf4a41d4192a9248f3fd5ccfadb54792687f31f63a17f46e5134c`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:7a86ad9fb59b43cc97f50c3516b4153bb228276c026e4c802c4a213b0fe1c20f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1902803411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03625f7f4ec599de5399e0e9d5f36d3c2052adeb06f8349ef7a96e3777ddf4e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 09 Nov 2023 06:47:20 GMT
RUN Install update 10.0.20348.2113
# Thu, 16 Nov 2023 01:36:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:33:15 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Nov 2023 05:33:16 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:33:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Nov 2023 05:33:45 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Nov 2023 05:33:46 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Nov 2023 05:33:47 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 16 Nov 2023 05:33:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Nov 2023 05:33:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Nov 2023 05:33:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Nov 2023 05:33:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Nov 2023 05:33:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Nov 2023 05:33:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Nov 2023 05:33:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Nov 2023 05:33:54 GMT
EXPOSE 80
# Thu, 16 Nov 2023 05:33:55 GMT
EXPOSE 443
# Thu, 16 Nov 2023 05:33:56 GMT
EXPOSE 443/udp
# Thu, 16 Nov 2023 05:33:57 GMT
EXPOSE 2019
# Thu, 16 Nov 2023 05:34:33 GMT
RUN caddy version
# Thu, 16 Nov 2023 05:34:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7989ef2c4cfb06d845746a3c3660481ea84d3f5c8216041855ce528f0ac4015c`  
		Last Modified: Tue, 14 Nov 2023 20:43:13 GMT  
		Size: 498.2 MB (498182566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbeb193d02c2ca7f9a9ea438fbf1bcdb6ea4a6fea626713330fd1ebb514424f`  
		Last Modified: Thu, 16 Nov 2023 02:25:14 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b269b5ac8d8c6baa501ca9b38fa715170022416aa7332a2d155a06529882b84a`  
		Last Modified: Thu, 16 Nov 2023 05:37:59 GMT  
		Size: 458.2 KB (458201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f982a236809063ef75b5db6a226207448d936d7791ede196115611649805c5`  
		Last Modified: Thu, 16 Nov 2023 05:37:58 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2783cb5dad5df996a48a9ebf989a6136c91f524f421bfff9e71ab764da46fd04`  
		Last Modified: Thu, 16 Nov 2023 05:38:01 GMT  
		Size: 15.3 MB (15269735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa26255a8f194a0aa31a8fd0c48e7dfba117358880abeaf7ad3c5f54a6be87d`  
		Last Modified: Thu, 16 Nov 2023 05:37:57 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706b8120af6e900b1d0dea48743c4fd50b63c785dbe02b5ccd4af53e68ebefff`  
		Last Modified: Thu, 16 Nov 2023 05:37:57 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c12376eb1027b4892f92b1b8dd45b1e05d78f365c2886ded9202ffbaab80e9`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a29b9f98e523c3477366f98e560b8638fb5c3f0a7a8c76c9a417a33b4d44804`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a9a2fb5b49cb3e38b64f06a755f57ec37b8b5eaf2152fe9e38ae9c8cb3b593`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53a0ea77b4fcc256276d31401de856267c72aeac7fefeeb6fbe655340bb4cf4`  
		Last Modified: Thu, 16 Nov 2023 05:37:55 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d80b783b85d05309ef9fe97740b873bd9092c13b53eea3d83adf6197cbe798`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9454c6602eef29f64927e75d96b8f26d7cf0c6c089afa91e260207675216501`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f23d9fc021e786b83141dd57c2a10dc279d17eacad254ec81d7922372d17876`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55a4267cea49483a79cbee8908d3daf6af4fb6fa1af94e350072034f128c5a1`  
		Last Modified: Thu, 16 Nov 2023 05:37:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9723590c56e28022e6ee055495ee5826c7ea085d2a8b7255d471b35bb27e9a6c`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b39c632f1f53a232721260e3ebcc755559883edb0272949f2d965799d62ef5`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3deb93ce29c0157e6c6b82bbad0ffb2102a833ea54672c93c05843899eac3bc`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09fe12ffad65804e54e566d7b3256d98268c5e943a40282d44bab50d3fb6a04`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517e7fd42cd9750ca7ef5a68df02e2bdc3be404dbd69681f36c7b0acb1562550`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 270.1 KB (270069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0727df29cc57ce0bb7db3c73852d6eaceb439603493f2e3ceb07ce2f8e8e4e99`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-alpine`

```console
$ docker pull caddy@sha256:9821d1ef822957bf0ac22f9c6e26ad6a3198604f29b3b79194acba7ccaff4532
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
$ docker pull caddy@sha256:0eff0e7322c718fc65b783418531f1e75c7f27f1a3877823378737e91296ee8c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18474760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3791fd914060b4c02165b77f6f2c6e4516be2e77a6a8bd8ffab228253f75f47`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:32:06 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 06:32:07 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 06:32:07 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 06:32:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 06:32:10 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 06:32:10 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 06:32:10 GMT
EXPOSE 80
# Fri, 01 Dec 2023 06:32:11 GMT
EXPOSE 443
# Fri, 01 Dec 2023 06:32:11 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 06:32:11 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 06:32:11 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 06:32:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08886dfc0722c4ed2cb6a70c285a33fe35aec069435868488356dde320b4d21c`  
		Last Modified: Fri, 01 Dec 2023 06:32:30 GMT  
		Size: 350.8 KB (350845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0132c3b72c65b40cace6033d219e1e6d680bb85808270b77a5189c509c10bc0`  
		Last Modified: Fri, 01 Dec 2023 06:32:29 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2ecdf85e2f8f19fc737312e7157f0141b45020324fcf01f4e92bbe707d8983`  
		Last Modified: Fri, 01 Dec 2023 06:32:32 GMT  
		Size: 14.7 MB (14713987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e05dc14b4b6c6dbdcfbdbe28c73e86cafc5287fa13d4f51fdfdfad7b51b8936d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17423853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3acb342ef8cbce6055e45fdabe7e8b60e98cab9d0aa967e362098333633440ff`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:39:01 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 00:39:02 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 00:39:03 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 00:39:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 00:39:05 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 00:39:05 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 00:39:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 00:39:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 00:39:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 80
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 443
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 00:39:06 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 00:39:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc24e4ccf558b6e992efaaa7a735322be11fe99ce19e722eee6ae70bb76515d`  
		Last Modified: Fri, 01 Dec 2023 00:39:21 GMT  
		Size: 347.6 KB (347632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cd6f3873930f7c6aa4ee5d06ef24c77a840fec6f0211e9572fbe0f43c04e1f`  
		Last Modified: Fri, 01 Dec 2023 00:39:21 GMT  
		Size: 7.5 KB (7508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c51a919a8bb024456b258f25a71adb53a14e30c7134e81fac343c44dbf7230c`  
		Last Modified: Fri, 01 Dec 2023 00:39:23 GMT  
		Size: 13.9 MB (13921843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:c3be58f3d1b5614d2a5e7bff50bc07567044bb119ec0f286c94df8169efc313b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17156415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194c773f5747022fdb5fc8d32e8dafcafd61f37e52238ad53627e3309c2fb4cb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:19:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 03:19:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 03:19:15 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 03:19:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 03:19:19 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 03:19:19 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 03:19:20 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 03:19:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 03:19:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 03:19:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 03:19:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 03:19:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 03:19:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 03:19:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 03:19:22 GMT
EXPOSE 80
# Fri, 01 Dec 2023 03:19:22 GMT
EXPOSE 443
# Fri, 01 Dec 2023 03:19:23 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 03:19:23 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 03:19:23 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 03:19:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803b34e1f84b29ca968d2fbf85c278608566c34dfd1742e088c6483685957029`  
		Last Modified: Fri, 01 Dec 2023 03:19:48 GMT  
		Size: 344.5 KB (344464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bbcb291a405e073d645e52039b6f84fa5071645ceb53988f99d384fbc6c4c1`  
		Last Modified: Fri, 01 Dec 2023 03:19:48 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d0aed5710d79e6bba64ce3cf139d40c4e2c3003d1feec3776b18919e3a1423`  
		Last Modified: Fri, 01 Dec 2023 03:19:50 GMT  
		Size: 13.9 MB (13903440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e7f68eb0f76a55ada8be1bb5213e5bbbcb0727fa8d4051f6f3edf1275bc2dc40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17274998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9487e6591f483b0f0d5fe25a89d069485fa10bb97a06ef07085f28b86995977c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:11:08 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 03:11:09 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 03:11:10 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 03:11:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 03:11:11 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 03:11:11 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 80
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 443
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 03:11:12 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 03:11:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e383270d6915b6b427f49a75d657d5a0403fcd47a5f89cd30e85143ca54c22`  
		Last Modified: Fri, 01 Dec 2023 03:11:28 GMT  
		Size: 360.7 KB (360655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27e927f808292c7b306432ed3ee61ecc6b7f637b8ccbdf5cb2d6bdc24649858`  
		Last Modified: Fri, 01 Dec 2023 03:11:28 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dab02cb145c1d5336977666f796446f69abbbfa721ab7a71525867eb3edfbc`  
		Last Modified: Fri, 01 Dec 2023 03:11:30 GMT  
		Size: 13.6 MB (13573804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:3f9f202dc07f3bb097e0e78330d59f52c488ff4ba3b4aa4a569f1a28c9db95f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.1 MB (17058981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:126d26f69982d49f88bac36f166a92d251494018b25e2e255972b98f38f495f8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:42:19 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 05:42:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 05:42:52 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 05:42:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 05:43:00 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 05:43:20 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 05:43:24 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 05:43:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 05:43:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 05:43:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 05:43:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 05:43:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 05:43:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 05:43:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 05:43:45 GMT
EXPOSE 80
# Fri, 01 Dec 2023 05:43:46 GMT
EXPOSE 443
# Fri, 01 Dec 2023 05:43:46 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 05:43:47 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 05:43:48 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 05:43:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce4bc2907f69809c3086f118895d7e5c8683349557239c0ce79dfbda0ce3768`  
		Last Modified: Fri, 01 Dec 2023 05:44:17 GMT  
		Size: 362.2 KB (362185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef8889b660799cb5b3c54f8771b4a37ad12c12f245aa74e4af501a899449137`  
		Last Modified: Fri, 01 Dec 2023 05:44:17 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681f2bb9965ff577316200c634bfb7e7db0d5b2ba971441db97e1405e3c0fc6b`  
		Last Modified: Fri, 01 Dec 2023 05:44:19 GMT  
		Size: 13.3 MB (13340969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:159a339dbc4d0e8279faad422e0a871d82adcc6736b9c4ac4c4b252c3dbee6a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.8 MB (17825031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0c61727c246c9eedd4c40bc927993a89531560cc027902c6f00b8f288f96b77`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:22:31 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 08:22:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 08:22:32 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 08:22:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 08:22:37 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 08:22:37 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 08:22:38 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 08:22:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 80
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 443
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 08:22:38 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 08:22:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20bbe0abb0a3f63718aa78742832077ad86b8ae86d70ce3ebcece342ec022c6`  
		Last Modified: Fri, 01 Dec 2023 08:23:07 GMT  
		Size: 354.9 KB (354948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1497491e477a92a5e82d0d68588396a3414c6e703fdc68c82c768ad6b18b28`  
		Last Modified: Fri, 01 Dec 2023 08:23:07 GMT  
		Size: 7.5 KB (7502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539ac3a1bb2d355499d388b4de966f9148263d5603f2db92aeba42084d02b3cf`  
		Last Modified: Fri, 01 Dec 2023 08:23:09 GMT  
		Size: 14.2 MB (14245127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-builder`

```console
$ docker pull caddy@sha256:dfd9af513214974c6a77e5e89c7cd3c6d2ddddb226bd21f95118958d47c0c537
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.5122; amd64
	-	windows version 10.0.20348.2113; amd64

### `caddy:2.7-builder` - linux; amd64

```console
$ docker pull caddy@sha256:fd75db17630bfaadeef0d2ee65994b5714e8b50b680116e62063b53f58ee8494
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76963250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c15f2632afa610125145b4eeb7cd15cfd6eb2789f9806d851ebe5254b2e0b4aa`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:46:23 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 03:46:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:25:52 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:26:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:26:02 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:26:02 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:26:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:26:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:26:03 GMT
WORKDIR /go
# Tue, 05 Dec 2023 20:48:59 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 20:48:59 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 20:48:59 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 20:48:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 20:48:59 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 20:49:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 20:49:01 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 20:49:01 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501dced60f86be38cc73d3c038f7db4afeee65726f7e422aacf09244539ebf1`  
		Last Modified: Fri, 01 Dec 2023 03:50:39 GMT  
		Size: 284.7 KB (284697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63d189496f5f03c835c9c85df2db6920546d36a1701f6b5ad15f800c671605d`  
		Last Modified: Tue, 05 Dec 2023 20:31:27 GMT  
		Size: 67.0 MB (67003308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aeb88dd0f3e06a57abc08c781b85c89d138194918c469aea9a1bed9753d2ed0`  
		Last Modified: Tue, 05 Dec 2023 20:31:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40ff2505fd8d96e76bddb63b05c2d42815db1dabe0093ec8f8f53be403b0d01`  
		Last Modified: Tue, 05 Dec 2023 20:49:17 GMT  
		Size: 5.0 MB (4970029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3868d63c7cd554f20832e0aff9559fa0cdd7cdbaa4de14e8043fefd0ebfde5`  
		Last Modified: Tue, 05 Dec 2023 20:49:16 GMT  
		Size: 1.3 MB (1302235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a2748825cf9745fffb7f4807c0b6fd474a0221d0d19177142c3f952e10ac78`  
		Last Modified: Tue, 05 Dec 2023 20:49:16 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2c90abb7280a71391618e8552a4faa4e66eb61f80d02402126d25f1365cf063f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75409540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a539589e36806b442a969b2dcf589a62915dde0f6bee440eb73fda5d315a9dd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:53:48 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 00:53:48 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:49:18 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:49:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:49:36 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:49:36 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:49:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:49:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:49:37 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:11:53 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:11:53 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:11:53 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:11:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:11:53 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:11:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:11:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:11:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e7ba0492eb25e7f21078441d7cdc65088836bc1984bc4a14cd3e9cd75cbf32`  
		Last Modified: Fri, 01 Dec 2023 01:00:23 GMT  
		Size: 284.9 KB (284884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de60bcfc919bc6b53554a040a5a58936a8d2e2bf66b2872b69d7a3164e35923f`  
		Last Modified: Tue, 05 Dec 2023 20:54:54 GMT  
		Size: 65.8 MB (65764248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e61f3b09467cb2b97e65a90f25e38cba8acfcd387d168214a949b59bf8c09a`  
		Last Modified: Tue, 05 Dec 2023 20:54:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7827ddd1dfa7654d070274e573dbfcc8fb5ac2ef73888f8b0563e0672811ad`  
		Last Modified: Tue, 05 Dec 2023 21:12:11 GMT  
		Size: 5.0 MB (4964331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f919a9a90cd0240dfd228f8b093cb51b08bf03eabc0326cfe303219b37469f5`  
		Last Modified: Tue, 05 Dec 2023 21:12:11 GMT  
		Size: 1.2 MB (1248647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66464a5ea9ace101c6914e8c5da3a953cb5a9b372ffc562f6a7ab2bcc2b9c0a6`  
		Last Modified: Tue, 05 Dec 2023 21:12:11 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:f65daee5179d36a392c0d931a02c5c400f99b4470bd68e3f326d6828bd8f3fb6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74707169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53077f2480efa131c1c20460899eb69b049d624d249a844e4e1c3bd88aa28d12`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:44:57 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 08:44:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:58:01 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:58:16 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:58:16 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:58:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:58:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:58:17 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:22:31 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:22:31 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:22:31 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:22:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:22:31 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:22:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:22:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:22:32 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a824ff289f1a3c765a444079137b8b7f1cee80348faa53e1ba4c960b73ed2a`  
		Last Modified: Fri, 01 Dec 2023 08:49:42 GMT  
		Size: 284.1 KB (284079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4989177b4ed66b7e9f9e8c4bfce82720b582e24b735d6628effa75d81c5718fc`  
		Last Modified: Tue, 05 Dec 2023 21:04:43 GMT  
		Size: 65.8 MB (65764197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f9b58eae167c54d3faa3eeffd480cdae7e8b4841eb816a86cfdd01f8ae29ef`  
		Last Modified: Tue, 05 Dec 2023 21:04:29 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4cd1a3aab8fc02791b1e19f81b7de1bd691c10a7c942acc7e733221bf12888`  
		Last Modified: Tue, 05 Dec 2023 21:22:47 GMT  
		Size: 4.5 MB (4511237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3a92f0249b45814852e4e987e1a6304bcfb211077150ab43415b31d929f4af`  
		Last Modified: Tue, 05 Dec 2023 21:22:47 GMT  
		Size: 1.2 MB (1246087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3152bffd7f15885d0e72b0adabc22f46542f569db908b69d63eb29addd5e950`  
		Last Modified: Tue, 05 Dec 2023 21:22:47 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:977753f53683eb84ddc7477e5a743e0e1e4e2a001f20edfa0f01d43359d85dc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73981644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0f601640aa519cb421e86cd75a6ad6223541d58cfe80b27b699a23a2585ce70`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:43:53 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 03:18:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:16:18 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:16:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:16:28 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:16:28 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:16:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:16:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:16:28 GMT
WORKDIR /go
# Tue, 05 Dec 2023 20:38:16 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 20:38:16 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 20:38:16 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 20:38:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 20:38:16 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 20:38:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 20:38:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 20:38:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a63ed24dc22a348b35d99b5ec9dc67ff66563b539875e5c8ab2d870b3991ac`  
		Last Modified: Fri, 01 Dec 2023 02:44:03 GMT  
		Size: 286.3 KB (286307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f00641dffc5c2a149049ee9046bb24cfc7de534b7495a0f27784a4fff0fadc`  
		Last Modified: Tue, 05 Dec 2023 20:21:00 GMT  
		Size: 64.1 MB (64094844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452682ba77e89fc55be3a168358f5f43bccad93ecdd3d53b4dec7fff6915128b`  
		Last Modified: Tue, 05 Dec 2023 20:20:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3fe1e12507f8c4a2731393eebfc5ab973aa344b0daceec525560b812b26f60`  
		Last Modified: Tue, 05 Dec 2023 20:38:33 GMT  
		Size: 5.1 MB (5068450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb3c2fad921714e69ace0b18d8f72eb2566d50bc92ff9e9dd125ec383131eb9`  
		Last Modified: Tue, 05 Dec 2023 20:38:32 GMT  
		Size: 1.2 MB (1198449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9c40c8a39fcf5ab6fa64b1c2e1dd5d0b5c1f6b4d9c11ed9481644fe94f1cbf`  
		Last Modified: Tue, 05 Dec 2023 20:38:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:50de875c68ad6aeffc5eb2dd0942d219481fe70c55088657bbe724abd05f7c49
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74206489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7029045647c7331bb58455d58f274c3e4356d86729c097b8d3cfe35717b3b9d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:37:34 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 06:37:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:38:14 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:38:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:38:37 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:38:38 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:38:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:38:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:38:41 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:04:33 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:04:34 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:04:35 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:04:35 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:04:35 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:04:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:04:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:04:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692dbecd5e141c462ab06ef113ec964b525e7564d734890cc1d5b1dbf33ee34e`  
		Last Modified: Fri, 01 Dec 2023 06:43:30 GMT  
		Size: 286.7 KB (286661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc89a0f2d97ecfd4d20235e72227fc24aa79a64509fe9ea64702db658f2ad26d`  
		Last Modified: Tue, 05 Dec 2023 20:46:23 GMT  
		Size: 64.1 MB (64115804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d76f2c2e2bbb4190b1865ddafdc8cb88adee4c79d7d5ba23e69696e9610889`  
		Last Modified: Tue, 05 Dec 2023 20:46:11 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e0ec0f713ee657d6aa159fab65c05939480b5ca50a8e3dc4b1a9a6578160f7`  
		Last Modified: Tue, 05 Dec 2023 21:04:57 GMT  
		Size: 5.3 MB (5268970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e164016cca4964643911960baccae8beaa47cc5086bbe3ebfd14183d5204a8`  
		Last Modified: Tue, 05 Dec 2023 21:04:56 GMT  
		Size: 1.2 MB (1186171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2932f0ef681ac7135c1e7ff9332dd4c154c1f793d04fda438db30a1573bacc8b`  
		Last Modified: Tue, 05 Dec 2023 21:04:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; s390x

```console
$ docker pull caddy@sha256:98d5d7af77acd9cc1b74499ba61056fb599a17742331f51a0fffa89ef56bb114
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76098838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d4f342a39bbb58bda0421e578348bf6d047bf7125db5c42216b2ba9b6d5040d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:14:49 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 08:14:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:44:16 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:44:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:45:03 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:45:04 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:45:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:45:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:45:05 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:14:29 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:14:29 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:14:29 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:14:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:14:30 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:14:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:14:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:14:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab563e8d41683e124df048aa9b564b0e8e1021e85213666971a015df51d5e48`  
		Last Modified: Fri, 01 Dec 2023 08:20:46 GMT  
		Size: 285.1 KB (285090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d44aea4caa072a45cb44ab86f401c76153b599207fb3cc311f44308e9b5da13`  
		Last Modified: Tue, 05 Dec 2023 20:57:00 GMT  
		Size: 66.2 MB (66218626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef66858f73257b9fd43395b7e2758cdaa72267303442d3a5dbef122796530c5`  
		Last Modified: Tue, 05 Dec 2023 20:56:49 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5261478888d8f0caaf878da0629c62f928bbbff35e7f873c1a463c6e39c0bd37`  
		Last Modified: Tue, 05 Dec 2023 21:14:53 GMT  
		Size: 5.1 MB (5114717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade58cb7b8ea422e0ab68cb58091d9adc84172a8de51990bb80269c07c5bd556`  
		Last Modified: Tue, 05 Dec 2023 21:14:53 GMT  
		Size: 1.3 MB (1262391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7f47ab035030fe8af075c6b5ebf045cd6bd32bef0700d8cc656ba7204685b7`  
		Last Modified: Tue, 05 Dec 2023 21:14:52 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:a4a6967f69e81e55f736b4e5d91bab0e44ce577821e0336b8b8ef7456679e1c1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2154296990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14a551f4e77e9632ddd054915a37f355befe0b5201417194368482bc6a54949d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 02:47:03 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Nov 2023 02:47:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Nov 2023 02:47:05 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Nov 2023 02:47:06 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Nov 2023 02:48:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:48:31 GMT
ENV GOPATH=C:\go
# Thu, 16 Nov 2023 02:49:41 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 05 Dec 2023 20:18:04 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:21:11 GMT
RUN $url = 'https://dl.google.com/go/go1.21.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'bbe603cde7c9dee658f45164b4d06de1eff6e6e6b800100824e7c00d56a9a92f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 05 Dec 2023 20:21:13 GMT
WORKDIR C:\go
# Tue, 05 Dec 2023 20:59:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 05 Dec 2023 20:59:30 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 20:59:31 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 20:59:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:00:49 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 05 Dec 2023 21:00:50 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e901367fac1450f509d3118ada9e004e3613844ebdf91861147a093483930a4`  
		Last Modified: Thu, 16 Nov 2023 03:11:57 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e08004205bd077d8f22b013c70dc2f10796c64fced1eb9927e0055daff2d05d`  
		Last Modified: Thu, 16 Nov 2023 03:11:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebc5048afc68ef48e2f2136545e2cccf26bb29eb4926bf4259b370ad55b4e7a`  
		Last Modified: Thu, 16 Nov 2023 03:11:55 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f50fe5c7ef21648f3eaa4304932877a116fcb910b8e9095c779a2fbe6d57f7e`  
		Last Modified: Thu, 16 Nov 2023 03:11:55 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76fe0e37750041d4ede2a0ca3b5245cfe075c3eb2ee27d7ce72ee8c3d7b20cc`  
		Last Modified: Thu, 16 Nov 2023 03:12:00 GMT  
		Size: 25.5 MB (25537512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8097bb9b8778d15dbf89d899653bf1634ec17554e5d84ef1ccfcac8ebf86afe2`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b542d31e914d67da86cc5701cdc282ab664dc1170507e3802e22ab3026436a90`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 263.2 KB (263200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86acdf7d3955fb44136bac433a30ccbbb97863120f270af32659dd65446666c7`  
		Last Modified: Tue, 05 Dec 2023 20:39:22 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1abe126c354944b7db8aa724d8f757167f7c3b36d39f976ef3b1b0d1b1b65ab`  
		Last Modified: Tue, 05 Dec 2023 20:39:41 GMT  
		Size: 69.4 MB (69361283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6338af096e09067ad482a0f4a6df1d1eee5b5595a64ca5f367b94ce27903e284`  
		Last Modified: Tue, 05 Dec 2023 20:39:22 GMT  
		Size: 1.5 KB (1529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0adc218b27ef5639384c060fb663de3bd74374279d3fd525aa281f63a754779`  
		Last Modified: Tue, 05 Dec 2023 21:02:06 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c21053b248805df7ad888734f5cd1df5a6b426111512d5a6b7530060e7f30b2`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57f384772c293e1d97326febf9e29d6bfef6eb9da2b053b6ad1e0ebea539508`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a2cba3fcdba1e3612614837be0fed9e3b7670483867a14203a15d395aa4179`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b447549db21db40db8a08cddb7d529bbd6e183aba676f13e2a3a5ff034fb67f8`  
		Last Modified: Tue, 05 Dec 2023 21:02:04 GMT  
		Size: 1.7 MB (1685436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408a12340d35fbfeee8cc5bdec3421ede796686f2b22d693863de08da6d51c91`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:081774d66d26fdb1b8b89fc90aeb9a72c559c0690770f153fa4ca3f1d5450e43
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1983623458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af2bcbcbf997ed6d0e17a2acebd1f65d19dbb6868d0523c306342bcc37644dd6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 09 Nov 2023 06:47:20 GMT
RUN Install update 10.0.20348.2113
# Thu, 16 Nov 2023 01:36:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 02:43:34 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Nov 2023 02:43:35 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Nov 2023 02:43:36 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Nov 2023 02:43:37 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Nov 2023 02:44:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:44:11 GMT
ENV GOPATH=C:\go
# Thu, 16 Nov 2023 02:44:30 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 05 Dec 2023 20:15:35 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:17:49 GMT
RUN $url = 'https://dl.google.com/go/go1.21.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'bbe603cde7c9dee658f45164b4d06de1eff6e6e6b800100824e7c00d56a9a92f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 05 Dec 2023 20:17:50 GMT
WORKDIR C:\go
# Tue, 05 Dec 2023 21:00:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 05 Dec 2023 21:00:58 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:00:59 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:01:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:01:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 05 Dec 2023 21:01:26 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7989ef2c4cfb06d845746a3c3660481ea84d3f5c8216041855ce528f0ac4015c`  
		Last Modified: Tue, 14 Nov 2023 20:43:13 GMT  
		Size: 498.2 MB (498182566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbeb193d02c2ca7f9a9ea438fbf1bcdb6ea4a6fea626713330fd1ebb514424f`  
		Last Modified: Thu, 16 Nov 2023 02:25:14 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b1d4a557f047b695f94452d9707061981d7fae4239c674b332282b8291963c`  
		Last Modified: Thu, 16 Nov 2023 03:11:20 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45549c207f14d769cba7c36b66157ec213bbc32ce57d685d8e2c407cf3987bb`  
		Last Modified: Thu, 16 Nov 2023 03:11:18 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c674717e06bf8cb25d5887393ef9568ee0ab6390966b9666808e836e9bd471d`  
		Last Modified: Thu, 16 Nov 2023 03:11:18 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2227badcd9f5f2b70b3d2ffd1c18887498f413c07802bfb334e8dc7b2d2acc`  
		Last Modified: Thu, 16 Nov 2023 03:11:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9f3b5e90a2e6028cf194e870b24a7158f875f18b81f4f9137a5db3ea1f79ac`  
		Last Modified: Thu, 16 Nov 2023 03:11:23 GMT  
		Size: 25.5 MB (25536225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7811a5416dcd19193a5b3ab9327607bf845f7ff77f95d3e20abdfb7435c32ae0`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5931209e960a94616639ea72e4d3ad9dc9cb554790ce930152c73bdc1449c034`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 266.6 KB (266600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a70f603a2fb4e76edd3165b62a179fb8f6410e265f5ae4a3732ee68e610034b`  
		Last Modified: Tue, 05 Dec 2023 20:38:48 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e37840dec3a6665ce48520be8b2c51b654359765bee5ab0780ee74746f0eb2`  
		Last Modified: Tue, 05 Dec 2023 20:39:08 GMT  
		Size: 69.3 MB (69342960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d16ae54757acda093616d24735d4c92d4676649bec49807fc35de90d15e15c`  
		Last Modified: Tue, 05 Dec 2023 20:38:48 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5744d01eddd2ef9d9673fdb0f0e48203fad1b01f2b14899a3ec6393c4548e75`  
		Last Modified: Tue, 05 Dec 2023 21:02:23 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35bb848667aa413b6ce6c309a4c2169635b0740dc335b9b39413a00627c01ab`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78369d5e83dd4f4ca5558a32848f3515e191b15f8427ea166a4f6327694ff9db`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2ae381a5e49194e43b26ac8036b1da5d2af930f7516796c476bcdb9c8125e3`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09db71960c4c717ed44d2694cf77f248223822e163297046010868c3ebf0767`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.7 MB (1677926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9dfae036c2fe0cfcd2e4f5a9acc265c45af769542844b9b617b62ec3ebd591`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-builder-alpine`

```console
$ docker pull caddy@sha256:3e0232193d2e16a551210bb7cf4da86b6d0bf45cb70508c343c680065d7c440e
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
$ docker pull caddy@sha256:fd75db17630bfaadeef0d2ee65994b5714e8b50b680116e62063b53f58ee8494
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76963250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c15f2632afa610125145b4eeb7cd15cfd6eb2789f9806d851ebe5254b2e0b4aa`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:46:23 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 03:46:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:25:52 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:26:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:26:02 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:26:02 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:26:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:26:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:26:03 GMT
WORKDIR /go
# Tue, 05 Dec 2023 20:48:59 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 20:48:59 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 20:48:59 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 20:48:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 20:48:59 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 20:49:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 20:49:01 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 20:49:01 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501dced60f86be38cc73d3c038f7db4afeee65726f7e422aacf09244539ebf1`  
		Last Modified: Fri, 01 Dec 2023 03:50:39 GMT  
		Size: 284.7 KB (284697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63d189496f5f03c835c9c85df2db6920546d36a1701f6b5ad15f800c671605d`  
		Last Modified: Tue, 05 Dec 2023 20:31:27 GMT  
		Size: 67.0 MB (67003308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aeb88dd0f3e06a57abc08c781b85c89d138194918c469aea9a1bed9753d2ed0`  
		Last Modified: Tue, 05 Dec 2023 20:31:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40ff2505fd8d96e76bddb63b05c2d42815db1dabe0093ec8f8f53be403b0d01`  
		Last Modified: Tue, 05 Dec 2023 20:49:17 GMT  
		Size: 5.0 MB (4970029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3868d63c7cd554f20832e0aff9559fa0cdd7cdbaa4de14e8043fefd0ebfde5`  
		Last Modified: Tue, 05 Dec 2023 20:49:16 GMT  
		Size: 1.3 MB (1302235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a2748825cf9745fffb7f4807c0b6fd474a0221d0d19177142c3f952e10ac78`  
		Last Modified: Tue, 05 Dec 2023 20:49:16 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2c90abb7280a71391618e8552a4faa4e66eb61f80d02402126d25f1365cf063f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75409540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a539589e36806b442a969b2dcf589a62915dde0f6bee440eb73fda5d315a9dd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:53:48 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 00:53:48 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:49:18 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:49:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:49:36 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:49:36 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:49:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:49:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:49:37 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:11:53 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:11:53 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:11:53 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:11:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:11:53 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:11:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:11:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:11:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e7ba0492eb25e7f21078441d7cdc65088836bc1984bc4a14cd3e9cd75cbf32`  
		Last Modified: Fri, 01 Dec 2023 01:00:23 GMT  
		Size: 284.9 KB (284884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de60bcfc919bc6b53554a040a5a58936a8d2e2bf66b2872b69d7a3164e35923f`  
		Last Modified: Tue, 05 Dec 2023 20:54:54 GMT  
		Size: 65.8 MB (65764248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e61f3b09467cb2b97e65a90f25e38cba8acfcd387d168214a949b59bf8c09a`  
		Last Modified: Tue, 05 Dec 2023 20:54:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7827ddd1dfa7654d070274e573dbfcc8fb5ac2ef73888f8b0563e0672811ad`  
		Last Modified: Tue, 05 Dec 2023 21:12:11 GMT  
		Size: 5.0 MB (4964331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f919a9a90cd0240dfd228f8b093cb51b08bf03eabc0326cfe303219b37469f5`  
		Last Modified: Tue, 05 Dec 2023 21:12:11 GMT  
		Size: 1.2 MB (1248647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66464a5ea9ace101c6914e8c5da3a953cb5a9b372ffc562f6a7ab2bcc2b9c0a6`  
		Last Modified: Tue, 05 Dec 2023 21:12:11 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:f65daee5179d36a392c0d931a02c5c400f99b4470bd68e3f326d6828bd8f3fb6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74707169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53077f2480efa131c1c20460899eb69b049d624d249a844e4e1c3bd88aa28d12`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:44:57 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 08:44:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:58:01 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:58:16 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:58:16 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:58:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:58:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:58:17 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:22:31 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:22:31 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:22:31 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:22:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:22:31 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:22:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:22:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:22:32 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a824ff289f1a3c765a444079137b8b7f1cee80348faa53e1ba4c960b73ed2a`  
		Last Modified: Fri, 01 Dec 2023 08:49:42 GMT  
		Size: 284.1 KB (284079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4989177b4ed66b7e9f9e8c4bfce82720b582e24b735d6628effa75d81c5718fc`  
		Last Modified: Tue, 05 Dec 2023 21:04:43 GMT  
		Size: 65.8 MB (65764197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f9b58eae167c54d3faa3eeffd480cdae7e8b4841eb816a86cfdd01f8ae29ef`  
		Last Modified: Tue, 05 Dec 2023 21:04:29 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4cd1a3aab8fc02791b1e19f81b7de1bd691c10a7c942acc7e733221bf12888`  
		Last Modified: Tue, 05 Dec 2023 21:22:47 GMT  
		Size: 4.5 MB (4511237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3a92f0249b45814852e4e987e1a6304bcfb211077150ab43415b31d929f4af`  
		Last Modified: Tue, 05 Dec 2023 21:22:47 GMT  
		Size: 1.2 MB (1246087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3152bffd7f15885d0e72b0adabc22f46542f569db908b69d63eb29addd5e950`  
		Last Modified: Tue, 05 Dec 2023 21:22:47 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:977753f53683eb84ddc7477e5a743e0e1e4e2a001f20edfa0f01d43359d85dc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73981644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0f601640aa519cb421e86cd75a6ad6223541d58cfe80b27b699a23a2585ce70`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:43:53 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 03:18:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:16:18 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:16:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:16:28 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:16:28 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:16:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:16:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:16:28 GMT
WORKDIR /go
# Tue, 05 Dec 2023 20:38:16 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 20:38:16 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 20:38:16 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 20:38:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 20:38:16 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 20:38:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 20:38:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 20:38:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a63ed24dc22a348b35d99b5ec9dc67ff66563b539875e5c8ab2d870b3991ac`  
		Last Modified: Fri, 01 Dec 2023 02:44:03 GMT  
		Size: 286.3 KB (286307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f00641dffc5c2a149049ee9046bb24cfc7de534b7495a0f27784a4fff0fadc`  
		Last Modified: Tue, 05 Dec 2023 20:21:00 GMT  
		Size: 64.1 MB (64094844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452682ba77e89fc55be3a168358f5f43bccad93ecdd3d53b4dec7fff6915128b`  
		Last Modified: Tue, 05 Dec 2023 20:20:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3fe1e12507f8c4a2731393eebfc5ab973aa344b0daceec525560b812b26f60`  
		Last Modified: Tue, 05 Dec 2023 20:38:33 GMT  
		Size: 5.1 MB (5068450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb3c2fad921714e69ace0b18d8f72eb2566d50bc92ff9e9dd125ec383131eb9`  
		Last Modified: Tue, 05 Dec 2023 20:38:32 GMT  
		Size: 1.2 MB (1198449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9c40c8a39fcf5ab6fa64b1c2e1dd5d0b5c1f6b4d9c11ed9481644fe94f1cbf`  
		Last Modified: Tue, 05 Dec 2023 20:38:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:50de875c68ad6aeffc5eb2dd0942d219481fe70c55088657bbe724abd05f7c49
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74206489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7029045647c7331bb58455d58f274c3e4356d86729c097b8d3cfe35717b3b9d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:37:34 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 06:37:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:38:14 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:38:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:38:37 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:38:38 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:38:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:38:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:38:41 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:04:33 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:04:34 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:04:35 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:04:35 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:04:35 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:04:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:04:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:04:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692dbecd5e141c462ab06ef113ec964b525e7564d734890cc1d5b1dbf33ee34e`  
		Last Modified: Fri, 01 Dec 2023 06:43:30 GMT  
		Size: 286.7 KB (286661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc89a0f2d97ecfd4d20235e72227fc24aa79a64509fe9ea64702db658f2ad26d`  
		Last Modified: Tue, 05 Dec 2023 20:46:23 GMT  
		Size: 64.1 MB (64115804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d76f2c2e2bbb4190b1865ddafdc8cb88adee4c79d7d5ba23e69696e9610889`  
		Last Modified: Tue, 05 Dec 2023 20:46:11 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e0ec0f713ee657d6aa159fab65c05939480b5ca50a8e3dc4b1a9a6578160f7`  
		Last Modified: Tue, 05 Dec 2023 21:04:57 GMT  
		Size: 5.3 MB (5268970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e164016cca4964643911960baccae8beaa47cc5086bbe3ebfd14183d5204a8`  
		Last Modified: Tue, 05 Dec 2023 21:04:56 GMT  
		Size: 1.2 MB (1186171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2932f0ef681ac7135c1e7ff9332dd4c154c1f793d04fda438db30a1573bacc8b`  
		Last Modified: Tue, 05 Dec 2023 21:04:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:98d5d7af77acd9cc1b74499ba61056fb599a17742331f51a0fffa89ef56bb114
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76098838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d4f342a39bbb58bda0421e578348bf6d047bf7125db5c42216b2ba9b6d5040d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:14:49 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 08:14:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:44:16 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:44:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:45:03 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:45:04 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:45:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:45:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:45:05 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:14:29 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:14:29 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:14:29 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:14:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:14:30 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:14:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:14:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:14:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab563e8d41683e124df048aa9b564b0e8e1021e85213666971a015df51d5e48`  
		Last Modified: Fri, 01 Dec 2023 08:20:46 GMT  
		Size: 285.1 KB (285090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d44aea4caa072a45cb44ab86f401c76153b599207fb3cc311f44308e9b5da13`  
		Last Modified: Tue, 05 Dec 2023 20:57:00 GMT  
		Size: 66.2 MB (66218626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef66858f73257b9fd43395b7e2758cdaa72267303442d3a5dbef122796530c5`  
		Last Modified: Tue, 05 Dec 2023 20:56:49 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5261478888d8f0caaf878da0629c62f928bbbff35e7f873c1a463c6e39c0bd37`  
		Last Modified: Tue, 05 Dec 2023 21:14:53 GMT  
		Size: 5.1 MB (5114717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade58cb7b8ea422e0ab68cb58091d9adc84172a8de51990bb80269c07c5bd556`  
		Last Modified: Tue, 05 Dec 2023 21:14:53 GMT  
		Size: 1.3 MB (1262391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7f47ab035030fe8af075c6b5ebf045cd6bd32bef0700d8cc656ba7204685b7`  
		Last Modified: Tue, 05 Dec 2023 21:14:52 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:9a3cb11cfc419a512a550298d752bbf00ea5dc0b4daa8993ab10db26d145fda9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `caddy:2.7-builder-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:a4a6967f69e81e55f736b4e5d91bab0e44ce577821e0336b8b8ef7456679e1c1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2154296990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14a551f4e77e9632ddd054915a37f355befe0b5201417194368482bc6a54949d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 02:47:03 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Nov 2023 02:47:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Nov 2023 02:47:05 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Nov 2023 02:47:06 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Nov 2023 02:48:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:48:31 GMT
ENV GOPATH=C:\go
# Thu, 16 Nov 2023 02:49:41 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 05 Dec 2023 20:18:04 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:21:11 GMT
RUN $url = 'https://dl.google.com/go/go1.21.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'bbe603cde7c9dee658f45164b4d06de1eff6e6e6b800100824e7c00d56a9a92f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 05 Dec 2023 20:21:13 GMT
WORKDIR C:\go
# Tue, 05 Dec 2023 20:59:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 05 Dec 2023 20:59:30 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 20:59:31 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 20:59:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:00:49 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 05 Dec 2023 21:00:50 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e901367fac1450f509d3118ada9e004e3613844ebdf91861147a093483930a4`  
		Last Modified: Thu, 16 Nov 2023 03:11:57 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e08004205bd077d8f22b013c70dc2f10796c64fced1eb9927e0055daff2d05d`  
		Last Modified: Thu, 16 Nov 2023 03:11:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebc5048afc68ef48e2f2136545e2cccf26bb29eb4926bf4259b370ad55b4e7a`  
		Last Modified: Thu, 16 Nov 2023 03:11:55 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f50fe5c7ef21648f3eaa4304932877a116fcb910b8e9095c779a2fbe6d57f7e`  
		Last Modified: Thu, 16 Nov 2023 03:11:55 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76fe0e37750041d4ede2a0ca3b5245cfe075c3eb2ee27d7ce72ee8c3d7b20cc`  
		Last Modified: Thu, 16 Nov 2023 03:12:00 GMT  
		Size: 25.5 MB (25537512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8097bb9b8778d15dbf89d899653bf1634ec17554e5d84ef1ccfcac8ebf86afe2`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b542d31e914d67da86cc5701cdc282ab664dc1170507e3802e22ab3026436a90`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 263.2 KB (263200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86acdf7d3955fb44136bac433a30ccbbb97863120f270af32659dd65446666c7`  
		Last Modified: Tue, 05 Dec 2023 20:39:22 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1abe126c354944b7db8aa724d8f757167f7c3b36d39f976ef3b1b0d1b1b65ab`  
		Last Modified: Tue, 05 Dec 2023 20:39:41 GMT  
		Size: 69.4 MB (69361283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6338af096e09067ad482a0f4a6df1d1eee5b5595a64ca5f367b94ce27903e284`  
		Last Modified: Tue, 05 Dec 2023 20:39:22 GMT  
		Size: 1.5 KB (1529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0adc218b27ef5639384c060fb663de3bd74374279d3fd525aa281f63a754779`  
		Last Modified: Tue, 05 Dec 2023 21:02:06 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c21053b248805df7ad888734f5cd1df5a6b426111512d5a6b7530060e7f30b2`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57f384772c293e1d97326febf9e29d6bfef6eb9da2b053b6ad1e0ebea539508`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a2cba3fcdba1e3612614837be0fed9e3b7670483867a14203a15d395aa4179`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b447549db21db40db8a08cddb7d529bbd6e183aba676f13e2a3a5ff034fb67f8`  
		Last Modified: Tue, 05 Dec 2023 21:02:04 GMT  
		Size: 1.7 MB (1685436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408a12340d35fbfeee8cc5bdec3421ede796686f2b22d693863de08da6d51c91`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:b98db9d0f32752a5a646d4009012af66a84d26002c3605d6fe3da6769aede98d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2113; amd64

### `caddy:2.7-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:081774d66d26fdb1b8b89fc90aeb9a72c559c0690770f153fa4ca3f1d5450e43
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1983623458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af2bcbcbf997ed6d0e17a2acebd1f65d19dbb6868d0523c306342bcc37644dd6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 09 Nov 2023 06:47:20 GMT
RUN Install update 10.0.20348.2113
# Thu, 16 Nov 2023 01:36:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 02:43:34 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Nov 2023 02:43:35 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Nov 2023 02:43:36 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Nov 2023 02:43:37 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Nov 2023 02:44:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:44:11 GMT
ENV GOPATH=C:\go
# Thu, 16 Nov 2023 02:44:30 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 05 Dec 2023 20:15:35 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:17:49 GMT
RUN $url = 'https://dl.google.com/go/go1.21.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'bbe603cde7c9dee658f45164b4d06de1eff6e6e6b800100824e7c00d56a9a92f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 05 Dec 2023 20:17:50 GMT
WORKDIR C:\go
# Tue, 05 Dec 2023 21:00:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 05 Dec 2023 21:00:58 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:00:59 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:01:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:01:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 05 Dec 2023 21:01:26 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7989ef2c4cfb06d845746a3c3660481ea84d3f5c8216041855ce528f0ac4015c`  
		Last Modified: Tue, 14 Nov 2023 20:43:13 GMT  
		Size: 498.2 MB (498182566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbeb193d02c2ca7f9a9ea438fbf1bcdb6ea4a6fea626713330fd1ebb514424f`  
		Last Modified: Thu, 16 Nov 2023 02:25:14 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b1d4a557f047b695f94452d9707061981d7fae4239c674b332282b8291963c`  
		Last Modified: Thu, 16 Nov 2023 03:11:20 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45549c207f14d769cba7c36b66157ec213bbc32ce57d685d8e2c407cf3987bb`  
		Last Modified: Thu, 16 Nov 2023 03:11:18 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c674717e06bf8cb25d5887393ef9568ee0ab6390966b9666808e836e9bd471d`  
		Last Modified: Thu, 16 Nov 2023 03:11:18 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2227badcd9f5f2b70b3d2ffd1c18887498f413c07802bfb334e8dc7b2d2acc`  
		Last Modified: Thu, 16 Nov 2023 03:11:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9f3b5e90a2e6028cf194e870b24a7158f875f18b81f4f9137a5db3ea1f79ac`  
		Last Modified: Thu, 16 Nov 2023 03:11:23 GMT  
		Size: 25.5 MB (25536225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7811a5416dcd19193a5b3ab9327607bf845f7ff77f95d3e20abdfb7435c32ae0`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5931209e960a94616639ea72e4d3ad9dc9cb554790ce930152c73bdc1449c034`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 266.6 KB (266600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a70f603a2fb4e76edd3165b62a179fb8f6410e265f5ae4a3732ee68e610034b`  
		Last Modified: Tue, 05 Dec 2023 20:38:48 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e37840dec3a6665ce48520be8b2c51b654359765bee5ab0780ee74746f0eb2`  
		Last Modified: Tue, 05 Dec 2023 20:39:08 GMT  
		Size: 69.3 MB (69342960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d16ae54757acda093616d24735d4c92d4676649bec49807fc35de90d15e15c`  
		Last Modified: Tue, 05 Dec 2023 20:38:48 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5744d01eddd2ef9d9673fdb0f0e48203fad1b01f2b14899a3ec6393c4548e75`  
		Last Modified: Tue, 05 Dec 2023 21:02:23 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35bb848667aa413b6ce6c309a4c2169635b0740dc335b9b39413a00627c01ab`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78369d5e83dd4f4ca5558a32848f3515e191b15f8427ea166a4f6327694ff9db`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2ae381a5e49194e43b26ac8036b1da5d2af930f7516796c476bcdb9c8125e3`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09db71960c4c717ed44d2694cf77f248223822e163297046010868c3ebf0767`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.7 MB (1677926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9dfae036c2fe0cfcd2e4f5a9acc265c45af769542844b9b617b62ec3ebd591`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-windowsservercore`

```console
$ docker pull caddy@sha256:b2a860f9d095b10b5613cfd76162decff7840f5881e3c5ecf4e01d29d829c405
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.5122; amd64
	-	windows version 10.0.20348.2113; amd64

### `caddy:2.7-windowsservercore` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:38df49f40c98b8d866440b7fec4635fcf669f4c138fd001b95f457b42e4e2265
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2073433228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7105669fddc0d611982501b46d56df54a820ca14cd7e3a3c62c02ef1bd40fc2e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:30:07 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Nov 2023 05:30:07 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:31:22 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Nov 2023 05:31:23 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Nov 2023 05:31:24 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Nov 2023 05:31:25 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 16 Nov 2023 05:31:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Nov 2023 05:31:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Nov 2023 05:31:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Nov 2023 05:31:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Nov 2023 05:31:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Nov 2023 05:31:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Nov 2023 05:31:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Nov 2023 05:31:32 GMT
EXPOSE 80
# Thu, 16 Nov 2023 05:31:33 GMT
EXPOSE 443
# Thu, 16 Nov 2023 05:31:34 GMT
EXPOSE 443/udp
# Thu, 16 Nov 2023 05:31:35 GMT
EXPOSE 2019
# Thu, 16 Nov 2023 05:32:33 GMT
RUN caddy version
# Thu, 16 Nov 2023 05:32:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d66ae500a331057bbb6b25a0c0e5718f2491209d7330f70b1203472b199bd5b`  
		Last Modified: Thu, 16 Nov 2023 05:37:31 GMT  
		Size: 451.2 KB (451175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec48b5261067a4b4643799633487cce5b6ee11cce36314b8a6b22964fd46ba4`  
		Last Modified: Thu, 16 Nov 2023 05:37:30 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bc40730815ee35e950756a15aa93561edd0f272d34d30de69bb8d7f58b1d8e`  
		Last Modified: Thu, 16 Nov 2023 05:37:34 GMT  
		Size: 15.3 MB (15273771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfce8b69f4cadeeaa9fcc771a3a5b374fc4a3c8c41c1a42a7878c1cad861645c`  
		Last Modified: Thu, 16 Nov 2023 05:37:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdd09852c86166de537f8b5f5b78eca092cfb95e9e2e1194c84a7a05334e5c4`  
		Last Modified: Thu, 16 Nov 2023 05:37:29 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f15c2b10239537d18dc39c5208acb0c8fc7bc25d6cd95cb59ed8e8aaf8b73be`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa35da536891cce8df35bca524d15b1b7465d4fc14354a1a15a2fa39d71a4a88`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654652f0bb6c82a0e1fd51010fd587112527866df3c9748cf9ed4414e70ee612`  
		Last Modified: Thu, 16 Nov 2023 05:37:29 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0fcd5cbdfe3f968d65ba5dcece2d017de82a3a4ec737745bd5560697735689`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9396734c66d2d27545fdeb2c33a462651a3807dfcbd04b590a01ace722161a21`  
		Last Modified: Thu, 16 Nov 2023 05:37:27 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a14586579bd1d9d9a9162b0678a119c826a7be5039b5419e90b82c772b33677`  
		Last Modified: Thu, 16 Nov 2023 05:37:27 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c773c8968545d0fca628d03a3b588ca4798423090cadd666d023cee5065235a5`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce86207f89519b9df4526afc22e743fef4a6266614fb8e082e975bf0f01862f`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7392ec7da7419f69c0413116467249934c403f42b53ff6090608481e1ba7985a`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73d1eee374e37176384bade9abdbe65d5aed23b976c507b3b88b17c758761f`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d556f28b534238f3c8497a928caa36428f1d333a69cabf15b4fc3d80aa7f3f9f`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd0eba7ede6da63115506e40bf2b6990915e5fba916e919c6525f447018bbd9`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf5b269f798b76bfba9ad2e27b5aab7bebe448007c818230643c16d6cf761af`  
		Last Modified: Thu, 16 Nov 2023 05:37:25 GMT  
		Size: 252.7 KB (252713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c70c9a3deaf4a41d4192a9248f3fd5ccfadb54792687f31f63a17f46e5134c`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-windowsservercore` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:7a86ad9fb59b43cc97f50c3516b4153bb228276c026e4c802c4a213b0fe1c20f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1902803411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03625f7f4ec599de5399e0e9d5f36d3c2052adeb06f8349ef7a96e3777ddf4e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 09 Nov 2023 06:47:20 GMT
RUN Install update 10.0.20348.2113
# Thu, 16 Nov 2023 01:36:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:33:15 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Nov 2023 05:33:16 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:33:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Nov 2023 05:33:45 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Nov 2023 05:33:46 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Nov 2023 05:33:47 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 16 Nov 2023 05:33:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Nov 2023 05:33:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Nov 2023 05:33:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Nov 2023 05:33:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Nov 2023 05:33:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Nov 2023 05:33:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Nov 2023 05:33:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Nov 2023 05:33:54 GMT
EXPOSE 80
# Thu, 16 Nov 2023 05:33:55 GMT
EXPOSE 443
# Thu, 16 Nov 2023 05:33:56 GMT
EXPOSE 443/udp
# Thu, 16 Nov 2023 05:33:57 GMT
EXPOSE 2019
# Thu, 16 Nov 2023 05:34:33 GMT
RUN caddy version
# Thu, 16 Nov 2023 05:34:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7989ef2c4cfb06d845746a3c3660481ea84d3f5c8216041855ce528f0ac4015c`  
		Last Modified: Tue, 14 Nov 2023 20:43:13 GMT  
		Size: 498.2 MB (498182566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbeb193d02c2ca7f9a9ea438fbf1bcdb6ea4a6fea626713330fd1ebb514424f`  
		Last Modified: Thu, 16 Nov 2023 02:25:14 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b269b5ac8d8c6baa501ca9b38fa715170022416aa7332a2d155a06529882b84a`  
		Last Modified: Thu, 16 Nov 2023 05:37:59 GMT  
		Size: 458.2 KB (458201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f982a236809063ef75b5db6a226207448d936d7791ede196115611649805c5`  
		Last Modified: Thu, 16 Nov 2023 05:37:58 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2783cb5dad5df996a48a9ebf989a6136c91f524f421bfff9e71ab764da46fd04`  
		Last Modified: Thu, 16 Nov 2023 05:38:01 GMT  
		Size: 15.3 MB (15269735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa26255a8f194a0aa31a8fd0c48e7dfba117358880abeaf7ad3c5f54a6be87d`  
		Last Modified: Thu, 16 Nov 2023 05:37:57 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706b8120af6e900b1d0dea48743c4fd50b63c785dbe02b5ccd4af53e68ebefff`  
		Last Modified: Thu, 16 Nov 2023 05:37:57 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c12376eb1027b4892f92b1b8dd45b1e05d78f365c2886ded9202ffbaab80e9`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a29b9f98e523c3477366f98e560b8638fb5c3f0a7a8c76c9a417a33b4d44804`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a9a2fb5b49cb3e38b64f06a755f57ec37b8b5eaf2152fe9e38ae9c8cb3b593`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53a0ea77b4fcc256276d31401de856267c72aeac7fefeeb6fbe655340bb4cf4`  
		Last Modified: Thu, 16 Nov 2023 05:37:55 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d80b783b85d05309ef9fe97740b873bd9092c13b53eea3d83adf6197cbe798`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9454c6602eef29f64927e75d96b8f26d7cf0c6c089afa91e260207675216501`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f23d9fc021e786b83141dd57c2a10dc279d17eacad254ec81d7922372d17876`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55a4267cea49483a79cbee8908d3daf6af4fb6fa1af94e350072034f128c5a1`  
		Last Modified: Thu, 16 Nov 2023 05:37:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9723590c56e28022e6ee055495ee5826c7ea085d2a8b7255d471b35bb27e9a6c`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b39c632f1f53a232721260e3ebcc755559883edb0272949f2d965799d62ef5`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3deb93ce29c0157e6c6b82bbad0ffb2102a833ea54672c93c05843899eac3bc`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09fe12ffad65804e54e566d7b3256d98268c5e943a40282d44bab50d3fb6a04`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517e7fd42cd9750ca7ef5a68df02e2bdc3be404dbd69681f36c7b0acb1562550`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 270.1 KB (270069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0727df29cc57ce0bb7db3c73852d6eaceb439603493f2e3ceb07ce2f8e8e4e99`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-windowsservercore-1809`

```console
$ docker pull caddy@sha256:2e8fbf0e299d85c14b2ac578c2ff6ee6f32e2e0c7dbd4afd5f683286575971d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `caddy:2.7-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:38df49f40c98b8d866440b7fec4635fcf669f4c138fd001b95f457b42e4e2265
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2073433228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7105669fddc0d611982501b46d56df54a820ca14cd7e3a3c62c02ef1bd40fc2e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:30:07 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Nov 2023 05:30:07 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:31:22 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Nov 2023 05:31:23 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Nov 2023 05:31:24 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Nov 2023 05:31:25 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 16 Nov 2023 05:31:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Nov 2023 05:31:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Nov 2023 05:31:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Nov 2023 05:31:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Nov 2023 05:31:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Nov 2023 05:31:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Nov 2023 05:31:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Nov 2023 05:31:32 GMT
EXPOSE 80
# Thu, 16 Nov 2023 05:31:33 GMT
EXPOSE 443
# Thu, 16 Nov 2023 05:31:34 GMT
EXPOSE 443/udp
# Thu, 16 Nov 2023 05:31:35 GMT
EXPOSE 2019
# Thu, 16 Nov 2023 05:32:33 GMT
RUN caddy version
# Thu, 16 Nov 2023 05:32:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d66ae500a331057bbb6b25a0c0e5718f2491209d7330f70b1203472b199bd5b`  
		Last Modified: Thu, 16 Nov 2023 05:37:31 GMT  
		Size: 451.2 KB (451175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec48b5261067a4b4643799633487cce5b6ee11cce36314b8a6b22964fd46ba4`  
		Last Modified: Thu, 16 Nov 2023 05:37:30 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bc40730815ee35e950756a15aa93561edd0f272d34d30de69bb8d7f58b1d8e`  
		Last Modified: Thu, 16 Nov 2023 05:37:34 GMT  
		Size: 15.3 MB (15273771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfce8b69f4cadeeaa9fcc771a3a5b374fc4a3c8c41c1a42a7878c1cad861645c`  
		Last Modified: Thu, 16 Nov 2023 05:37:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdd09852c86166de537f8b5f5b78eca092cfb95e9e2e1194c84a7a05334e5c4`  
		Last Modified: Thu, 16 Nov 2023 05:37:29 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f15c2b10239537d18dc39c5208acb0c8fc7bc25d6cd95cb59ed8e8aaf8b73be`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa35da536891cce8df35bca524d15b1b7465d4fc14354a1a15a2fa39d71a4a88`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654652f0bb6c82a0e1fd51010fd587112527866df3c9748cf9ed4414e70ee612`  
		Last Modified: Thu, 16 Nov 2023 05:37:29 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0fcd5cbdfe3f968d65ba5dcece2d017de82a3a4ec737745bd5560697735689`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9396734c66d2d27545fdeb2c33a462651a3807dfcbd04b590a01ace722161a21`  
		Last Modified: Thu, 16 Nov 2023 05:37:27 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a14586579bd1d9d9a9162b0678a119c826a7be5039b5419e90b82c772b33677`  
		Last Modified: Thu, 16 Nov 2023 05:37:27 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c773c8968545d0fca628d03a3b588ca4798423090cadd666d023cee5065235a5`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce86207f89519b9df4526afc22e743fef4a6266614fb8e082e975bf0f01862f`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7392ec7da7419f69c0413116467249934c403f42b53ff6090608481e1ba7985a`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73d1eee374e37176384bade9abdbe65d5aed23b976c507b3b88b17c758761f`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d556f28b534238f3c8497a928caa36428f1d333a69cabf15b4fc3d80aa7f3f9f`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd0eba7ede6da63115506e40bf2b6990915e5fba916e919c6525f447018bbd9`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf5b269f798b76bfba9ad2e27b5aab7bebe448007c818230643c16d6cf761af`  
		Last Modified: Thu, 16 Nov 2023 05:37:25 GMT  
		Size: 252.7 KB (252713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c70c9a3deaf4a41d4192a9248f3fd5ccfadb54792687f31f63a17f46e5134c`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:7302fa54b56c8f2363f0caf1ac496c297c9eda88207a05836e5e06c40272769b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2113; amd64

### `caddy:2.7-windowsservercore-ltsc2022` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:7a86ad9fb59b43cc97f50c3516b4153bb228276c026e4c802c4a213b0fe1c20f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1902803411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03625f7f4ec599de5399e0e9d5f36d3c2052adeb06f8349ef7a96e3777ddf4e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 09 Nov 2023 06:47:20 GMT
RUN Install update 10.0.20348.2113
# Thu, 16 Nov 2023 01:36:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:33:15 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Nov 2023 05:33:16 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:33:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Nov 2023 05:33:45 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Nov 2023 05:33:46 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Nov 2023 05:33:47 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 16 Nov 2023 05:33:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Nov 2023 05:33:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Nov 2023 05:33:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Nov 2023 05:33:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Nov 2023 05:33:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Nov 2023 05:33:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Nov 2023 05:33:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Nov 2023 05:33:54 GMT
EXPOSE 80
# Thu, 16 Nov 2023 05:33:55 GMT
EXPOSE 443
# Thu, 16 Nov 2023 05:33:56 GMT
EXPOSE 443/udp
# Thu, 16 Nov 2023 05:33:57 GMT
EXPOSE 2019
# Thu, 16 Nov 2023 05:34:33 GMT
RUN caddy version
# Thu, 16 Nov 2023 05:34:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7989ef2c4cfb06d845746a3c3660481ea84d3f5c8216041855ce528f0ac4015c`  
		Last Modified: Tue, 14 Nov 2023 20:43:13 GMT  
		Size: 498.2 MB (498182566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbeb193d02c2ca7f9a9ea438fbf1bcdb6ea4a6fea626713330fd1ebb514424f`  
		Last Modified: Thu, 16 Nov 2023 02:25:14 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b269b5ac8d8c6baa501ca9b38fa715170022416aa7332a2d155a06529882b84a`  
		Last Modified: Thu, 16 Nov 2023 05:37:59 GMT  
		Size: 458.2 KB (458201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f982a236809063ef75b5db6a226207448d936d7791ede196115611649805c5`  
		Last Modified: Thu, 16 Nov 2023 05:37:58 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2783cb5dad5df996a48a9ebf989a6136c91f524f421bfff9e71ab764da46fd04`  
		Last Modified: Thu, 16 Nov 2023 05:38:01 GMT  
		Size: 15.3 MB (15269735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa26255a8f194a0aa31a8fd0c48e7dfba117358880abeaf7ad3c5f54a6be87d`  
		Last Modified: Thu, 16 Nov 2023 05:37:57 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706b8120af6e900b1d0dea48743c4fd50b63c785dbe02b5ccd4af53e68ebefff`  
		Last Modified: Thu, 16 Nov 2023 05:37:57 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c12376eb1027b4892f92b1b8dd45b1e05d78f365c2886ded9202ffbaab80e9`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a29b9f98e523c3477366f98e560b8638fb5c3f0a7a8c76c9a417a33b4d44804`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a9a2fb5b49cb3e38b64f06a755f57ec37b8b5eaf2152fe9e38ae9c8cb3b593`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53a0ea77b4fcc256276d31401de856267c72aeac7fefeeb6fbe655340bb4cf4`  
		Last Modified: Thu, 16 Nov 2023 05:37:55 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d80b783b85d05309ef9fe97740b873bd9092c13b53eea3d83adf6197cbe798`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9454c6602eef29f64927e75d96b8f26d7cf0c6c089afa91e260207675216501`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f23d9fc021e786b83141dd57c2a10dc279d17eacad254ec81d7922372d17876`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55a4267cea49483a79cbee8908d3daf6af4fb6fa1af94e350072034f128c5a1`  
		Last Modified: Thu, 16 Nov 2023 05:37:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9723590c56e28022e6ee055495ee5826c7ea085d2a8b7255d471b35bb27e9a6c`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b39c632f1f53a232721260e3ebcc755559883edb0272949f2d965799d62ef5`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3deb93ce29c0157e6c6b82bbad0ffb2102a833ea54672c93c05843899eac3bc`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09fe12ffad65804e54e566d7b3256d98268c5e943a40282d44bab50d3fb6a04`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517e7fd42cd9750ca7ef5a68df02e2bdc3be404dbd69681f36c7b0acb1562550`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 270.1 KB (270069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0727df29cc57ce0bb7db3c73852d6eaceb439603493f2e3ceb07ce2f8e8e4e99`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.6`

**does not exist** (yet?)

## `caddy:2.7.6-alpine`

**does not exist** (yet?)

## `caddy:2.7.6-builder`

**does not exist** (yet?)

## `caddy:2.7.6-builder-alpine`

**does not exist** (yet?)

## `caddy:2.7.6-builder-windowsservercore-1809`

**does not exist** (yet?)

## `caddy:2.7.6-builder-windowsservercore-ltsc2022`

**does not exist** (yet?)

## `caddy:2.7.6-windowsservercore`

**does not exist** (yet?)

## `caddy:2.7.6-windowsservercore-1809`

**does not exist** (yet?)

## `caddy:2.7.6-windowsservercore-ltsc2022`

**does not exist** (yet?)

## `caddy:alpine`

```console
$ docker pull caddy@sha256:9821d1ef822957bf0ac22f9c6e26ad6a3198604f29b3b79194acba7ccaff4532
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
$ docker pull caddy@sha256:0eff0e7322c718fc65b783418531f1e75c7f27f1a3877823378737e91296ee8c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18474760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3791fd914060b4c02165b77f6f2c6e4516be2e77a6a8bd8ffab228253f75f47`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:32:06 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 06:32:07 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 06:32:07 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 06:32:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 06:32:10 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 06:32:10 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 06:32:10 GMT
EXPOSE 80
# Fri, 01 Dec 2023 06:32:11 GMT
EXPOSE 443
# Fri, 01 Dec 2023 06:32:11 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 06:32:11 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 06:32:11 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 06:32:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08886dfc0722c4ed2cb6a70c285a33fe35aec069435868488356dde320b4d21c`  
		Last Modified: Fri, 01 Dec 2023 06:32:30 GMT  
		Size: 350.8 KB (350845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0132c3b72c65b40cace6033d219e1e6d680bb85808270b77a5189c509c10bc0`  
		Last Modified: Fri, 01 Dec 2023 06:32:29 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2ecdf85e2f8f19fc737312e7157f0141b45020324fcf01f4e92bbe707d8983`  
		Last Modified: Fri, 01 Dec 2023 06:32:32 GMT  
		Size: 14.7 MB (14713987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e05dc14b4b6c6dbdcfbdbe28c73e86cafc5287fa13d4f51fdfdfad7b51b8936d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17423853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3acb342ef8cbce6055e45fdabe7e8b60e98cab9d0aa967e362098333633440ff`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:39:01 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 00:39:02 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 00:39:03 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 00:39:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 00:39:05 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 00:39:05 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 00:39:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 00:39:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 00:39:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 80
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 443
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 00:39:06 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 00:39:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc24e4ccf558b6e992efaaa7a735322be11fe99ce19e722eee6ae70bb76515d`  
		Last Modified: Fri, 01 Dec 2023 00:39:21 GMT  
		Size: 347.6 KB (347632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cd6f3873930f7c6aa4ee5d06ef24c77a840fec6f0211e9572fbe0f43c04e1f`  
		Last Modified: Fri, 01 Dec 2023 00:39:21 GMT  
		Size: 7.5 KB (7508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c51a919a8bb024456b258f25a71adb53a14e30c7134e81fac343c44dbf7230c`  
		Last Modified: Fri, 01 Dec 2023 00:39:23 GMT  
		Size: 13.9 MB (13921843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:c3be58f3d1b5614d2a5e7bff50bc07567044bb119ec0f286c94df8169efc313b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17156415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194c773f5747022fdb5fc8d32e8dafcafd61f37e52238ad53627e3309c2fb4cb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:19:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 03:19:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 03:19:15 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 03:19:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 03:19:19 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 03:19:19 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 03:19:20 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 03:19:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 03:19:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 03:19:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 03:19:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 03:19:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 03:19:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 03:19:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 03:19:22 GMT
EXPOSE 80
# Fri, 01 Dec 2023 03:19:22 GMT
EXPOSE 443
# Fri, 01 Dec 2023 03:19:23 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 03:19:23 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 03:19:23 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 03:19:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803b34e1f84b29ca968d2fbf85c278608566c34dfd1742e088c6483685957029`  
		Last Modified: Fri, 01 Dec 2023 03:19:48 GMT  
		Size: 344.5 KB (344464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bbcb291a405e073d645e52039b6f84fa5071645ceb53988f99d384fbc6c4c1`  
		Last Modified: Fri, 01 Dec 2023 03:19:48 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d0aed5710d79e6bba64ce3cf139d40c4e2c3003d1feec3776b18919e3a1423`  
		Last Modified: Fri, 01 Dec 2023 03:19:50 GMT  
		Size: 13.9 MB (13903440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e7f68eb0f76a55ada8be1bb5213e5bbbcb0727fa8d4051f6f3edf1275bc2dc40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17274998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9487e6591f483b0f0d5fe25a89d069485fa10bb97a06ef07085f28b86995977c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:11:08 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 03:11:09 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 03:11:10 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 03:11:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 03:11:11 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 03:11:11 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 80
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 443
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 03:11:12 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 03:11:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e383270d6915b6b427f49a75d657d5a0403fcd47a5f89cd30e85143ca54c22`  
		Last Modified: Fri, 01 Dec 2023 03:11:28 GMT  
		Size: 360.7 KB (360655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27e927f808292c7b306432ed3ee61ecc6b7f637b8ccbdf5cb2d6bdc24649858`  
		Last Modified: Fri, 01 Dec 2023 03:11:28 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dab02cb145c1d5336977666f796446f69abbbfa721ab7a71525867eb3edfbc`  
		Last Modified: Fri, 01 Dec 2023 03:11:30 GMT  
		Size: 13.6 MB (13573804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:3f9f202dc07f3bb097e0e78330d59f52c488ff4ba3b4aa4a569f1a28c9db95f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.1 MB (17058981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:126d26f69982d49f88bac36f166a92d251494018b25e2e255972b98f38f495f8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:42:19 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 05:42:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 05:42:52 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 05:42:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 05:43:00 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 05:43:20 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 05:43:24 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 05:43:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 05:43:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 05:43:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 05:43:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 05:43:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 05:43:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 05:43:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 05:43:45 GMT
EXPOSE 80
# Fri, 01 Dec 2023 05:43:46 GMT
EXPOSE 443
# Fri, 01 Dec 2023 05:43:46 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 05:43:47 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 05:43:48 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 05:43:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce4bc2907f69809c3086f118895d7e5c8683349557239c0ce79dfbda0ce3768`  
		Last Modified: Fri, 01 Dec 2023 05:44:17 GMT  
		Size: 362.2 KB (362185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef8889b660799cb5b3c54f8771b4a37ad12c12f245aa74e4af501a899449137`  
		Last Modified: Fri, 01 Dec 2023 05:44:17 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681f2bb9965ff577316200c634bfb7e7db0d5b2ba971441db97e1405e3c0fc6b`  
		Last Modified: Fri, 01 Dec 2023 05:44:19 GMT  
		Size: 13.3 MB (13340969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:159a339dbc4d0e8279faad422e0a871d82adcc6736b9c4ac4c4b252c3dbee6a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.8 MB (17825031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0c61727c246c9eedd4c40bc927993a89531560cc027902c6f00b8f288f96b77`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:22:31 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 08:22:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 08:22:32 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 08:22:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 08:22:37 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 08:22:37 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 08:22:38 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 08:22:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 80
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 443
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 08:22:38 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 08:22:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20bbe0abb0a3f63718aa78742832077ad86b8ae86d70ce3ebcece342ec022c6`  
		Last Modified: Fri, 01 Dec 2023 08:23:07 GMT  
		Size: 354.9 KB (354948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1497491e477a92a5e82d0d68588396a3414c6e703fdc68c82c768ad6b18b28`  
		Last Modified: Fri, 01 Dec 2023 08:23:07 GMT  
		Size: 7.5 KB (7502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539ac3a1bb2d355499d388b4de966f9148263d5603f2db92aeba42084d02b3cf`  
		Last Modified: Fri, 01 Dec 2023 08:23:09 GMT  
		Size: 14.2 MB (14245127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:dfd9af513214974c6a77e5e89c7cd3c6d2ddddb226bd21f95118958d47c0c537
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.5122; amd64
	-	windows version 10.0.20348.2113; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:fd75db17630bfaadeef0d2ee65994b5714e8b50b680116e62063b53f58ee8494
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76963250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c15f2632afa610125145b4eeb7cd15cfd6eb2789f9806d851ebe5254b2e0b4aa`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:46:23 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 03:46:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:25:52 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:26:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:26:02 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:26:02 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:26:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:26:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:26:03 GMT
WORKDIR /go
# Tue, 05 Dec 2023 20:48:59 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 20:48:59 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 20:48:59 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 20:48:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 20:48:59 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 20:49:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 20:49:01 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 20:49:01 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501dced60f86be38cc73d3c038f7db4afeee65726f7e422aacf09244539ebf1`  
		Last Modified: Fri, 01 Dec 2023 03:50:39 GMT  
		Size: 284.7 KB (284697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63d189496f5f03c835c9c85df2db6920546d36a1701f6b5ad15f800c671605d`  
		Last Modified: Tue, 05 Dec 2023 20:31:27 GMT  
		Size: 67.0 MB (67003308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aeb88dd0f3e06a57abc08c781b85c89d138194918c469aea9a1bed9753d2ed0`  
		Last Modified: Tue, 05 Dec 2023 20:31:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40ff2505fd8d96e76bddb63b05c2d42815db1dabe0093ec8f8f53be403b0d01`  
		Last Modified: Tue, 05 Dec 2023 20:49:17 GMT  
		Size: 5.0 MB (4970029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3868d63c7cd554f20832e0aff9559fa0cdd7cdbaa4de14e8043fefd0ebfde5`  
		Last Modified: Tue, 05 Dec 2023 20:49:16 GMT  
		Size: 1.3 MB (1302235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a2748825cf9745fffb7f4807c0b6fd474a0221d0d19177142c3f952e10ac78`  
		Last Modified: Tue, 05 Dec 2023 20:49:16 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2c90abb7280a71391618e8552a4faa4e66eb61f80d02402126d25f1365cf063f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75409540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a539589e36806b442a969b2dcf589a62915dde0f6bee440eb73fda5d315a9dd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:53:48 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 00:53:48 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:49:18 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:49:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:49:36 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:49:36 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:49:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:49:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:49:37 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:11:53 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:11:53 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:11:53 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:11:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:11:53 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:11:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:11:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:11:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e7ba0492eb25e7f21078441d7cdc65088836bc1984bc4a14cd3e9cd75cbf32`  
		Last Modified: Fri, 01 Dec 2023 01:00:23 GMT  
		Size: 284.9 KB (284884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de60bcfc919bc6b53554a040a5a58936a8d2e2bf66b2872b69d7a3164e35923f`  
		Last Modified: Tue, 05 Dec 2023 20:54:54 GMT  
		Size: 65.8 MB (65764248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e61f3b09467cb2b97e65a90f25e38cba8acfcd387d168214a949b59bf8c09a`  
		Last Modified: Tue, 05 Dec 2023 20:54:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7827ddd1dfa7654d070274e573dbfcc8fb5ac2ef73888f8b0563e0672811ad`  
		Last Modified: Tue, 05 Dec 2023 21:12:11 GMT  
		Size: 5.0 MB (4964331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f919a9a90cd0240dfd228f8b093cb51b08bf03eabc0326cfe303219b37469f5`  
		Last Modified: Tue, 05 Dec 2023 21:12:11 GMT  
		Size: 1.2 MB (1248647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66464a5ea9ace101c6914e8c5da3a953cb5a9b372ffc562f6a7ab2bcc2b9c0a6`  
		Last Modified: Tue, 05 Dec 2023 21:12:11 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:f65daee5179d36a392c0d931a02c5c400f99b4470bd68e3f326d6828bd8f3fb6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74707169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53077f2480efa131c1c20460899eb69b049d624d249a844e4e1c3bd88aa28d12`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:44:57 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 08:44:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:58:01 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:58:16 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:58:16 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:58:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:58:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:58:17 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:22:31 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:22:31 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:22:31 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:22:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:22:31 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:22:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:22:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:22:32 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a824ff289f1a3c765a444079137b8b7f1cee80348faa53e1ba4c960b73ed2a`  
		Last Modified: Fri, 01 Dec 2023 08:49:42 GMT  
		Size: 284.1 KB (284079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4989177b4ed66b7e9f9e8c4bfce82720b582e24b735d6628effa75d81c5718fc`  
		Last Modified: Tue, 05 Dec 2023 21:04:43 GMT  
		Size: 65.8 MB (65764197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f9b58eae167c54d3faa3eeffd480cdae7e8b4841eb816a86cfdd01f8ae29ef`  
		Last Modified: Tue, 05 Dec 2023 21:04:29 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4cd1a3aab8fc02791b1e19f81b7de1bd691c10a7c942acc7e733221bf12888`  
		Last Modified: Tue, 05 Dec 2023 21:22:47 GMT  
		Size: 4.5 MB (4511237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3a92f0249b45814852e4e987e1a6304bcfb211077150ab43415b31d929f4af`  
		Last Modified: Tue, 05 Dec 2023 21:22:47 GMT  
		Size: 1.2 MB (1246087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3152bffd7f15885d0e72b0adabc22f46542f569db908b69d63eb29addd5e950`  
		Last Modified: Tue, 05 Dec 2023 21:22:47 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:977753f53683eb84ddc7477e5a743e0e1e4e2a001f20edfa0f01d43359d85dc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73981644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0f601640aa519cb421e86cd75a6ad6223541d58cfe80b27b699a23a2585ce70`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:43:53 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 03:18:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:16:18 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:16:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:16:28 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:16:28 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:16:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:16:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:16:28 GMT
WORKDIR /go
# Tue, 05 Dec 2023 20:38:16 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 20:38:16 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 20:38:16 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 20:38:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 20:38:16 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 20:38:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 20:38:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 20:38:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a63ed24dc22a348b35d99b5ec9dc67ff66563b539875e5c8ab2d870b3991ac`  
		Last Modified: Fri, 01 Dec 2023 02:44:03 GMT  
		Size: 286.3 KB (286307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f00641dffc5c2a149049ee9046bb24cfc7de534b7495a0f27784a4fff0fadc`  
		Last Modified: Tue, 05 Dec 2023 20:21:00 GMT  
		Size: 64.1 MB (64094844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452682ba77e89fc55be3a168358f5f43bccad93ecdd3d53b4dec7fff6915128b`  
		Last Modified: Tue, 05 Dec 2023 20:20:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3fe1e12507f8c4a2731393eebfc5ab973aa344b0daceec525560b812b26f60`  
		Last Modified: Tue, 05 Dec 2023 20:38:33 GMT  
		Size: 5.1 MB (5068450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb3c2fad921714e69ace0b18d8f72eb2566d50bc92ff9e9dd125ec383131eb9`  
		Last Modified: Tue, 05 Dec 2023 20:38:32 GMT  
		Size: 1.2 MB (1198449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9c40c8a39fcf5ab6fa64b1c2e1dd5d0b5c1f6b4d9c11ed9481644fe94f1cbf`  
		Last Modified: Tue, 05 Dec 2023 20:38:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:50de875c68ad6aeffc5eb2dd0942d219481fe70c55088657bbe724abd05f7c49
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74206489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7029045647c7331bb58455d58f274c3e4356d86729c097b8d3cfe35717b3b9d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:37:34 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 06:37:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:38:14 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:38:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:38:37 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:38:38 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:38:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:38:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:38:41 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:04:33 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:04:34 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:04:35 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:04:35 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:04:35 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:04:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:04:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:04:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692dbecd5e141c462ab06ef113ec964b525e7564d734890cc1d5b1dbf33ee34e`  
		Last Modified: Fri, 01 Dec 2023 06:43:30 GMT  
		Size: 286.7 KB (286661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc89a0f2d97ecfd4d20235e72227fc24aa79a64509fe9ea64702db658f2ad26d`  
		Last Modified: Tue, 05 Dec 2023 20:46:23 GMT  
		Size: 64.1 MB (64115804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d76f2c2e2bbb4190b1865ddafdc8cb88adee4c79d7d5ba23e69696e9610889`  
		Last Modified: Tue, 05 Dec 2023 20:46:11 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e0ec0f713ee657d6aa159fab65c05939480b5ca50a8e3dc4b1a9a6578160f7`  
		Last Modified: Tue, 05 Dec 2023 21:04:57 GMT  
		Size: 5.3 MB (5268970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e164016cca4964643911960baccae8beaa47cc5086bbe3ebfd14183d5204a8`  
		Last Modified: Tue, 05 Dec 2023 21:04:56 GMT  
		Size: 1.2 MB (1186171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2932f0ef681ac7135c1e7ff9332dd4c154c1f793d04fda438db30a1573bacc8b`  
		Last Modified: Tue, 05 Dec 2023 21:04:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:98d5d7af77acd9cc1b74499ba61056fb599a17742331f51a0fffa89ef56bb114
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76098838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d4f342a39bbb58bda0421e578348bf6d047bf7125db5c42216b2ba9b6d5040d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:14:49 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 08:14:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:44:16 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:44:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:45:03 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:45:04 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:45:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:45:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:45:05 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:14:29 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:14:29 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:14:29 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:14:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:14:30 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:14:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:14:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:14:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab563e8d41683e124df048aa9b564b0e8e1021e85213666971a015df51d5e48`  
		Last Modified: Fri, 01 Dec 2023 08:20:46 GMT  
		Size: 285.1 KB (285090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d44aea4caa072a45cb44ab86f401c76153b599207fb3cc311f44308e9b5da13`  
		Last Modified: Tue, 05 Dec 2023 20:57:00 GMT  
		Size: 66.2 MB (66218626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef66858f73257b9fd43395b7e2758cdaa72267303442d3a5dbef122796530c5`  
		Last Modified: Tue, 05 Dec 2023 20:56:49 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5261478888d8f0caaf878da0629c62f928bbbff35e7f873c1a463c6e39c0bd37`  
		Last Modified: Tue, 05 Dec 2023 21:14:53 GMT  
		Size: 5.1 MB (5114717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade58cb7b8ea422e0ab68cb58091d9adc84172a8de51990bb80269c07c5bd556`  
		Last Modified: Tue, 05 Dec 2023 21:14:53 GMT  
		Size: 1.3 MB (1262391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7f47ab035030fe8af075c6b5ebf045cd6bd32bef0700d8cc656ba7204685b7`  
		Last Modified: Tue, 05 Dec 2023 21:14:52 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:a4a6967f69e81e55f736b4e5d91bab0e44ce577821e0336b8b8ef7456679e1c1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2154296990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14a551f4e77e9632ddd054915a37f355befe0b5201417194368482bc6a54949d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 02:47:03 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Nov 2023 02:47:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Nov 2023 02:47:05 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Nov 2023 02:47:06 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Nov 2023 02:48:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:48:31 GMT
ENV GOPATH=C:\go
# Thu, 16 Nov 2023 02:49:41 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 05 Dec 2023 20:18:04 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:21:11 GMT
RUN $url = 'https://dl.google.com/go/go1.21.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'bbe603cde7c9dee658f45164b4d06de1eff6e6e6b800100824e7c00d56a9a92f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 05 Dec 2023 20:21:13 GMT
WORKDIR C:\go
# Tue, 05 Dec 2023 20:59:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 05 Dec 2023 20:59:30 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 20:59:31 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 20:59:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:00:49 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 05 Dec 2023 21:00:50 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e901367fac1450f509d3118ada9e004e3613844ebdf91861147a093483930a4`  
		Last Modified: Thu, 16 Nov 2023 03:11:57 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e08004205bd077d8f22b013c70dc2f10796c64fced1eb9927e0055daff2d05d`  
		Last Modified: Thu, 16 Nov 2023 03:11:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebc5048afc68ef48e2f2136545e2cccf26bb29eb4926bf4259b370ad55b4e7a`  
		Last Modified: Thu, 16 Nov 2023 03:11:55 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f50fe5c7ef21648f3eaa4304932877a116fcb910b8e9095c779a2fbe6d57f7e`  
		Last Modified: Thu, 16 Nov 2023 03:11:55 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76fe0e37750041d4ede2a0ca3b5245cfe075c3eb2ee27d7ce72ee8c3d7b20cc`  
		Last Modified: Thu, 16 Nov 2023 03:12:00 GMT  
		Size: 25.5 MB (25537512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8097bb9b8778d15dbf89d899653bf1634ec17554e5d84ef1ccfcac8ebf86afe2`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b542d31e914d67da86cc5701cdc282ab664dc1170507e3802e22ab3026436a90`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 263.2 KB (263200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86acdf7d3955fb44136bac433a30ccbbb97863120f270af32659dd65446666c7`  
		Last Modified: Tue, 05 Dec 2023 20:39:22 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1abe126c354944b7db8aa724d8f757167f7c3b36d39f976ef3b1b0d1b1b65ab`  
		Last Modified: Tue, 05 Dec 2023 20:39:41 GMT  
		Size: 69.4 MB (69361283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6338af096e09067ad482a0f4a6df1d1eee5b5595a64ca5f367b94ce27903e284`  
		Last Modified: Tue, 05 Dec 2023 20:39:22 GMT  
		Size: 1.5 KB (1529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0adc218b27ef5639384c060fb663de3bd74374279d3fd525aa281f63a754779`  
		Last Modified: Tue, 05 Dec 2023 21:02:06 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c21053b248805df7ad888734f5cd1df5a6b426111512d5a6b7530060e7f30b2`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57f384772c293e1d97326febf9e29d6bfef6eb9da2b053b6ad1e0ebea539508`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a2cba3fcdba1e3612614837be0fed9e3b7670483867a14203a15d395aa4179`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b447549db21db40db8a08cddb7d529bbd6e183aba676f13e2a3a5ff034fb67f8`  
		Last Modified: Tue, 05 Dec 2023 21:02:04 GMT  
		Size: 1.7 MB (1685436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408a12340d35fbfeee8cc5bdec3421ede796686f2b22d693863de08da6d51c91`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:081774d66d26fdb1b8b89fc90aeb9a72c559c0690770f153fa4ca3f1d5450e43
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1983623458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af2bcbcbf997ed6d0e17a2acebd1f65d19dbb6868d0523c306342bcc37644dd6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 09 Nov 2023 06:47:20 GMT
RUN Install update 10.0.20348.2113
# Thu, 16 Nov 2023 01:36:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 02:43:34 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Nov 2023 02:43:35 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Nov 2023 02:43:36 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Nov 2023 02:43:37 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Nov 2023 02:44:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:44:11 GMT
ENV GOPATH=C:\go
# Thu, 16 Nov 2023 02:44:30 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 05 Dec 2023 20:15:35 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:17:49 GMT
RUN $url = 'https://dl.google.com/go/go1.21.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'bbe603cde7c9dee658f45164b4d06de1eff6e6e6b800100824e7c00d56a9a92f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 05 Dec 2023 20:17:50 GMT
WORKDIR C:\go
# Tue, 05 Dec 2023 21:00:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 05 Dec 2023 21:00:58 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:00:59 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:01:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:01:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 05 Dec 2023 21:01:26 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7989ef2c4cfb06d845746a3c3660481ea84d3f5c8216041855ce528f0ac4015c`  
		Last Modified: Tue, 14 Nov 2023 20:43:13 GMT  
		Size: 498.2 MB (498182566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbeb193d02c2ca7f9a9ea438fbf1bcdb6ea4a6fea626713330fd1ebb514424f`  
		Last Modified: Thu, 16 Nov 2023 02:25:14 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b1d4a557f047b695f94452d9707061981d7fae4239c674b332282b8291963c`  
		Last Modified: Thu, 16 Nov 2023 03:11:20 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45549c207f14d769cba7c36b66157ec213bbc32ce57d685d8e2c407cf3987bb`  
		Last Modified: Thu, 16 Nov 2023 03:11:18 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c674717e06bf8cb25d5887393ef9568ee0ab6390966b9666808e836e9bd471d`  
		Last Modified: Thu, 16 Nov 2023 03:11:18 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2227badcd9f5f2b70b3d2ffd1c18887498f413c07802bfb334e8dc7b2d2acc`  
		Last Modified: Thu, 16 Nov 2023 03:11:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9f3b5e90a2e6028cf194e870b24a7158f875f18b81f4f9137a5db3ea1f79ac`  
		Last Modified: Thu, 16 Nov 2023 03:11:23 GMT  
		Size: 25.5 MB (25536225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7811a5416dcd19193a5b3ab9327607bf845f7ff77f95d3e20abdfb7435c32ae0`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5931209e960a94616639ea72e4d3ad9dc9cb554790ce930152c73bdc1449c034`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 266.6 KB (266600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a70f603a2fb4e76edd3165b62a179fb8f6410e265f5ae4a3732ee68e610034b`  
		Last Modified: Tue, 05 Dec 2023 20:38:48 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e37840dec3a6665ce48520be8b2c51b654359765bee5ab0780ee74746f0eb2`  
		Last Modified: Tue, 05 Dec 2023 20:39:08 GMT  
		Size: 69.3 MB (69342960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d16ae54757acda093616d24735d4c92d4676649bec49807fc35de90d15e15c`  
		Last Modified: Tue, 05 Dec 2023 20:38:48 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5744d01eddd2ef9d9673fdb0f0e48203fad1b01f2b14899a3ec6393c4548e75`  
		Last Modified: Tue, 05 Dec 2023 21:02:23 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35bb848667aa413b6ce6c309a4c2169635b0740dc335b9b39413a00627c01ab`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78369d5e83dd4f4ca5558a32848f3515e191b15f8427ea166a4f6327694ff9db`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2ae381a5e49194e43b26ac8036b1da5d2af930f7516796c476bcdb9c8125e3`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09db71960c4c717ed44d2694cf77f248223822e163297046010868c3ebf0767`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.7 MB (1677926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9dfae036c2fe0cfcd2e4f5a9acc265c45af769542844b9b617b62ec3ebd591`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:3e0232193d2e16a551210bb7cf4da86b6d0bf45cb70508c343c680065d7c440e
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
$ docker pull caddy@sha256:fd75db17630bfaadeef0d2ee65994b5714e8b50b680116e62063b53f58ee8494
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76963250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c15f2632afa610125145b4eeb7cd15cfd6eb2789f9806d851ebe5254b2e0b4aa`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:46:23 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 03:46:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:25:52 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:26:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:26:02 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:26:02 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:26:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:26:03 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:26:03 GMT
WORKDIR /go
# Tue, 05 Dec 2023 20:48:59 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 20:48:59 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 20:48:59 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 20:48:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 20:48:59 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 20:49:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 20:49:01 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 20:49:01 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501dced60f86be38cc73d3c038f7db4afeee65726f7e422aacf09244539ebf1`  
		Last Modified: Fri, 01 Dec 2023 03:50:39 GMT  
		Size: 284.7 KB (284697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63d189496f5f03c835c9c85df2db6920546d36a1701f6b5ad15f800c671605d`  
		Last Modified: Tue, 05 Dec 2023 20:31:27 GMT  
		Size: 67.0 MB (67003308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aeb88dd0f3e06a57abc08c781b85c89d138194918c469aea9a1bed9753d2ed0`  
		Last Modified: Tue, 05 Dec 2023 20:31:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40ff2505fd8d96e76bddb63b05c2d42815db1dabe0093ec8f8f53be403b0d01`  
		Last Modified: Tue, 05 Dec 2023 20:49:17 GMT  
		Size: 5.0 MB (4970029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3868d63c7cd554f20832e0aff9559fa0cdd7cdbaa4de14e8043fefd0ebfde5`  
		Last Modified: Tue, 05 Dec 2023 20:49:16 GMT  
		Size: 1.3 MB (1302235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a2748825cf9745fffb7f4807c0b6fd474a0221d0d19177142c3f952e10ac78`  
		Last Modified: Tue, 05 Dec 2023 20:49:16 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:2c90abb7280a71391618e8552a4faa4e66eb61f80d02402126d25f1365cf063f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75409540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a539589e36806b442a969b2dcf589a62915dde0f6bee440eb73fda5d315a9dd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:53:48 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 00:53:48 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:49:18 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:49:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:49:36 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:49:36 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:49:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:49:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:49:37 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:11:53 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:11:53 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:11:53 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:11:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:11:53 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:11:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:11:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:11:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e7ba0492eb25e7f21078441d7cdc65088836bc1984bc4a14cd3e9cd75cbf32`  
		Last Modified: Fri, 01 Dec 2023 01:00:23 GMT  
		Size: 284.9 KB (284884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de60bcfc919bc6b53554a040a5a58936a8d2e2bf66b2872b69d7a3164e35923f`  
		Last Modified: Tue, 05 Dec 2023 20:54:54 GMT  
		Size: 65.8 MB (65764248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e61f3b09467cb2b97e65a90f25e38cba8acfcd387d168214a949b59bf8c09a`  
		Last Modified: Tue, 05 Dec 2023 20:54:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7827ddd1dfa7654d070274e573dbfcc8fb5ac2ef73888f8b0563e0672811ad`  
		Last Modified: Tue, 05 Dec 2023 21:12:11 GMT  
		Size: 5.0 MB (4964331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f919a9a90cd0240dfd228f8b093cb51b08bf03eabc0326cfe303219b37469f5`  
		Last Modified: Tue, 05 Dec 2023 21:12:11 GMT  
		Size: 1.2 MB (1248647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66464a5ea9ace101c6914e8c5da3a953cb5a9b372ffc562f6a7ab2bcc2b9c0a6`  
		Last Modified: Tue, 05 Dec 2023 21:12:11 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:f65daee5179d36a392c0d931a02c5c400f99b4470bd68e3f326d6828bd8f3fb6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74707169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53077f2480efa131c1c20460899eb69b049d624d249a844e4e1c3bd88aa28d12`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:44:57 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 08:44:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:58:01 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:58:16 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:58:16 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:58:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:58:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:58:17 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:22:31 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:22:31 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:22:31 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:22:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:22:31 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:22:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:22:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:22:32 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a824ff289f1a3c765a444079137b8b7f1cee80348faa53e1ba4c960b73ed2a`  
		Last Modified: Fri, 01 Dec 2023 08:49:42 GMT  
		Size: 284.1 KB (284079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4989177b4ed66b7e9f9e8c4bfce82720b582e24b735d6628effa75d81c5718fc`  
		Last Modified: Tue, 05 Dec 2023 21:04:43 GMT  
		Size: 65.8 MB (65764197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f9b58eae167c54d3faa3eeffd480cdae7e8b4841eb816a86cfdd01f8ae29ef`  
		Last Modified: Tue, 05 Dec 2023 21:04:29 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4cd1a3aab8fc02791b1e19f81b7de1bd691c10a7c942acc7e733221bf12888`  
		Last Modified: Tue, 05 Dec 2023 21:22:47 GMT  
		Size: 4.5 MB (4511237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3a92f0249b45814852e4e987e1a6304bcfb211077150ab43415b31d929f4af`  
		Last Modified: Tue, 05 Dec 2023 21:22:47 GMT  
		Size: 1.2 MB (1246087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3152bffd7f15885d0e72b0adabc22f46542f569db908b69d63eb29addd5e950`  
		Last Modified: Tue, 05 Dec 2023 21:22:47 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:977753f53683eb84ddc7477e5a743e0e1e4e2a001f20edfa0f01d43359d85dc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73981644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0f601640aa519cb421e86cd75a6ad6223541d58cfe80b27b699a23a2585ce70`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:43:53 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 03:18:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:16:18 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:16:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:16:28 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:16:28 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:16:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:16:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:16:28 GMT
WORKDIR /go
# Tue, 05 Dec 2023 20:38:16 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 20:38:16 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 20:38:16 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 20:38:16 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 20:38:16 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 20:38:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 20:38:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 20:38:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a63ed24dc22a348b35d99b5ec9dc67ff66563b539875e5c8ab2d870b3991ac`  
		Last Modified: Fri, 01 Dec 2023 02:44:03 GMT  
		Size: 286.3 KB (286307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f00641dffc5c2a149049ee9046bb24cfc7de534b7495a0f27784a4fff0fadc`  
		Last Modified: Tue, 05 Dec 2023 20:21:00 GMT  
		Size: 64.1 MB (64094844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452682ba77e89fc55be3a168358f5f43bccad93ecdd3d53b4dec7fff6915128b`  
		Last Modified: Tue, 05 Dec 2023 20:20:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3fe1e12507f8c4a2731393eebfc5ab973aa344b0daceec525560b812b26f60`  
		Last Modified: Tue, 05 Dec 2023 20:38:33 GMT  
		Size: 5.1 MB (5068450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb3c2fad921714e69ace0b18d8f72eb2566d50bc92ff9e9dd125ec383131eb9`  
		Last Modified: Tue, 05 Dec 2023 20:38:32 GMT  
		Size: 1.2 MB (1198449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9c40c8a39fcf5ab6fa64b1c2e1dd5d0b5c1f6b4d9c11ed9481644fe94f1cbf`  
		Last Modified: Tue, 05 Dec 2023 20:38:32 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:50de875c68ad6aeffc5eb2dd0942d219481fe70c55088657bbe724abd05f7c49
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74206489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7029045647c7331bb58455d58f274c3e4356d86729c097b8d3cfe35717b3b9d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:37:34 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 06:37:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:38:14 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:38:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:38:37 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:38:38 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:38:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:38:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:38:41 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:04:33 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:04:34 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:04:35 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:04:35 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:04:35 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:04:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:04:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:04:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692dbecd5e141c462ab06ef113ec964b525e7564d734890cc1d5b1dbf33ee34e`  
		Last Modified: Fri, 01 Dec 2023 06:43:30 GMT  
		Size: 286.7 KB (286661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc89a0f2d97ecfd4d20235e72227fc24aa79a64509fe9ea64702db658f2ad26d`  
		Last Modified: Tue, 05 Dec 2023 20:46:23 GMT  
		Size: 64.1 MB (64115804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d76f2c2e2bbb4190b1865ddafdc8cb88adee4c79d7d5ba23e69696e9610889`  
		Last Modified: Tue, 05 Dec 2023 20:46:11 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e0ec0f713ee657d6aa159fab65c05939480b5ca50a8e3dc4b1a9a6578160f7`  
		Last Modified: Tue, 05 Dec 2023 21:04:57 GMT  
		Size: 5.3 MB (5268970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e164016cca4964643911960baccae8beaa47cc5086bbe3ebfd14183d5204a8`  
		Last Modified: Tue, 05 Dec 2023 21:04:56 GMT  
		Size: 1.2 MB (1186171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2932f0ef681ac7135c1e7ff9332dd4c154c1f793d04fda438db30a1573bacc8b`  
		Last Modified: Tue, 05 Dec 2023 21:04:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:98d5d7af77acd9cc1b74499ba61056fb599a17742331f51a0fffa89ef56bb114
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76098838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d4f342a39bbb58bda0421e578348bf6d047bf7125db5c42216b2ba9b6d5040d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:14:49 GMT
RUN apk add --no-cache ca-certificates
# Fri, 01 Dec 2023 08:14:49 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:44:16 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:44:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.5.linux-amd64.tar.gz'; 			sha256='e2bc0b3e4b64111ec117295c088bde5f00eeed1567999ff77bc859d7df70078e'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.5.linux-armv6l.tar.gz'; 			sha256='837f4bf4e22fcdf920ffeaa4abf3d02d1314e03725431065f4d44c46a01b42fe'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.5.linux-arm64.tar.gz'; 			sha256='841cced7ecda9b2014f139f5bab5ae31785f35399f236b8b3e75dff2a2978d96'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.5.linux-386.tar.gz'; 			sha256='8f4dba9cf5c61757bbd7e9ebdb93b6a30a1b03f4a636a1ba0cc2f27b907ab8e1'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.5.linux-ppc64le.tar.gz'; 			sha256='907b8c6ec4be9b184952e5d3493be66b1746442394a8bc78556c56834cd7c38b'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.5.linux-riscv64.tar.gz'; 			sha256='984d8f999f5019d15527a1a0e6b0c3ef879833e26dcd422ab0ef4d81ac486b96'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.5.linux-s390x.tar.gz'; 			sha256='9c4a81b72ebe44368813cd03684e1080a818bf915d84163abae2ed325a1b2dc0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.5.src.tar.gz'; 		sha256='285cbbdf4b6e6e62ed58f370f3f6d8c30825d6e56c5853c66d3c23bcdb09db19'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Dec 2023 20:45:03 GMT
ENV GOTOOLCHAIN=local
# Tue, 05 Dec 2023 20:45:04 GMT
ENV GOPATH=/go
# Tue, 05 Dec 2023 20:45:04 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 20:45:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 05 Dec 2023 20:45:05 GMT
WORKDIR /go
# Tue, 05 Dec 2023 21:14:29 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 05 Dec 2023 21:14:29 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:14:29 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:14:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:14:30 GMT
ENV XCADDY_SETCAP=1
# Tue, 05 Dec 2023 21:14:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 05 Dec 2023 21:14:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 05 Dec 2023 21:14:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab563e8d41683e124df048aa9b564b0e8e1021e85213666971a015df51d5e48`  
		Last Modified: Fri, 01 Dec 2023 08:20:46 GMT  
		Size: 285.1 KB (285090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d44aea4caa072a45cb44ab86f401c76153b599207fb3cc311f44308e9b5da13`  
		Last Modified: Tue, 05 Dec 2023 20:57:00 GMT  
		Size: 66.2 MB (66218626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef66858f73257b9fd43395b7e2758cdaa72267303442d3a5dbef122796530c5`  
		Last Modified: Tue, 05 Dec 2023 20:56:49 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5261478888d8f0caaf878da0629c62f928bbbff35e7f873c1a463c6e39c0bd37`  
		Last Modified: Tue, 05 Dec 2023 21:14:53 GMT  
		Size: 5.1 MB (5114717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade58cb7b8ea422e0ab68cb58091d9adc84172a8de51990bb80269c07c5bd556`  
		Last Modified: Tue, 05 Dec 2023 21:14:53 GMT  
		Size: 1.3 MB (1262391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7f47ab035030fe8af075c6b5ebf045cd6bd32bef0700d8cc656ba7204685b7`  
		Last Modified: Tue, 05 Dec 2023 21:14:52 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:9a3cb11cfc419a512a550298d752bbf00ea5dc0b4daa8993ab10db26d145fda9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:a4a6967f69e81e55f736b4e5d91bab0e44ce577821e0336b8b8ef7456679e1c1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2154296990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14a551f4e77e9632ddd054915a37f355befe0b5201417194368482bc6a54949d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 02:47:03 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Nov 2023 02:47:04 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Nov 2023 02:47:05 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Nov 2023 02:47:06 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Nov 2023 02:48:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:48:31 GMT
ENV GOPATH=C:\go
# Thu, 16 Nov 2023 02:49:41 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 05 Dec 2023 20:18:04 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:21:11 GMT
RUN $url = 'https://dl.google.com/go/go1.21.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'bbe603cde7c9dee658f45164b4d06de1eff6e6e6b800100824e7c00d56a9a92f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 05 Dec 2023 20:21:13 GMT
WORKDIR C:\go
# Tue, 05 Dec 2023 20:59:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 05 Dec 2023 20:59:30 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 20:59:31 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 20:59:32 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:00:49 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 05 Dec 2023 21:00:50 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e901367fac1450f509d3118ada9e004e3613844ebdf91861147a093483930a4`  
		Last Modified: Thu, 16 Nov 2023 03:11:57 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e08004205bd077d8f22b013c70dc2f10796c64fced1eb9927e0055daff2d05d`  
		Last Modified: Thu, 16 Nov 2023 03:11:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebc5048afc68ef48e2f2136545e2cccf26bb29eb4926bf4259b370ad55b4e7a`  
		Last Modified: Thu, 16 Nov 2023 03:11:55 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f50fe5c7ef21648f3eaa4304932877a116fcb910b8e9095c779a2fbe6d57f7e`  
		Last Modified: Thu, 16 Nov 2023 03:11:55 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76fe0e37750041d4ede2a0ca3b5245cfe075c3eb2ee27d7ce72ee8c3d7b20cc`  
		Last Modified: Thu, 16 Nov 2023 03:12:00 GMT  
		Size: 25.5 MB (25537512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8097bb9b8778d15dbf89d899653bf1634ec17554e5d84ef1ccfcac8ebf86afe2`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b542d31e914d67da86cc5701cdc282ab664dc1170507e3802e22ab3026436a90`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 263.2 KB (263200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86acdf7d3955fb44136bac433a30ccbbb97863120f270af32659dd65446666c7`  
		Last Modified: Tue, 05 Dec 2023 20:39:22 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1abe126c354944b7db8aa724d8f757167f7c3b36d39f976ef3b1b0d1b1b65ab`  
		Last Modified: Tue, 05 Dec 2023 20:39:41 GMT  
		Size: 69.4 MB (69361283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6338af096e09067ad482a0f4a6df1d1eee5b5595a64ca5f367b94ce27903e284`  
		Last Modified: Tue, 05 Dec 2023 20:39:22 GMT  
		Size: 1.5 KB (1529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0adc218b27ef5639384c060fb663de3bd74374279d3fd525aa281f63a754779`  
		Last Modified: Tue, 05 Dec 2023 21:02:06 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c21053b248805df7ad888734f5cd1df5a6b426111512d5a6b7530060e7f30b2`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57f384772c293e1d97326febf9e29d6bfef6eb9da2b053b6ad1e0ebea539508`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a2cba3fcdba1e3612614837be0fed9e3b7670483867a14203a15d395aa4179`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b447549db21db40db8a08cddb7d529bbd6e183aba676f13e2a3a5ff034fb67f8`  
		Last Modified: Tue, 05 Dec 2023 21:02:04 GMT  
		Size: 1.7 MB (1685436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408a12340d35fbfeee8cc5bdec3421ede796686f2b22d693863de08da6d51c91`  
		Last Modified: Tue, 05 Dec 2023 21:02:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:b98db9d0f32752a5a646d4009012af66a84d26002c3605d6fe3da6769aede98d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2113; amd64

### `caddy:builder-windowsservercore-ltsc2022` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:081774d66d26fdb1b8b89fc90aeb9a72c559c0690770f153fa4ca3f1d5450e43
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1983623458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af2bcbcbf997ed6d0e17a2acebd1f65d19dbb6868d0523c306342bcc37644dd6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 09 Nov 2023 06:47:20 GMT
RUN Install update 10.0.20348.2113
# Thu, 16 Nov 2023 01:36:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 02:43:34 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Nov 2023 02:43:35 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Nov 2023 02:43:36 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Nov 2023 02:43:37 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Nov 2023 02:44:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:44:11 GMT
ENV GOPATH=C:\go
# Thu, 16 Nov 2023 02:44:30 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 05 Dec 2023 20:15:35 GMT
ENV GOLANG_VERSION=1.21.5
# Tue, 05 Dec 2023 20:17:49 GMT
RUN $url = 'https://dl.google.com/go/go1.21.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'bbe603cde7c9dee658f45164b4d06de1eff6e6e6b800100824e7c00d56a9a92f'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 05 Dec 2023 20:17:50 GMT
WORKDIR C:\go
# Tue, 05 Dec 2023 21:00:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 05 Dec 2023 21:00:58 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 05 Dec 2023 21:00:59 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 05 Dec 2023 21:01:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 05 Dec 2023 21:01:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 05 Dec 2023 21:01:26 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7989ef2c4cfb06d845746a3c3660481ea84d3f5c8216041855ce528f0ac4015c`  
		Last Modified: Tue, 14 Nov 2023 20:43:13 GMT  
		Size: 498.2 MB (498182566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbeb193d02c2ca7f9a9ea438fbf1bcdb6ea4a6fea626713330fd1ebb514424f`  
		Last Modified: Thu, 16 Nov 2023 02:25:14 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b1d4a557f047b695f94452d9707061981d7fae4239c674b332282b8291963c`  
		Last Modified: Thu, 16 Nov 2023 03:11:20 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45549c207f14d769cba7c36b66157ec213bbc32ce57d685d8e2c407cf3987bb`  
		Last Modified: Thu, 16 Nov 2023 03:11:18 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c674717e06bf8cb25d5887393ef9568ee0ab6390966b9666808e836e9bd471d`  
		Last Modified: Thu, 16 Nov 2023 03:11:18 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2227badcd9f5f2b70b3d2ffd1c18887498f413c07802bfb334e8dc7b2d2acc`  
		Last Modified: Thu, 16 Nov 2023 03:11:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9f3b5e90a2e6028cf194e870b24a7158f875f18b81f4f9137a5db3ea1f79ac`  
		Last Modified: Thu, 16 Nov 2023 03:11:23 GMT  
		Size: 25.5 MB (25536225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7811a5416dcd19193a5b3ab9327607bf845f7ff77f95d3e20abdfb7435c32ae0`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5931209e960a94616639ea72e4d3ad9dc9cb554790ce930152c73bdc1449c034`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 266.6 KB (266600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a70f603a2fb4e76edd3165b62a179fb8f6410e265f5ae4a3732ee68e610034b`  
		Last Modified: Tue, 05 Dec 2023 20:38:48 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e37840dec3a6665ce48520be8b2c51b654359765bee5ab0780ee74746f0eb2`  
		Last Modified: Tue, 05 Dec 2023 20:39:08 GMT  
		Size: 69.3 MB (69342960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d16ae54757acda093616d24735d4c92d4676649bec49807fc35de90d15e15c`  
		Last Modified: Tue, 05 Dec 2023 20:38:48 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5744d01eddd2ef9d9673fdb0f0e48203fad1b01f2b14899a3ec6393c4548e75`  
		Last Modified: Tue, 05 Dec 2023 21:02:23 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35bb848667aa413b6ce6c309a4c2169635b0740dc335b9b39413a00627c01ab`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78369d5e83dd4f4ca5558a32848f3515e191b15f8427ea166a4f6327694ff9db`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2ae381a5e49194e43b26ac8036b1da5d2af930f7516796c476bcdb9c8125e3`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09db71960c4c717ed44d2694cf77f248223822e163297046010868c3ebf0767`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.7 MB (1677926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9dfae036c2fe0cfcd2e4f5a9acc265c45af769542844b9b617b62ec3ebd591`  
		Last Modified: Tue, 05 Dec 2023 21:02:21 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:9eb928f0a3142d0a38e6d457f7696c08c13e070d49d6499cc5b0afe644ecb281
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.5122; amd64
	-	windows version 10.0.20348.2113; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:0eff0e7322c718fc65b783418531f1e75c7f27f1a3877823378737e91296ee8c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18474760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3791fd914060b4c02165b77f6f2c6e4516be2e77a6a8bd8ffab228253f75f47`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:32:06 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 06:32:07 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 06:32:07 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 06:32:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 06:32:10 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 06:32:10 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 06:32:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 06:32:10 GMT
EXPOSE 80
# Fri, 01 Dec 2023 06:32:11 GMT
EXPOSE 443
# Fri, 01 Dec 2023 06:32:11 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 06:32:11 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 06:32:11 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 06:32:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08886dfc0722c4ed2cb6a70c285a33fe35aec069435868488356dde320b4d21c`  
		Last Modified: Fri, 01 Dec 2023 06:32:30 GMT  
		Size: 350.8 KB (350845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0132c3b72c65b40cace6033d219e1e6d680bb85808270b77a5189c509c10bc0`  
		Last Modified: Fri, 01 Dec 2023 06:32:29 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2ecdf85e2f8f19fc737312e7157f0141b45020324fcf01f4e92bbe707d8983`  
		Last Modified: Fri, 01 Dec 2023 06:32:32 GMT  
		Size: 14.7 MB (14713987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e05dc14b4b6c6dbdcfbdbe28c73e86cafc5287fa13d4f51fdfdfad7b51b8936d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17423853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3acb342ef8cbce6055e45fdabe7e8b60e98cab9d0aa967e362098333633440ff`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:39:01 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 00:39:02 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 00:39:03 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 00:39:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 00:39:05 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 00:39:05 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 00:39:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 00:39:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 00:39:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 00:39:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 80
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 443
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 00:39:06 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 00:39:06 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 00:39:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc24e4ccf558b6e992efaaa7a735322be11fe99ce19e722eee6ae70bb76515d`  
		Last Modified: Fri, 01 Dec 2023 00:39:21 GMT  
		Size: 347.6 KB (347632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cd6f3873930f7c6aa4ee5d06ef24c77a840fec6f0211e9572fbe0f43c04e1f`  
		Last Modified: Fri, 01 Dec 2023 00:39:21 GMT  
		Size: 7.5 KB (7508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c51a919a8bb024456b258f25a71adb53a14e30c7134e81fac343c44dbf7230c`  
		Last Modified: Fri, 01 Dec 2023 00:39:23 GMT  
		Size: 13.9 MB (13921843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:c3be58f3d1b5614d2a5e7bff50bc07567044bb119ec0f286c94df8169efc313b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17156415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194c773f5747022fdb5fc8d32e8dafcafd61f37e52238ad53627e3309c2fb4cb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:19:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 03:19:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 03:19:15 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 03:19:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 03:19:19 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 03:19:19 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 03:19:20 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 03:19:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 03:19:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 03:19:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 03:19:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 03:19:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 03:19:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 03:19:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 03:19:22 GMT
EXPOSE 80
# Fri, 01 Dec 2023 03:19:22 GMT
EXPOSE 443
# Fri, 01 Dec 2023 03:19:23 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 03:19:23 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 03:19:23 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 03:19:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803b34e1f84b29ca968d2fbf85c278608566c34dfd1742e088c6483685957029`  
		Last Modified: Fri, 01 Dec 2023 03:19:48 GMT  
		Size: 344.5 KB (344464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bbcb291a405e073d645e52039b6f84fa5071645ceb53988f99d384fbc6c4c1`  
		Last Modified: Fri, 01 Dec 2023 03:19:48 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d0aed5710d79e6bba64ce3cf139d40c4e2c3003d1feec3776b18919e3a1423`  
		Last Modified: Fri, 01 Dec 2023 03:19:50 GMT  
		Size: 13.9 MB (13903440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e7f68eb0f76a55ada8be1bb5213e5bbbcb0727fa8d4051f6f3edf1275bc2dc40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17274998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9487e6591f483b0f0d5fe25a89d069485fa10bb97a06ef07085f28b86995977c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 03:11:08 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 03:11:09 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 03:11:10 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 03:11:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 03:11:11 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 03:11:11 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 03:11:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 80
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 443
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 03:11:12 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 03:11:12 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 03:11:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e383270d6915b6b427f49a75d657d5a0403fcd47a5f89cd30e85143ca54c22`  
		Last Modified: Fri, 01 Dec 2023 03:11:28 GMT  
		Size: 360.7 KB (360655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27e927f808292c7b306432ed3ee61ecc6b7f637b8ccbdf5cb2d6bdc24649858`  
		Last Modified: Fri, 01 Dec 2023 03:11:28 GMT  
		Size: 7.5 KB (7506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dab02cb145c1d5336977666f796446f69abbbfa721ab7a71525867eb3edfbc`  
		Last Modified: Fri, 01 Dec 2023 03:11:30 GMT  
		Size: 13.6 MB (13573804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:3f9f202dc07f3bb097e0e78330d59f52c488ff4ba3b4aa4a569f1a28c9db95f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.1 MB (17058981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:126d26f69982d49f88bac36f166a92d251494018b25e2e255972b98f38f495f8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:42:19 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 05:42:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 05:42:52 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 05:42:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 05:43:00 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 05:43:20 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 05:43:24 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 05:43:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 05:43:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 05:43:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 05:43:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 05:43:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 05:43:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 05:43:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 05:43:45 GMT
EXPOSE 80
# Fri, 01 Dec 2023 05:43:46 GMT
EXPOSE 443
# Fri, 01 Dec 2023 05:43:46 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 05:43:47 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 05:43:48 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 05:43:49 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce4bc2907f69809c3086f118895d7e5c8683349557239c0ce79dfbda0ce3768`  
		Last Modified: Fri, 01 Dec 2023 05:44:17 GMT  
		Size: 362.2 KB (362185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef8889b660799cb5b3c54f8771b4a37ad12c12f245aa74e4af501a899449137`  
		Last Modified: Fri, 01 Dec 2023 05:44:17 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681f2bb9965ff577316200c634bfb7e7db0d5b2ba971441db97e1405e3c0fc6b`  
		Last Modified: Fri, 01 Dec 2023 05:44:19 GMT  
		Size: 13.3 MB (13340969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:159a339dbc4d0e8279faad422e0a871d82adcc6736b9c4ac4c4b252c3dbee6a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.8 MB (17825031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0c61727c246c9eedd4c40bc927993a89531560cc027902c6f00b8f288f96b77`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:22:31 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 01 Dec 2023 08:22:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Fri, 01 Dec 2023 08:22:32 GMT
ENV CADDY_VERSION=v2.7.5
# Fri, 01 Dec 2023 08:22:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4afdf50ccf3a8f32344dbac46006ca2b5d90c2ef656c53e8617f1c3b81c5f9e44bd3a9e0b62975f73c85451c354d3d9b5292f5247d18a62d95ab19c8b0a5dba7' ;; 		armhf)   binArch='armv6'; checksum='5f47b4ff5d290799bba1b9183c6ddfe7fee69c8086375337a7498717ce09fc627845f6cb466840daf539c763979ab60fe229b9ddeaf7f92fad800742d4ad5b3a' ;; 		armv7)   binArch='armv7'; checksum='bdd120779427cf288a383ecf9d63fa6b61e2118f189e02263ad45989bae507ce1db84ced60de3b33653e9729166e4ca436785503558955b9934be69138184055' ;; 		aarch64) binArch='arm64'; checksum='a857cbe25bcc5402e9c4fa2a6c36338f91b7e23962beedccd32e10b3aa34dda084ae742c79085d6e7581acfe33f7c9cf161224b1e56cdb661ebfb6f7424b8d0a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='72c66d44cfc8f8d248e04f08903866d62a0e11c36b51c49c08c73c833a3f4322a780405543e721dcf375b71dee06e90230c64141efb2a9614f551e2134f120a9' ;; 		s390x)   binArch='s390x'; checksum='5fb95fb495da282330f34b7f23fff3e664638397dcde2c33a3c7450e448154425b2514573604be3cac03d30b37444c4866170f232f14a33e50bff0d1e1abf126' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 01 Dec 2023 08:22:37 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 01 Dec 2023 08:22:37 GMT
ENV XDG_DATA_HOME=/data
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 01 Dec 2023 08:22:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 01 Dec 2023 08:22:38 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 01 Dec 2023 08:22:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 80
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 443
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 443/udp
# Fri, 01 Dec 2023 08:22:38 GMT
EXPOSE 2019
# Fri, 01 Dec 2023 08:22:38 GMT
WORKDIR /srv
# Fri, 01 Dec 2023 08:22:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20bbe0abb0a3f63718aa78742832077ad86b8ae86d70ce3ebcece342ec022c6`  
		Last Modified: Fri, 01 Dec 2023 08:23:07 GMT  
		Size: 354.9 KB (354948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1497491e477a92a5e82d0d68588396a3414c6e703fdc68c82c768ad6b18b28`  
		Last Modified: Fri, 01 Dec 2023 08:23:07 GMT  
		Size: 7.5 KB (7502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539ac3a1bb2d355499d388b4de966f9148263d5603f2db92aeba42084d02b3cf`  
		Last Modified: Fri, 01 Dec 2023 08:23:09 GMT  
		Size: 14.2 MB (14245127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:38df49f40c98b8d866440b7fec4635fcf669f4c138fd001b95f457b42e4e2265
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2073433228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7105669fddc0d611982501b46d56df54a820ca14cd7e3a3c62c02ef1bd40fc2e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:30:07 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Nov 2023 05:30:07 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:31:22 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Nov 2023 05:31:23 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Nov 2023 05:31:24 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Nov 2023 05:31:25 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 16 Nov 2023 05:31:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Nov 2023 05:31:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Nov 2023 05:31:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Nov 2023 05:31:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Nov 2023 05:31:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Nov 2023 05:31:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Nov 2023 05:31:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Nov 2023 05:31:32 GMT
EXPOSE 80
# Thu, 16 Nov 2023 05:31:33 GMT
EXPOSE 443
# Thu, 16 Nov 2023 05:31:34 GMT
EXPOSE 443/udp
# Thu, 16 Nov 2023 05:31:35 GMT
EXPOSE 2019
# Thu, 16 Nov 2023 05:32:33 GMT
RUN caddy version
# Thu, 16 Nov 2023 05:32:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d66ae500a331057bbb6b25a0c0e5718f2491209d7330f70b1203472b199bd5b`  
		Last Modified: Thu, 16 Nov 2023 05:37:31 GMT  
		Size: 451.2 KB (451175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec48b5261067a4b4643799633487cce5b6ee11cce36314b8a6b22964fd46ba4`  
		Last Modified: Thu, 16 Nov 2023 05:37:30 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bc40730815ee35e950756a15aa93561edd0f272d34d30de69bb8d7f58b1d8e`  
		Last Modified: Thu, 16 Nov 2023 05:37:34 GMT  
		Size: 15.3 MB (15273771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfce8b69f4cadeeaa9fcc771a3a5b374fc4a3c8c41c1a42a7878c1cad861645c`  
		Last Modified: Thu, 16 Nov 2023 05:37:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdd09852c86166de537f8b5f5b78eca092cfb95e9e2e1194c84a7a05334e5c4`  
		Last Modified: Thu, 16 Nov 2023 05:37:29 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f15c2b10239537d18dc39c5208acb0c8fc7bc25d6cd95cb59ed8e8aaf8b73be`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa35da536891cce8df35bca524d15b1b7465d4fc14354a1a15a2fa39d71a4a88`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654652f0bb6c82a0e1fd51010fd587112527866df3c9748cf9ed4414e70ee612`  
		Last Modified: Thu, 16 Nov 2023 05:37:29 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0fcd5cbdfe3f968d65ba5dcece2d017de82a3a4ec737745bd5560697735689`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9396734c66d2d27545fdeb2c33a462651a3807dfcbd04b590a01ace722161a21`  
		Last Modified: Thu, 16 Nov 2023 05:37:27 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a14586579bd1d9d9a9162b0678a119c826a7be5039b5419e90b82c772b33677`  
		Last Modified: Thu, 16 Nov 2023 05:37:27 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c773c8968545d0fca628d03a3b588ca4798423090cadd666d023cee5065235a5`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce86207f89519b9df4526afc22e743fef4a6266614fb8e082e975bf0f01862f`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7392ec7da7419f69c0413116467249934c403f42b53ff6090608481e1ba7985a`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73d1eee374e37176384bade9abdbe65d5aed23b976c507b3b88b17c758761f`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d556f28b534238f3c8497a928caa36428f1d333a69cabf15b4fc3d80aa7f3f9f`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd0eba7ede6da63115506e40bf2b6990915e5fba916e919c6525f447018bbd9`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf5b269f798b76bfba9ad2e27b5aab7bebe448007c818230643c16d6cf761af`  
		Last Modified: Thu, 16 Nov 2023 05:37:25 GMT  
		Size: 252.7 KB (252713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c70c9a3deaf4a41d4192a9248f3fd5ccfadb54792687f31f63a17f46e5134c`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:7a86ad9fb59b43cc97f50c3516b4153bb228276c026e4c802c4a213b0fe1c20f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1902803411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03625f7f4ec599de5399e0e9d5f36d3c2052adeb06f8349ef7a96e3777ddf4e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 09 Nov 2023 06:47:20 GMT
RUN Install update 10.0.20348.2113
# Thu, 16 Nov 2023 01:36:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:33:15 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Nov 2023 05:33:16 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:33:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Nov 2023 05:33:45 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Nov 2023 05:33:46 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Nov 2023 05:33:47 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 16 Nov 2023 05:33:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Nov 2023 05:33:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Nov 2023 05:33:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Nov 2023 05:33:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Nov 2023 05:33:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Nov 2023 05:33:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Nov 2023 05:33:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Nov 2023 05:33:54 GMT
EXPOSE 80
# Thu, 16 Nov 2023 05:33:55 GMT
EXPOSE 443
# Thu, 16 Nov 2023 05:33:56 GMT
EXPOSE 443/udp
# Thu, 16 Nov 2023 05:33:57 GMT
EXPOSE 2019
# Thu, 16 Nov 2023 05:34:33 GMT
RUN caddy version
# Thu, 16 Nov 2023 05:34:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7989ef2c4cfb06d845746a3c3660481ea84d3f5c8216041855ce528f0ac4015c`  
		Last Modified: Tue, 14 Nov 2023 20:43:13 GMT  
		Size: 498.2 MB (498182566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbeb193d02c2ca7f9a9ea438fbf1bcdb6ea4a6fea626713330fd1ebb514424f`  
		Last Modified: Thu, 16 Nov 2023 02:25:14 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b269b5ac8d8c6baa501ca9b38fa715170022416aa7332a2d155a06529882b84a`  
		Last Modified: Thu, 16 Nov 2023 05:37:59 GMT  
		Size: 458.2 KB (458201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f982a236809063ef75b5db6a226207448d936d7791ede196115611649805c5`  
		Last Modified: Thu, 16 Nov 2023 05:37:58 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2783cb5dad5df996a48a9ebf989a6136c91f524f421bfff9e71ab764da46fd04`  
		Last Modified: Thu, 16 Nov 2023 05:38:01 GMT  
		Size: 15.3 MB (15269735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa26255a8f194a0aa31a8fd0c48e7dfba117358880abeaf7ad3c5f54a6be87d`  
		Last Modified: Thu, 16 Nov 2023 05:37:57 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706b8120af6e900b1d0dea48743c4fd50b63c785dbe02b5ccd4af53e68ebefff`  
		Last Modified: Thu, 16 Nov 2023 05:37:57 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c12376eb1027b4892f92b1b8dd45b1e05d78f365c2886ded9202ffbaab80e9`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a29b9f98e523c3477366f98e560b8638fb5c3f0a7a8c76c9a417a33b4d44804`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a9a2fb5b49cb3e38b64f06a755f57ec37b8b5eaf2152fe9e38ae9c8cb3b593`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53a0ea77b4fcc256276d31401de856267c72aeac7fefeeb6fbe655340bb4cf4`  
		Last Modified: Thu, 16 Nov 2023 05:37:55 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d80b783b85d05309ef9fe97740b873bd9092c13b53eea3d83adf6197cbe798`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9454c6602eef29f64927e75d96b8f26d7cf0c6c089afa91e260207675216501`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f23d9fc021e786b83141dd57c2a10dc279d17eacad254ec81d7922372d17876`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55a4267cea49483a79cbee8908d3daf6af4fb6fa1af94e350072034f128c5a1`  
		Last Modified: Thu, 16 Nov 2023 05:37:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9723590c56e28022e6ee055495ee5826c7ea085d2a8b7255d471b35bb27e9a6c`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b39c632f1f53a232721260e3ebcc755559883edb0272949f2d965799d62ef5`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3deb93ce29c0157e6c6b82bbad0ffb2102a833ea54672c93c05843899eac3bc`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09fe12ffad65804e54e566d7b3256d98268c5e943a40282d44bab50d3fb6a04`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517e7fd42cd9750ca7ef5a68df02e2bdc3be404dbd69681f36c7b0acb1562550`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 270.1 KB (270069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0727df29cc57ce0bb7db3c73852d6eaceb439603493f2e3ceb07ce2f8e8e4e99`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:b2a860f9d095b10b5613cfd76162decff7840f5881e3c5ecf4e01d29d829c405
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.5122; amd64
	-	windows version 10.0.20348.2113; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:38df49f40c98b8d866440b7fec4635fcf669f4c138fd001b95f457b42e4e2265
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2073433228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7105669fddc0d611982501b46d56df54a820ca14cd7e3a3c62c02ef1bd40fc2e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:30:07 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Nov 2023 05:30:07 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:31:22 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Nov 2023 05:31:23 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Nov 2023 05:31:24 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Nov 2023 05:31:25 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 16 Nov 2023 05:31:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Nov 2023 05:31:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Nov 2023 05:31:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Nov 2023 05:31:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Nov 2023 05:31:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Nov 2023 05:31:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Nov 2023 05:31:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Nov 2023 05:31:32 GMT
EXPOSE 80
# Thu, 16 Nov 2023 05:31:33 GMT
EXPOSE 443
# Thu, 16 Nov 2023 05:31:34 GMT
EXPOSE 443/udp
# Thu, 16 Nov 2023 05:31:35 GMT
EXPOSE 2019
# Thu, 16 Nov 2023 05:32:33 GMT
RUN caddy version
# Thu, 16 Nov 2023 05:32:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d66ae500a331057bbb6b25a0c0e5718f2491209d7330f70b1203472b199bd5b`  
		Last Modified: Thu, 16 Nov 2023 05:37:31 GMT  
		Size: 451.2 KB (451175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec48b5261067a4b4643799633487cce5b6ee11cce36314b8a6b22964fd46ba4`  
		Last Modified: Thu, 16 Nov 2023 05:37:30 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bc40730815ee35e950756a15aa93561edd0f272d34d30de69bb8d7f58b1d8e`  
		Last Modified: Thu, 16 Nov 2023 05:37:34 GMT  
		Size: 15.3 MB (15273771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfce8b69f4cadeeaa9fcc771a3a5b374fc4a3c8c41c1a42a7878c1cad861645c`  
		Last Modified: Thu, 16 Nov 2023 05:37:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdd09852c86166de537f8b5f5b78eca092cfb95e9e2e1194c84a7a05334e5c4`  
		Last Modified: Thu, 16 Nov 2023 05:37:29 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f15c2b10239537d18dc39c5208acb0c8fc7bc25d6cd95cb59ed8e8aaf8b73be`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa35da536891cce8df35bca524d15b1b7465d4fc14354a1a15a2fa39d71a4a88`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654652f0bb6c82a0e1fd51010fd587112527866df3c9748cf9ed4414e70ee612`  
		Last Modified: Thu, 16 Nov 2023 05:37:29 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0fcd5cbdfe3f968d65ba5dcece2d017de82a3a4ec737745bd5560697735689`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9396734c66d2d27545fdeb2c33a462651a3807dfcbd04b590a01ace722161a21`  
		Last Modified: Thu, 16 Nov 2023 05:37:27 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a14586579bd1d9d9a9162b0678a119c826a7be5039b5419e90b82c772b33677`  
		Last Modified: Thu, 16 Nov 2023 05:37:27 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c773c8968545d0fca628d03a3b588ca4798423090cadd666d023cee5065235a5`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce86207f89519b9df4526afc22e743fef4a6266614fb8e082e975bf0f01862f`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7392ec7da7419f69c0413116467249934c403f42b53ff6090608481e1ba7985a`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73d1eee374e37176384bade9abdbe65d5aed23b976c507b3b88b17c758761f`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d556f28b534238f3c8497a928caa36428f1d333a69cabf15b4fc3d80aa7f3f9f`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd0eba7ede6da63115506e40bf2b6990915e5fba916e919c6525f447018bbd9`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf5b269f798b76bfba9ad2e27b5aab7bebe448007c818230643c16d6cf761af`  
		Last Modified: Thu, 16 Nov 2023 05:37:25 GMT  
		Size: 252.7 KB (252713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c70c9a3deaf4a41d4192a9248f3fd5ccfadb54792687f31f63a17f46e5134c`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:7a86ad9fb59b43cc97f50c3516b4153bb228276c026e4c802c4a213b0fe1c20f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1902803411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03625f7f4ec599de5399e0e9d5f36d3c2052adeb06f8349ef7a96e3777ddf4e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 09 Nov 2023 06:47:20 GMT
RUN Install update 10.0.20348.2113
# Thu, 16 Nov 2023 01:36:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:33:15 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Nov 2023 05:33:16 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:33:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Nov 2023 05:33:45 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Nov 2023 05:33:46 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Nov 2023 05:33:47 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 16 Nov 2023 05:33:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Nov 2023 05:33:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Nov 2023 05:33:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Nov 2023 05:33:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Nov 2023 05:33:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Nov 2023 05:33:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Nov 2023 05:33:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Nov 2023 05:33:54 GMT
EXPOSE 80
# Thu, 16 Nov 2023 05:33:55 GMT
EXPOSE 443
# Thu, 16 Nov 2023 05:33:56 GMT
EXPOSE 443/udp
# Thu, 16 Nov 2023 05:33:57 GMT
EXPOSE 2019
# Thu, 16 Nov 2023 05:34:33 GMT
RUN caddy version
# Thu, 16 Nov 2023 05:34:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7989ef2c4cfb06d845746a3c3660481ea84d3f5c8216041855ce528f0ac4015c`  
		Last Modified: Tue, 14 Nov 2023 20:43:13 GMT  
		Size: 498.2 MB (498182566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbeb193d02c2ca7f9a9ea438fbf1bcdb6ea4a6fea626713330fd1ebb514424f`  
		Last Modified: Thu, 16 Nov 2023 02:25:14 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b269b5ac8d8c6baa501ca9b38fa715170022416aa7332a2d155a06529882b84a`  
		Last Modified: Thu, 16 Nov 2023 05:37:59 GMT  
		Size: 458.2 KB (458201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f982a236809063ef75b5db6a226207448d936d7791ede196115611649805c5`  
		Last Modified: Thu, 16 Nov 2023 05:37:58 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2783cb5dad5df996a48a9ebf989a6136c91f524f421bfff9e71ab764da46fd04`  
		Last Modified: Thu, 16 Nov 2023 05:38:01 GMT  
		Size: 15.3 MB (15269735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa26255a8f194a0aa31a8fd0c48e7dfba117358880abeaf7ad3c5f54a6be87d`  
		Last Modified: Thu, 16 Nov 2023 05:37:57 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706b8120af6e900b1d0dea48743c4fd50b63c785dbe02b5ccd4af53e68ebefff`  
		Last Modified: Thu, 16 Nov 2023 05:37:57 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c12376eb1027b4892f92b1b8dd45b1e05d78f365c2886ded9202ffbaab80e9`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a29b9f98e523c3477366f98e560b8638fb5c3f0a7a8c76c9a417a33b4d44804`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a9a2fb5b49cb3e38b64f06a755f57ec37b8b5eaf2152fe9e38ae9c8cb3b593`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53a0ea77b4fcc256276d31401de856267c72aeac7fefeeb6fbe655340bb4cf4`  
		Last Modified: Thu, 16 Nov 2023 05:37:55 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d80b783b85d05309ef9fe97740b873bd9092c13b53eea3d83adf6197cbe798`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9454c6602eef29f64927e75d96b8f26d7cf0c6c089afa91e260207675216501`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f23d9fc021e786b83141dd57c2a10dc279d17eacad254ec81d7922372d17876`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55a4267cea49483a79cbee8908d3daf6af4fb6fa1af94e350072034f128c5a1`  
		Last Modified: Thu, 16 Nov 2023 05:37:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9723590c56e28022e6ee055495ee5826c7ea085d2a8b7255d471b35bb27e9a6c`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b39c632f1f53a232721260e3ebcc755559883edb0272949f2d965799d62ef5`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3deb93ce29c0157e6c6b82bbad0ffb2102a833ea54672c93c05843899eac3bc`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09fe12ffad65804e54e566d7b3256d98268c5e943a40282d44bab50d3fb6a04`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517e7fd42cd9750ca7ef5a68df02e2bdc3be404dbd69681f36c7b0acb1562550`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 270.1 KB (270069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0727df29cc57ce0bb7db3c73852d6eaceb439603493f2e3ceb07ce2f8e8e4e99`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:2e8fbf0e299d85c14b2ac578c2ff6ee6f32e2e0c7dbd4afd5f683286575971d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:38df49f40c98b8d866440b7fec4635fcf669f4c138fd001b95f457b42e4e2265
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2073433228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7105669fddc0d611982501b46d56df54a820ca14cd7e3a3c62c02ef1bd40fc2e`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:30:07 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Nov 2023 05:30:07 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:31:22 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Nov 2023 05:31:23 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Nov 2023 05:31:24 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Nov 2023 05:31:25 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 16 Nov 2023 05:31:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Nov 2023 05:31:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Nov 2023 05:31:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Nov 2023 05:31:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Nov 2023 05:31:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Nov 2023 05:31:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Nov 2023 05:31:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Nov 2023 05:31:32 GMT
EXPOSE 80
# Thu, 16 Nov 2023 05:31:33 GMT
EXPOSE 443
# Thu, 16 Nov 2023 05:31:34 GMT
EXPOSE 443/udp
# Thu, 16 Nov 2023 05:31:35 GMT
EXPOSE 2019
# Thu, 16 Nov 2023 05:32:33 GMT
RUN caddy version
# Thu, 16 Nov 2023 05:32:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d66ae500a331057bbb6b25a0c0e5718f2491209d7330f70b1203472b199bd5b`  
		Last Modified: Thu, 16 Nov 2023 05:37:31 GMT  
		Size: 451.2 KB (451175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec48b5261067a4b4643799633487cce5b6ee11cce36314b8a6b22964fd46ba4`  
		Last Modified: Thu, 16 Nov 2023 05:37:30 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bc40730815ee35e950756a15aa93561edd0f272d34d30de69bb8d7f58b1d8e`  
		Last Modified: Thu, 16 Nov 2023 05:37:34 GMT  
		Size: 15.3 MB (15273771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfce8b69f4cadeeaa9fcc771a3a5b374fc4a3c8c41c1a42a7878c1cad861645c`  
		Last Modified: Thu, 16 Nov 2023 05:37:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdd09852c86166de537f8b5f5b78eca092cfb95e9e2e1194c84a7a05334e5c4`  
		Last Modified: Thu, 16 Nov 2023 05:37:29 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f15c2b10239537d18dc39c5208acb0c8fc7bc25d6cd95cb59ed8e8aaf8b73be`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa35da536891cce8df35bca524d15b1b7465d4fc14354a1a15a2fa39d71a4a88`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654652f0bb6c82a0e1fd51010fd587112527866df3c9748cf9ed4414e70ee612`  
		Last Modified: Thu, 16 Nov 2023 05:37:29 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0fcd5cbdfe3f968d65ba5dcece2d017de82a3a4ec737745bd5560697735689`  
		Last Modified: Thu, 16 Nov 2023 05:37:28 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9396734c66d2d27545fdeb2c33a462651a3807dfcbd04b590a01ace722161a21`  
		Last Modified: Thu, 16 Nov 2023 05:37:27 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a14586579bd1d9d9a9162b0678a119c826a7be5039b5419e90b82c772b33677`  
		Last Modified: Thu, 16 Nov 2023 05:37:27 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c773c8968545d0fca628d03a3b588ca4798423090cadd666d023cee5065235a5`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce86207f89519b9df4526afc22e743fef4a6266614fb8e082e975bf0f01862f`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7392ec7da7419f69c0413116467249934c403f42b53ff6090608481e1ba7985a`  
		Last Modified: Thu, 16 Nov 2023 05:37:26 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73d1eee374e37176384bade9abdbe65d5aed23b976c507b3b88b17c758761f`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d556f28b534238f3c8497a928caa36428f1d333a69cabf15b4fc3d80aa7f3f9f`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd0eba7ede6da63115506e40bf2b6990915e5fba916e919c6525f447018bbd9`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf5b269f798b76bfba9ad2e27b5aab7bebe448007c818230643c16d6cf761af`  
		Last Modified: Thu, 16 Nov 2023 05:37:25 GMT  
		Size: 252.7 KB (252713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c70c9a3deaf4a41d4192a9248f3fd5ccfadb54792687f31f63a17f46e5134c`  
		Last Modified: Thu, 16 Nov 2023 05:37:24 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:7302fa54b56c8f2363f0caf1ac496c297c9eda88207a05836e5e06c40272769b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2113; amd64

### `caddy:windowsservercore-ltsc2022` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:7a86ad9fb59b43cc97f50c3516b4153bb228276c026e4c802c4a213b0fe1c20f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1902803411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03625f7f4ec599de5399e0e9d5f36d3c2052adeb06f8349ef7a96e3777ddf4e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 09 Nov 2023 06:47:20 GMT
RUN Install update 10.0.20348.2113
# Thu, 16 Nov 2023 01:36:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:33:15 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Nov 2023 05:33:16 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:33:44 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.5/caddy_2.7.5_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3201e91a00d8c49acf6165753df34fccfb9c0eacb610b0dad5e5c465cdaced761b061f0c7fc200ce4e87f4acfbd6421e9b3e0121ba293532f4afdf7c9c9c96a0')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Nov 2023 05:33:45 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Nov 2023 05:33:46 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Nov 2023 05:33:47 GMT
LABEL org.opencontainers.image.version=v2.7.5
# Thu, 16 Nov 2023 05:33:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Nov 2023 05:33:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Nov 2023 05:33:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Nov 2023 05:33:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Nov 2023 05:33:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Nov 2023 05:33:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Nov 2023 05:33:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Nov 2023 05:33:54 GMT
EXPOSE 80
# Thu, 16 Nov 2023 05:33:55 GMT
EXPOSE 443
# Thu, 16 Nov 2023 05:33:56 GMT
EXPOSE 443/udp
# Thu, 16 Nov 2023 05:33:57 GMT
EXPOSE 2019
# Thu, 16 Nov 2023 05:34:33 GMT
RUN caddy version
# Thu, 16 Nov 2023 05:34:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7989ef2c4cfb06d845746a3c3660481ea84d3f5c8216041855ce528f0ac4015c`  
		Last Modified: Tue, 14 Nov 2023 20:43:13 GMT  
		Size: 498.2 MB (498182566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbeb193d02c2ca7f9a9ea438fbf1bcdb6ea4a6fea626713330fd1ebb514424f`  
		Last Modified: Thu, 16 Nov 2023 02:25:14 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b269b5ac8d8c6baa501ca9b38fa715170022416aa7332a2d155a06529882b84a`  
		Last Modified: Thu, 16 Nov 2023 05:37:59 GMT  
		Size: 458.2 KB (458201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f982a236809063ef75b5db6a226207448d936d7791ede196115611649805c5`  
		Last Modified: Thu, 16 Nov 2023 05:37:58 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2783cb5dad5df996a48a9ebf989a6136c91f524f421bfff9e71ab764da46fd04`  
		Last Modified: Thu, 16 Nov 2023 05:38:01 GMT  
		Size: 15.3 MB (15269735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa26255a8f194a0aa31a8fd0c48e7dfba117358880abeaf7ad3c5f54a6be87d`  
		Last Modified: Thu, 16 Nov 2023 05:37:57 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706b8120af6e900b1d0dea48743c4fd50b63c785dbe02b5ccd4af53e68ebefff`  
		Last Modified: Thu, 16 Nov 2023 05:37:57 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c12376eb1027b4892f92b1b8dd45b1e05d78f365c2886ded9202ffbaab80e9`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a29b9f98e523c3477366f98e560b8638fb5c3f0a7a8c76c9a417a33b4d44804`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a9a2fb5b49cb3e38b64f06a755f57ec37b8b5eaf2152fe9e38ae9c8cb3b593`  
		Last Modified: Thu, 16 Nov 2023 05:37:56 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53a0ea77b4fcc256276d31401de856267c72aeac7fefeeb6fbe655340bb4cf4`  
		Last Modified: Thu, 16 Nov 2023 05:37:55 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d80b783b85d05309ef9fe97740b873bd9092c13b53eea3d83adf6197cbe798`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9454c6602eef29f64927e75d96b8f26d7cf0c6c089afa91e260207675216501`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f23d9fc021e786b83141dd57c2a10dc279d17eacad254ec81d7922372d17876`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55a4267cea49483a79cbee8908d3daf6af4fb6fa1af94e350072034f128c5a1`  
		Last Modified: Thu, 16 Nov 2023 05:37:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9723590c56e28022e6ee055495ee5826c7ea085d2a8b7255d471b35bb27e9a6c`  
		Last Modified: Thu, 16 Nov 2023 05:37:54 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b39c632f1f53a232721260e3ebcc755559883edb0272949f2d965799d62ef5`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3deb93ce29c0157e6c6b82bbad0ffb2102a833ea54672c93c05843899eac3bc`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09fe12ffad65804e54e566d7b3256d98268c5e943a40282d44bab50d3fb6a04`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517e7fd42cd9750ca7ef5a68df02e2bdc3be404dbd69681f36c7b0acb1562550`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 270.1 KB (270069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0727df29cc57ce0bb7db3c73852d6eaceb439603493f2e3ceb07ce2f8e8e4e99`  
		Last Modified: Thu, 16 Nov 2023 05:37:52 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
