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
$ docker pull caddy@sha256:279a5ff568ff6c9e6185a6151e065aacb01c0f275b85f52dd950ac9ae204d8ab
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
$ docker pull caddy@sha256:8e3595ce7a7ebd91a4e91eb41ee367a10e18eb9a711fb28e47f611a7882b3dcc
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
$ docker pull caddy@sha256:5b9c67db8969d2d07fbbea52156ed4a9d59c6b20452e5f230c230a686b60c426
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
$ docker pull caddy@sha256:9557c75b38fa3d68dee8dc5098bacb77894db187429baffcf2028f41edd5686e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76955142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70f74c1f483f810509bfd9c4187e0a600e5a9e8aa2ca801acd27e9cc06aa8d2e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:10:40 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 18:05:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:20:24 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:20:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:20:35 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:20:35 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:20:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:20:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:20:36 GMT
WORKDIR /go
# Tue, 07 Nov 2023 20:44:48 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 20:44:48 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 20:44:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 20:44:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 20:44:50 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834bccaa730c985b202b64916ba9cbab707b8a165cece04b8aea3801d6a75741`  
		Last Modified: Sat, 21 Oct 2023 03:10:51 GMT  
		Size: 284.7 KB (284695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bde6e5b785726fea08cb0fb123a90298ceca5cbdc7f267aec8af550c401a2f6`  
		Last Modified: Tue, 07 Nov 2023 20:26:52 GMT  
		Size: 67.0 MB (66995661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebe3be3b56eef1186e8ed89cfaaacf25685600944b44bcdbbd57eb8c8d188e4`  
		Last Modified: Tue, 07 Nov 2023 20:26:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2104133a0e423dca65ea3889907e07d16f2aee507a0b4e6c113befd233f3376e`  
		Last Modified: Tue, 07 Nov 2023 20:45:08 GMT  
		Size: 5.0 MB (4970027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3223ac085d84a7150dcade2bc8258b726591b749677608a2b7e3a02664a48ba5`  
		Last Modified: Tue, 07 Nov 2023 20:45:07 GMT  
		Size: 1.3 MB (1302232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3306c1ee0dab13ecea29b0e17a898223583940e47acc99449853e9e59435f3`  
		Last Modified: Tue, 07 Nov 2023 20:45:07 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:925051dfec44d86d69116ecf542f98f048d16edc30ee04e84dd0f94b8a306f28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75395073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:337623b638f4d83149457aa62bc5b13dff2de821cac1d7a7deb4b0eba81c383c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:43:17 GMT
RUN apk add --no-cache ca-certificates
# Tue, 07 Nov 2023 20:49:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:49:19 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:49:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:49:36 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:49:36 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:49:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:49:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:49:37 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:12:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:12:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:12:40 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:12:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:12:40 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:12:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:12:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:12:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4459abd186485ffcfbc9a0cc16ba7fc77e7b8af5dd55624328e90ec67ef669`  
		Last Modified: Sat, 21 Oct 2023 00:43:27 GMT  
		Size: 284.9 KB (284882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e47353e44109dd9c41cf34c24ec76dc67e7767decf78622589a90a58c3b2f4`  
		Last Modified: Tue, 07 Nov 2023 20:55:24 GMT  
		Size: 65.8 MB (65751371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed03a7f93d0719301c31ce952f21b9a5a31d7a50775d4ee8bc1070f1ce19f9f`  
		Last Modified: Tue, 07 Nov 2023 20:55:04 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c4b96bb9b7fb0e5321265d67484456c37c1fbd1d5e2565c4f9225f9989acaf`  
		Last Modified: Tue, 07 Nov 2023 21:13:02 GMT  
		Size: 5.0 MB (4964302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82c013a69236b77e239aa51756075002025bfab6a1124e524c8c4f855b72142`  
		Last Modified: Tue, 07 Nov 2023 21:13:02 GMT  
		Size: 1.2 MB (1248664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856961b563a2d5414382e81b6e6a0f242bf2a09bb03623ff004cc79275c9b02c`  
		Last Modified: Tue, 07 Nov 2023 21:13:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:c3408f987d7ee9eedb1a5fcefc1cdf4b24092224fdc2d91a0aae5e4b0ad1e1f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74692592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7150e3216cb69f9c924809d80e3f784b9e25038c5c743f8e415853df8163fd0`
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
# Tue, 07 Nov 2023 21:00:37 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 21:00:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 21:00:51 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 21:00:51 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 21:00:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:00:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 21:00:52 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:25:34 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:25:34 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:25:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:25:36 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:25:36 GMT
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
	-	`sha256:4a3debef18506403ac44cc4950a8cbaaea2e9d311ae1a83607be6f7b78b291ce`  
		Last Modified: Tue, 07 Nov 2023 21:07:30 GMT  
		Size: 65.8 MB (65750717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce90421070593b8c5625d529316d162aac0bcfd55fc9e7507b337aed33c64191`  
		Last Modified: Tue, 07 Nov 2023 21:07:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc6fcb2c4fc6a718864e032be82c1edac9d3564e3b7a5833d5f1c1879365074`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 4.5 MB (4511246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91736d5dba9b84ca32af89f184018cf79348d96d127c913d2721ef9a62c5031`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 1.2 MB (1246088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc61b28fe019881fc188747ffde817dc4796c027b44cb91541a4cb9b08714cf`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b843e7253f9266dbfe42a8aa6ed190a23d4c10856ea0ab900fba06faf579e47f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73974255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b375a225af66400861808f202e662bafd23e07644f836d4e47c6d399b765686d`
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
# Tue, 07 Nov 2023 20:39:55 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:40:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:40:05 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:40:05 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:40:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:40:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:40:06 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:02:44 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:02:44 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:02:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:02:45 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:02:45 GMT
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
	-	`sha256:f9e3860c59e00c3164218e7e9c694435e2bcaaf14693bbc68c2a02a882bcc6a2`  
		Last Modified: Tue, 07 Nov 2023 20:45:13 GMT  
		Size: 64.1 MB (64088686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e79fdc38632695ae6832600d13ce667f701f785944433806d5fbf89a90b675`  
		Last Modified: Tue, 07 Nov 2023 20:45:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f0a09267a67162a19517c78b4e687814d8f7b56bd3f768cada6f09460a11c6`  
		Last Modified: Tue, 07 Nov 2023 21:03:01 GMT  
		Size: 5.1 MB (5068431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5a0da72908eb54180139e187b047089c01454fc561d10071e004ddddbc83b7`  
		Last Modified: Tue, 07 Nov 2023 21:03:01 GMT  
		Size: 1.2 MB (1198449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c321b6ea80f52f37c190337f940f0c24d98385d9a2311b30680a11ff757a30f`  
		Last Modified: Tue, 07 Nov 2023 21:03:00 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:4206943b7073e21d109937a4da710faadb4c2d68b06eed13cca7a2e81a427ed0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74200658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ad7628f7abe471737f92d250481b6d37b0dbc08b27f4fecd6de4b7069255fce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:50:06 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 13:54:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:17:41 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 21:18:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 21:18:05 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 21:18:06 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 21:18:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:18:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 21:18:08 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:43:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:43:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:43:40 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:43:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:43:41 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:43:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:43:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:43:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ea699c459f4e83d317f31dad3d23c45cc29bbd728f76aa22bd9e4a8180feb8`  
		Last Modified: Sat, 21 Oct 2023 00:50:20 GMT  
		Size: 286.7 KB (286665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f7b3697956c8adf732de1fa607b670ec20dad24d26aa13bdfd9b275c65ab7e`  
		Last Modified: Tue, 07 Nov 2023 21:25:46 GMT  
		Size: 64.1 MB (64111773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f1720227a74244550a3b19be823a0538279f71347eea9e055bc39b87306e09`  
		Last Modified: Tue, 07 Nov 2023 21:25:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5aa813cd8b314d1ecc000832dd9d9a65d87b48fe12a3e26e8973a24739e1e5d`  
		Last Modified: Tue, 07 Nov 2023 21:44:02 GMT  
		Size: 5.3 MB (5268975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526c725b224548c8658f358c73e89e88e8e4ed758879e446da57649f8147caa3`  
		Last Modified: Tue, 07 Nov 2023 21:44:01 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5ec0b117cae64f834ae1c8a5f1c6e2eb7d03ed218ac12f9e531fb65d2749ae`  
		Last Modified: Tue, 07 Nov 2023 21:44:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:01d8af8337066c19a93a4af95f039f93092c42c25958cb75f773287862af55fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76087350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45f25b6ed469e7fd4e3d10476165542d74cc1ff9aa294642362d158ea159c841`
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
# Tue, 07 Nov 2023 20:43:18 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:43:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:43:36 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:43:36 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:43:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:43:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:43:37 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:08:19 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:08:19 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:08:20 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:08:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:08:20 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:08:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:08:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:08:21 GMT
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
	-	`sha256:72d99582ceb0709a8c9a1d5fdc62f431b171ef30aafa94a2f14cdc818695abc2`  
		Last Modified: Tue, 07 Nov 2023 20:50:45 GMT  
		Size: 66.2 MB (66209518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd3acc2cfafbeca6b9582dca1e5dca9862e6059e686d6fd717790f4353277cf`  
		Last Modified: Tue, 07 Nov 2023 20:50:34 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad32e6427b3c189cb8976ef70af84e8e86a742134fbfcc46ce989b710509dfc`  
		Last Modified: Tue, 07 Nov 2023 21:08:48 GMT  
		Size: 5.1 MB (5114684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d837cb4f1c5fec0ee05235ea0bb20b16067e00a6f0494f88afa5fb527b5f790`  
		Last Modified: Tue, 07 Nov 2023 21:08:47 GMT  
		Size: 1.3 MB (1262388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf5bb743910ff919d1d7c652a4eeda2079fef5385f4c212839b9345c940c370`  
		Last Modified: Tue, 07 Nov 2023 21:08:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:823c52d733e025f2f7a994e81853c644a8cb7fc8e2cfaf1759cfbd9f42981bae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2154235329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e51a76e2131305dc407d432736a885084ead87fe0cc9c9a227736e6799405b0`
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
# Thu, 16 Nov 2023 02:49:42 GMT
ENV GOLANG_VERSION=1.21.4
# Thu, 16 Nov 2023 02:52:53 GMT
RUN $url = 'https://dl.google.com/go/go1.21.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '79e5428e068c912d9cfa6cd115c13549856ec689c1332eac17f5d6122e19d595'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:52:55 GMT
WORKDIR C:\go
# Thu, 16 Nov 2023 05:34:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:34:44 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 16 Nov 2023 05:34:45 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:34:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Nov 2023 05:36:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Nov 2023 05:36:01 GMT
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
	-	`sha256:c30930da8ed1e8bdc54250c940331ca68cda0bfb62284a10c659fbd0768848ea`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d113e76a38d50789cec61e62343c448b0f781f2edc2150f8abe914796df72325`  
		Last Modified: Thu, 16 Nov 2023 03:12:14 GMT  
		Size: 69.3 MB (69322889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e233c1968dbb3ae85985bbd8b98ec9454199ca20141c642a7884444c1bc7c7`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 1.6 KB (1580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be3840df58058d3a67a1f4fc3b8987c93be3fba0227a49b9ab08af23db164b3`  
		Last Modified: Thu, 16 Nov 2023 05:38:22 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64072f71e3f7e1d01b75b904e8cb73988c110ba09d61072634272c1c6e0192f5`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be28c184970d229ba318ac93ef72165a50289b21f6822ac961e779c3f7594b2`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fadbb7cc6286a3cc2b7fc543b3a14f8c4527bd76a612ec0e0f971acc57a35a48`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f55e1de34150b2a36b3073acb80b8a2be69b440782f880794957e941f29220`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.7 MB (1661568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be73ad07c8ccee0635f69cb11e8c37458731e7c8791d6b55e3c75a04b533099`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:256d98ebfd54e7da9c594d3a17888987e08a54f31e1a902fdba6062d6475e357
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1983592262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:932ff705341933569835dda3a9df0a381c9efadb23aedbc990ae4c3fe927da37`
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
# Thu, 16 Nov 2023 02:44:31 GMT
ENV GOLANG_VERSION=1.21.4
# Thu, 16 Nov 2023 02:46:51 GMT
RUN $url = 'https://dl.google.com/go/go1.21.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '79e5428e068c912d9cfa6cd115c13549856ec689c1332eac17f5d6122e19d595'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:46:53 GMT
WORKDIR C:\go
# Thu, 16 Nov 2023 05:36:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:36:15 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 16 Nov 2023 05:36:16 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:36:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Nov 2023 05:36:43 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Nov 2023 05:36:44 GMT
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
	-	`sha256:2e99ca1444cc508d00e7f114e5d0ad9c56d99298bd9767a001ab05a1735cacb4`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753e4af07bf1638babc6e18c4a455b8703dfec478e0794970b2e57d76792a281`  
		Last Modified: Thu, 16 Nov 2023 03:11:38 GMT  
		Size: 69.3 MB (69321984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ace7dc382558d5cfabba6fa5df0abb49108d5b6e7ef243a4b4ccfa7639d022`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.6 KB (1572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dee0b52088af84428a19e50ee688425ccee03091d9de2d42ab608d6f4988b90`  
		Last Modified: Thu, 16 Nov 2023 05:38:42 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae08626268dc4e22e38977aa0284b4f4e8aa2a88d8dbf3cfe61c9ffc10292d3`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12154a346b5aa10235e1da2e2c14f346f6de03387fabad1e8b0df50ce81588e5`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33ca4e95a635026944c3bc5da0516b66036a17f0f1a41f8bc2cccfd4afd1015`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37d2fb80d01142c2f56374c7be06d04ac0ddebd778ee3e052d6e627969b6af7`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.7 MB (1667548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41cc79b0b9e584ff384ef15b6bd7d7f1f12e5e73e9105b3e89537f183c38d8d`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:a51593964dcf5b43b549589e0e77d0dec7a1c3491fb5054a8e1e93e22505d1a6
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
$ docker pull caddy@sha256:9557c75b38fa3d68dee8dc5098bacb77894db187429baffcf2028f41edd5686e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76955142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70f74c1f483f810509bfd9c4187e0a600e5a9e8aa2ca801acd27e9cc06aa8d2e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:10:40 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 18:05:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:20:24 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:20:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:20:35 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:20:35 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:20:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:20:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:20:36 GMT
WORKDIR /go
# Tue, 07 Nov 2023 20:44:48 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 20:44:48 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 20:44:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 20:44:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 20:44:50 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834bccaa730c985b202b64916ba9cbab707b8a165cece04b8aea3801d6a75741`  
		Last Modified: Sat, 21 Oct 2023 03:10:51 GMT  
		Size: 284.7 KB (284695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bde6e5b785726fea08cb0fb123a90298ceca5cbdc7f267aec8af550c401a2f6`  
		Last Modified: Tue, 07 Nov 2023 20:26:52 GMT  
		Size: 67.0 MB (66995661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebe3be3b56eef1186e8ed89cfaaacf25685600944b44bcdbbd57eb8c8d188e4`  
		Last Modified: Tue, 07 Nov 2023 20:26:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2104133a0e423dca65ea3889907e07d16f2aee507a0b4e6c113befd233f3376e`  
		Last Modified: Tue, 07 Nov 2023 20:45:08 GMT  
		Size: 5.0 MB (4970027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3223ac085d84a7150dcade2bc8258b726591b749677608a2b7e3a02664a48ba5`  
		Last Modified: Tue, 07 Nov 2023 20:45:07 GMT  
		Size: 1.3 MB (1302232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3306c1ee0dab13ecea29b0e17a898223583940e47acc99449853e9e59435f3`  
		Last Modified: Tue, 07 Nov 2023 20:45:07 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:925051dfec44d86d69116ecf542f98f048d16edc30ee04e84dd0f94b8a306f28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75395073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:337623b638f4d83149457aa62bc5b13dff2de821cac1d7a7deb4b0eba81c383c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:43:17 GMT
RUN apk add --no-cache ca-certificates
# Tue, 07 Nov 2023 20:49:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:49:19 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:49:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:49:36 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:49:36 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:49:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:49:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:49:37 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:12:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:12:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:12:40 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:12:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:12:40 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:12:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:12:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:12:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4459abd186485ffcfbc9a0cc16ba7fc77e7b8af5dd55624328e90ec67ef669`  
		Last Modified: Sat, 21 Oct 2023 00:43:27 GMT  
		Size: 284.9 KB (284882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e47353e44109dd9c41cf34c24ec76dc67e7767decf78622589a90a58c3b2f4`  
		Last Modified: Tue, 07 Nov 2023 20:55:24 GMT  
		Size: 65.8 MB (65751371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed03a7f93d0719301c31ce952f21b9a5a31d7a50775d4ee8bc1070f1ce19f9f`  
		Last Modified: Tue, 07 Nov 2023 20:55:04 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c4b96bb9b7fb0e5321265d67484456c37c1fbd1d5e2565c4f9225f9989acaf`  
		Last Modified: Tue, 07 Nov 2023 21:13:02 GMT  
		Size: 5.0 MB (4964302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82c013a69236b77e239aa51756075002025bfab6a1124e524c8c4f855b72142`  
		Last Modified: Tue, 07 Nov 2023 21:13:02 GMT  
		Size: 1.2 MB (1248664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856961b563a2d5414382e81b6e6a0f242bf2a09bb03623ff004cc79275c9b02c`  
		Last Modified: Tue, 07 Nov 2023 21:13:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:c3408f987d7ee9eedb1a5fcefc1cdf4b24092224fdc2d91a0aae5e4b0ad1e1f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74692592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7150e3216cb69f9c924809d80e3f784b9e25038c5c743f8e415853df8163fd0`
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
# Tue, 07 Nov 2023 21:00:37 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 21:00:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 21:00:51 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 21:00:51 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 21:00:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:00:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 21:00:52 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:25:34 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:25:34 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:25:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:25:36 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:25:36 GMT
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
	-	`sha256:4a3debef18506403ac44cc4950a8cbaaea2e9d311ae1a83607be6f7b78b291ce`  
		Last Modified: Tue, 07 Nov 2023 21:07:30 GMT  
		Size: 65.8 MB (65750717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce90421070593b8c5625d529316d162aac0bcfd55fc9e7507b337aed33c64191`  
		Last Modified: Tue, 07 Nov 2023 21:07:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc6fcb2c4fc6a718864e032be82c1edac9d3564e3b7a5833d5f1c1879365074`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 4.5 MB (4511246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91736d5dba9b84ca32af89f184018cf79348d96d127c913d2721ef9a62c5031`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 1.2 MB (1246088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc61b28fe019881fc188747ffde817dc4796c027b44cb91541a4cb9b08714cf`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b843e7253f9266dbfe42a8aa6ed190a23d4c10856ea0ab900fba06faf579e47f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73974255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b375a225af66400861808f202e662bafd23e07644f836d4e47c6d399b765686d`
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
# Tue, 07 Nov 2023 20:39:55 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:40:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:40:05 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:40:05 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:40:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:40:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:40:06 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:02:44 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:02:44 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:02:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:02:45 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:02:45 GMT
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
	-	`sha256:f9e3860c59e00c3164218e7e9c694435e2bcaaf14693bbc68c2a02a882bcc6a2`  
		Last Modified: Tue, 07 Nov 2023 20:45:13 GMT  
		Size: 64.1 MB (64088686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e79fdc38632695ae6832600d13ce667f701f785944433806d5fbf89a90b675`  
		Last Modified: Tue, 07 Nov 2023 20:45:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f0a09267a67162a19517c78b4e687814d8f7b56bd3f768cada6f09460a11c6`  
		Last Modified: Tue, 07 Nov 2023 21:03:01 GMT  
		Size: 5.1 MB (5068431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5a0da72908eb54180139e187b047089c01454fc561d10071e004ddddbc83b7`  
		Last Modified: Tue, 07 Nov 2023 21:03:01 GMT  
		Size: 1.2 MB (1198449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c321b6ea80f52f37c190337f940f0c24d98385d9a2311b30680a11ff757a30f`  
		Last Modified: Tue, 07 Nov 2023 21:03:00 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:4206943b7073e21d109937a4da710faadb4c2d68b06eed13cca7a2e81a427ed0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74200658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ad7628f7abe471737f92d250481b6d37b0dbc08b27f4fecd6de4b7069255fce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:50:06 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 13:54:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:17:41 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 21:18:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 21:18:05 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 21:18:06 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 21:18:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:18:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 21:18:08 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:43:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:43:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:43:40 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:43:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:43:41 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:43:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:43:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:43:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ea699c459f4e83d317f31dad3d23c45cc29bbd728f76aa22bd9e4a8180feb8`  
		Last Modified: Sat, 21 Oct 2023 00:50:20 GMT  
		Size: 286.7 KB (286665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f7b3697956c8adf732de1fa607b670ec20dad24d26aa13bdfd9b275c65ab7e`  
		Last Modified: Tue, 07 Nov 2023 21:25:46 GMT  
		Size: 64.1 MB (64111773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f1720227a74244550a3b19be823a0538279f71347eea9e055bc39b87306e09`  
		Last Modified: Tue, 07 Nov 2023 21:25:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5aa813cd8b314d1ecc000832dd9d9a65d87b48fe12a3e26e8973a24739e1e5d`  
		Last Modified: Tue, 07 Nov 2023 21:44:02 GMT  
		Size: 5.3 MB (5268975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526c725b224548c8658f358c73e89e88e8e4ed758879e446da57649f8147caa3`  
		Last Modified: Tue, 07 Nov 2023 21:44:01 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5ec0b117cae64f834ae1c8a5f1c6e2eb7d03ed218ac12f9e531fb65d2749ae`  
		Last Modified: Tue, 07 Nov 2023 21:44:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:01d8af8337066c19a93a4af95f039f93092c42c25958cb75f773287862af55fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76087350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45f25b6ed469e7fd4e3d10476165542d74cc1ff9aa294642362d158ea159c841`
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
# Tue, 07 Nov 2023 20:43:18 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:43:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:43:36 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:43:36 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:43:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:43:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:43:37 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:08:19 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:08:19 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:08:20 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:08:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:08:20 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:08:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:08:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:08:21 GMT
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
	-	`sha256:72d99582ceb0709a8c9a1d5fdc62f431b171ef30aafa94a2f14cdc818695abc2`  
		Last Modified: Tue, 07 Nov 2023 20:50:45 GMT  
		Size: 66.2 MB (66209518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd3acc2cfafbeca6b9582dca1e5dca9862e6059e686d6fd717790f4353277cf`  
		Last Modified: Tue, 07 Nov 2023 20:50:34 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad32e6427b3c189cb8976ef70af84e8e86a742134fbfcc46ce989b710509dfc`  
		Last Modified: Tue, 07 Nov 2023 21:08:48 GMT  
		Size: 5.1 MB (5114684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d837cb4f1c5fec0ee05235ea0bb20b16067e00a6f0494f88afa5fb527b5f790`  
		Last Modified: Tue, 07 Nov 2023 21:08:47 GMT  
		Size: 1.3 MB (1262388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf5bb743910ff919d1d7c652a4eeda2079fef5385f4c212839b9345c940c370`  
		Last Modified: Tue, 07 Nov 2023 21:08:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:db8add82121fb31a1612a7e34b5af6a2180acc560a75b5c295c6421ec5854064
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:823c52d733e025f2f7a994e81853c644a8cb7fc8e2cfaf1759cfbd9f42981bae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2154235329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e51a76e2131305dc407d432736a885084ead87fe0cc9c9a227736e6799405b0`
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
# Thu, 16 Nov 2023 02:49:42 GMT
ENV GOLANG_VERSION=1.21.4
# Thu, 16 Nov 2023 02:52:53 GMT
RUN $url = 'https://dl.google.com/go/go1.21.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '79e5428e068c912d9cfa6cd115c13549856ec689c1332eac17f5d6122e19d595'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:52:55 GMT
WORKDIR C:\go
# Thu, 16 Nov 2023 05:34:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:34:44 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 16 Nov 2023 05:34:45 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:34:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Nov 2023 05:36:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Nov 2023 05:36:01 GMT
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
	-	`sha256:c30930da8ed1e8bdc54250c940331ca68cda0bfb62284a10c659fbd0768848ea`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d113e76a38d50789cec61e62343c448b0f781f2edc2150f8abe914796df72325`  
		Last Modified: Thu, 16 Nov 2023 03:12:14 GMT  
		Size: 69.3 MB (69322889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e233c1968dbb3ae85985bbd8b98ec9454199ca20141c642a7884444c1bc7c7`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 1.6 KB (1580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be3840df58058d3a67a1f4fc3b8987c93be3fba0227a49b9ab08af23db164b3`  
		Last Modified: Thu, 16 Nov 2023 05:38:22 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64072f71e3f7e1d01b75b904e8cb73988c110ba09d61072634272c1c6e0192f5`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be28c184970d229ba318ac93ef72165a50289b21f6822ac961e779c3f7594b2`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fadbb7cc6286a3cc2b7fc543b3a14f8c4527bd76a612ec0e0f971acc57a35a48`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f55e1de34150b2a36b3073acb80b8a2be69b440782f880794957e941f29220`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.7 MB (1661568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be73ad07c8ccee0635f69cb11e8c37458731e7c8791d6b55e3c75a04b533099`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:8e5bb4c8c32d947b3fa0e530ecb103d4dc813be81cf27e924be9b5171dd1a8a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2113; amd64

### `caddy:2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:256d98ebfd54e7da9c594d3a17888987e08a54f31e1a902fdba6062d6475e357
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1983592262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:932ff705341933569835dda3a9df0a381c9efadb23aedbc990ae4c3fe927da37`
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
# Thu, 16 Nov 2023 02:44:31 GMT
ENV GOLANG_VERSION=1.21.4
# Thu, 16 Nov 2023 02:46:51 GMT
RUN $url = 'https://dl.google.com/go/go1.21.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '79e5428e068c912d9cfa6cd115c13549856ec689c1332eac17f5d6122e19d595'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:46:53 GMT
WORKDIR C:\go
# Thu, 16 Nov 2023 05:36:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:36:15 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 16 Nov 2023 05:36:16 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:36:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Nov 2023 05:36:43 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Nov 2023 05:36:44 GMT
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
	-	`sha256:2e99ca1444cc508d00e7f114e5d0ad9c56d99298bd9767a001ab05a1735cacb4`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753e4af07bf1638babc6e18c4a455b8703dfec478e0794970b2e57d76792a281`  
		Last Modified: Thu, 16 Nov 2023 03:11:38 GMT  
		Size: 69.3 MB (69321984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ace7dc382558d5cfabba6fa5df0abb49108d5b6e7ef243a4b4ccfa7639d022`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.6 KB (1572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dee0b52088af84428a19e50ee688425ccee03091d9de2d42ab608d6f4988b90`  
		Last Modified: Thu, 16 Nov 2023 05:38:42 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae08626268dc4e22e38977aa0284b4f4e8aa2a88d8dbf3cfe61c9ffc10292d3`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12154a346b5aa10235e1da2e2c14f346f6de03387fabad1e8b0df50ce81588e5`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33ca4e95a635026944c3bc5da0516b66036a17f0f1a41f8bc2cccfd4afd1015`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37d2fb80d01142c2f56374c7be06d04ac0ddebd778ee3e052d6e627969b6af7`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.7 MB (1667548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41cc79b0b9e584ff384ef15b6bd7d7f1f12e5e73e9105b3e89537f183c38d8d`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1418 bytes)  
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
$ docker pull caddy@sha256:279a5ff568ff6c9e6185a6151e065aacb01c0f275b85f52dd950ac9ae204d8ab
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
$ docker pull caddy@sha256:8e3595ce7a7ebd91a4e91eb41ee367a10e18eb9a711fb28e47f611a7882b3dcc
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
$ docker pull caddy@sha256:5b9c67db8969d2d07fbbea52156ed4a9d59c6b20452e5f230c230a686b60c426
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
$ docker pull caddy@sha256:9557c75b38fa3d68dee8dc5098bacb77894db187429baffcf2028f41edd5686e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76955142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70f74c1f483f810509bfd9c4187e0a600e5a9e8aa2ca801acd27e9cc06aa8d2e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:10:40 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 18:05:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:20:24 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:20:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:20:35 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:20:35 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:20:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:20:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:20:36 GMT
WORKDIR /go
# Tue, 07 Nov 2023 20:44:48 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 20:44:48 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 20:44:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 20:44:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 20:44:50 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834bccaa730c985b202b64916ba9cbab707b8a165cece04b8aea3801d6a75741`  
		Last Modified: Sat, 21 Oct 2023 03:10:51 GMT  
		Size: 284.7 KB (284695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bde6e5b785726fea08cb0fb123a90298ceca5cbdc7f267aec8af550c401a2f6`  
		Last Modified: Tue, 07 Nov 2023 20:26:52 GMT  
		Size: 67.0 MB (66995661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebe3be3b56eef1186e8ed89cfaaacf25685600944b44bcdbbd57eb8c8d188e4`  
		Last Modified: Tue, 07 Nov 2023 20:26:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2104133a0e423dca65ea3889907e07d16f2aee507a0b4e6c113befd233f3376e`  
		Last Modified: Tue, 07 Nov 2023 20:45:08 GMT  
		Size: 5.0 MB (4970027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3223ac085d84a7150dcade2bc8258b726591b749677608a2b7e3a02664a48ba5`  
		Last Modified: Tue, 07 Nov 2023 20:45:07 GMT  
		Size: 1.3 MB (1302232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3306c1ee0dab13ecea29b0e17a898223583940e47acc99449853e9e59435f3`  
		Last Modified: Tue, 07 Nov 2023 20:45:07 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:925051dfec44d86d69116ecf542f98f048d16edc30ee04e84dd0f94b8a306f28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75395073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:337623b638f4d83149457aa62bc5b13dff2de821cac1d7a7deb4b0eba81c383c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:43:17 GMT
RUN apk add --no-cache ca-certificates
# Tue, 07 Nov 2023 20:49:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:49:19 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:49:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:49:36 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:49:36 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:49:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:49:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:49:37 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:12:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:12:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:12:40 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:12:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:12:40 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:12:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:12:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:12:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4459abd186485ffcfbc9a0cc16ba7fc77e7b8af5dd55624328e90ec67ef669`  
		Last Modified: Sat, 21 Oct 2023 00:43:27 GMT  
		Size: 284.9 KB (284882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e47353e44109dd9c41cf34c24ec76dc67e7767decf78622589a90a58c3b2f4`  
		Last Modified: Tue, 07 Nov 2023 20:55:24 GMT  
		Size: 65.8 MB (65751371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed03a7f93d0719301c31ce952f21b9a5a31d7a50775d4ee8bc1070f1ce19f9f`  
		Last Modified: Tue, 07 Nov 2023 20:55:04 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c4b96bb9b7fb0e5321265d67484456c37c1fbd1d5e2565c4f9225f9989acaf`  
		Last Modified: Tue, 07 Nov 2023 21:13:02 GMT  
		Size: 5.0 MB (4964302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82c013a69236b77e239aa51756075002025bfab6a1124e524c8c4f855b72142`  
		Last Modified: Tue, 07 Nov 2023 21:13:02 GMT  
		Size: 1.2 MB (1248664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856961b563a2d5414382e81b6e6a0f242bf2a09bb03623ff004cc79275c9b02c`  
		Last Modified: Tue, 07 Nov 2023 21:13:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:c3408f987d7ee9eedb1a5fcefc1cdf4b24092224fdc2d91a0aae5e4b0ad1e1f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74692592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7150e3216cb69f9c924809d80e3f784b9e25038c5c743f8e415853df8163fd0`
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
# Tue, 07 Nov 2023 21:00:37 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 21:00:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 21:00:51 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 21:00:51 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 21:00:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:00:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 21:00:52 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:25:34 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:25:34 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:25:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:25:36 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:25:36 GMT
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
	-	`sha256:4a3debef18506403ac44cc4950a8cbaaea2e9d311ae1a83607be6f7b78b291ce`  
		Last Modified: Tue, 07 Nov 2023 21:07:30 GMT  
		Size: 65.8 MB (65750717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce90421070593b8c5625d529316d162aac0bcfd55fc9e7507b337aed33c64191`  
		Last Modified: Tue, 07 Nov 2023 21:07:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc6fcb2c4fc6a718864e032be82c1edac9d3564e3b7a5833d5f1c1879365074`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 4.5 MB (4511246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91736d5dba9b84ca32af89f184018cf79348d96d127c913d2721ef9a62c5031`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 1.2 MB (1246088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc61b28fe019881fc188747ffde817dc4796c027b44cb91541a4cb9b08714cf`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b843e7253f9266dbfe42a8aa6ed190a23d4c10856ea0ab900fba06faf579e47f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73974255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b375a225af66400861808f202e662bafd23e07644f836d4e47c6d399b765686d`
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
# Tue, 07 Nov 2023 20:39:55 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:40:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:40:05 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:40:05 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:40:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:40:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:40:06 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:02:44 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:02:44 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:02:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:02:45 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:02:45 GMT
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
	-	`sha256:f9e3860c59e00c3164218e7e9c694435e2bcaaf14693bbc68c2a02a882bcc6a2`  
		Last Modified: Tue, 07 Nov 2023 20:45:13 GMT  
		Size: 64.1 MB (64088686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e79fdc38632695ae6832600d13ce667f701f785944433806d5fbf89a90b675`  
		Last Modified: Tue, 07 Nov 2023 20:45:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f0a09267a67162a19517c78b4e687814d8f7b56bd3f768cada6f09460a11c6`  
		Last Modified: Tue, 07 Nov 2023 21:03:01 GMT  
		Size: 5.1 MB (5068431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5a0da72908eb54180139e187b047089c01454fc561d10071e004ddddbc83b7`  
		Last Modified: Tue, 07 Nov 2023 21:03:01 GMT  
		Size: 1.2 MB (1198449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c321b6ea80f52f37c190337f940f0c24d98385d9a2311b30680a11ff757a30f`  
		Last Modified: Tue, 07 Nov 2023 21:03:00 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:4206943b7073e21d109937a4da710faadb4c2d68b06eed13cca7a2e81a427ed0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74200658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ad7628f7abe471737f92d250481b6d37b0dbc08b27f4fecd6de4b7069255fce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:50:06 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 13:54:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:17:41 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 21:18:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 21:18:05 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 21:18:06 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 21:18:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:18:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 21:18:08 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:43:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:43:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:43:40 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:43:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:43:41 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:43:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:43:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:43:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ea699c459f4e83d317f31dad3d23c45cc29bbd728f76aa22bd9e4a8180feb8`  
		Last Modified: Sat, 21 Oct 2023 00:50:20 GMT  
		Size: 286.7 KB (286665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f7b3697956c8adf732de1fa607b670ec20dad24d26aa13bdfd9b275c65ab7e`  
		Last Modified: Tue, 07 Nov 2023 21:25:46 GMT  
		Size: 64.1 MB (64111773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f1720227a74244550a3b19be823a0538279f71347eea9e055bc39b87306e09`  
		Last Modified: Tue, 07 Nov 2023 21:25:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5aa813cd8b314d1ecc000832dd9d9a65d87b48fe12a3e26e8973a24739e1e5d`  
		Last Modified: Tue, 07 Nov 2023 21:44:02 GMT  
		Size: 5.3 MB (5268975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526c725b224548c8658f358c73e89e88e8e4ed758879e446da57649f8147caa3`  
		Last Modified: Tue, 07 Nov 2023 21:44:01 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5ec0b117cae64f834ae1c8a5f1c6e2eb7d03ed218ac12f9e531fb65d2749ae`  
		Last Modified: Tue, 07 Nov 2023 21:44:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; s390x

```console
$ docker pull caddy@sha256:01d8af8337066c19a93a4af95f039f93092c42c25958cb75f773287862af55fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76087350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45f25b6ed469e7fd4e3d10476165542d74cc1ff9aa294642362d158ea159c841`
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
# Tue, 07 Nov 2023 20:43:18 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:43:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:43:36 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:43:36 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:43:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:43:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:43:37 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:08:19 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:08:19 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:08:20 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:08:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:08:20 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:08:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:08:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:08:21 GMT
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
	-	`sha256:72d99582ceb0709a8c9a1d5fdc62f431b171ef30aafa94a2f14cdc818695abc2`  
		Last Modified: Tue, 07 Nov 2023 20:50:45 GMT  
		Size: 66.2 MB (66209518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd3acc2cfafbeca6b9582dca1e5dca9862e6059e686d6fd717790f4353277cf`  
		Last Modified: Tue, 07 Nov 2023 20:50:34 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad32e6427b3c189cb8976ef70af84e8e86a742134fbfcc46ce989b710509dfc`  
		Last Modified: Tue, 07 Nov 2023 21:08:48 GMT  
		Size: 5.1 MB (5114684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d837cb4f1c5fec0ee05235ea0bb20b16067e00a6f0494f88afa5fb527b5f790`  
		Last Modified: Tue, 07 Nov 2023 21:08:47 GMT  
		Size: 1.3 MB (1262388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf5bb743910ff919d1d7c652a4eeda2079fef5385f4c212839b9345c940c370`  
		Last Modified: Tue, 07 Nov 2023 21:08:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:823c52d733e025f2f7a994e81853c644a8cb7fc8e2cfaf1759cfbd9f42981bae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2154235329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e51a76e2131305dc407d432736a885084ead87fe0cc9c9a227736e6799405b0`
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
# Thu, 16 Nov 2023 02:49:42 GMT
ENV GOLANG_VERSION=1.21.4
# Thu, 16 Nov 2023 02:52:53 GMT
RUN $url = 'https://dl.google.com/go/go1.21.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '79e5428e068c912d9cfa6cd115c13549856ec689c1332eac17f5d6122e19d595'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:52:55 GMT
WORKDIR C:\go
# Thu, 16 Nov 2023 05:34:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:34:44 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 16 Nov 2023 05:34:45 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:34:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Nov 2023 05:36:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Nov 2023 05:36:01 GMT
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
	-	`sha256:c30930da8ed1e8bdc54250c940331ca68cda0bfb62284a10c659fbd0768848ea`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d113e76a38d50789cec61e62343c448b0f781f2edc2150f8abe914796df72325`  
		Last Modified: Thu, 16 Nov 2023 03:12:14 GMT  
		Size: 69.3 MB (69322889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e233c1968dbb3ae85985bbd8b98ec9454199ca20141c642a7884444c1bc7c7`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 1.6 KB (1580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be3840df58058d3a67a1f4fc3b8987c93be3fba0227a49b9ab08af23db164b3`  
		Last Modified: Thu, 16 Nov 2023 05:38:22 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64072f71e3f7e1d01b75b904e8cb73988c110ba09d61072634272c1c6e0192f5`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be28c184970d229ba318ac93ef72165a50289b21f6822ac961e779c3f7594b2`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fadbb7cc6286a3cc2b7fc543b3a14f8c4527bd76a612ec0e0f971acc57a35a48`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f55e1de34150b2a36b3073acb80b8a2be69b440782f880794957e941f29220`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.7 MB (1661568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be73ad07c8ccee0635f69cb11e8c37458731e7c8791d6b55e3c75a04b533099`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:256d98ebfd54e7da9c594d3a17888987e08a54f31e1a902fdba6062d6475e357
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1983592262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:932ff705341933569835dda3a9df0a381c9efadb23aedbc990ae4c3fe927da37`
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
# Thu, 16 Nov 2023 02:44:31 GMT
ENV GOLANG_VERSION=1.21.4
# Thu, 16 Nov 2023 02:46:51 GMT
RUN $url = 'https://dl.google.com/go/go1.21.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '79e5428e068c912d9cfa6cd115c13549856ec689c1332eac17f5d6122e19d595'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:46:53 GMT
WORKDIR C:\go
# Thu, 16 Nov 2023 05:36:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:36:15 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 16 Nov 2023 05:36:16 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:36:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Nov 2023 05:36:43 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Nov 2023 05:36:44 GMT
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
	-	`sha256:2e99ca1444cc508d00e7f114e5d0ad9c56d99298bd9767a001ab05a1735cacb4`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753e4af07bf1638babc6e18c4a455b8703dfec478e0794970b2e57d76792a281`  
		Last Modified: Thu, 16 Nov 2023 03:11:38 GMT  
		Size: 69.3 MB (69321984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ace7dc382558d5cfabba6fa5df0abb49108d5b6e7ef243a4b4ccfa7639d022`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.6 KB (1572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dee0b52088af84428a19e50ee688425ccee03091d9de2d42ab608d6f4988b90`  
		Last Modified: Thu, 16 Nov 2023 05:38:42 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae08626268dc4e22e38977aa0284b4f4e8aa2a88d8dbf3cfe61c9ffc10292d3`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12154a346b5aa10235e1da2e2c14f346f6de03387fabad1e8b0df50ce81588e5`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33ca4e95a635026944c3bc5da0516b66036a17f0f1a41f8bc2cccfd4afd1015`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37d2fb80d01142c2f56374c7be06d04ac0ddebd778ee3e052d6e627969b6af7`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.7 MB (1667548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41cc79b0b9e584ff384ef15b6bd7d7f1f12e5e73e9105b3e89537f183c38d8d`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-builder-alpine`

```console
$ docker pull caddy@sha256:a51593964dcf5b43b549589e0e77d0dec7a1c3491fb5054a8e1e93e22505d1a6
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
$ docker pull caddy@sha256:9557c75b38fa3d68dee8dc5098bacb77894db187429baffcf2028f41edd5686e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76955142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70f74c1f483f810509bfd9c4187e0a600e5a9e8aa2ca801acd27e9cc06aa8d2e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:10:40 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 18:05:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:20:24 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:20:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:20:35 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:20:35 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:20:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:20:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:20:36 GMT
WORKDIR /go
# Tue, 07 Nov 2023 20:44:48 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 20:44:48 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 20:44:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 20:44:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 20:44:50 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834bccaa730c985b202b64916ba9cbab707b8a165cece04b8aea3801d6a75741`  
		Last Modified: Sat, 21 Oct 2023 03:10:51 GMT  
		Size: 284.7 KB (284695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bde6e5b785726fea08cb0fb123a90298ceca5cbdc7f267aec8af550c401a2f6`  
		Last Modified: Tue, 07 Nov 2023 20:26:52 GMT  
		Size: 67.0 MB (66995661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebe3be3b56eef1186e8ed89cfaaacf25685600944b44bcdbbd57eb8c8d188e4`  
		Last Modified: Tue, 07 Nov 2023 20:26:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2104133a0e423dca65ea3889907e07d16f2aee507a0b4e6c113befd233f3376e`  
		Last Modified: Tue, 07 Nov 2023 20:45:08 GMT  
		Size: 5.0 MB (4970027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3223ac085d84a7150dcade2bc8258b726591b749677608a2b7e3a02664a48ba5`  
		Last Modified: Tue, 07 Nov 2023 20:45:07 GMT  
		Size: 1.3 MB (1302232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3306c1ee0dab13ecea29b0e17a898223583940e47acc99449853e9e59435f3`  
		Last Modified: Tue, 07 Nov 2023 20:45:07 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:925051dfec44d86d69116ecf542f98f048d16edc30ee04e84dd0f94b8a306f28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75395073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:337623b638f4d83149457aa62bc5b13dff2de821cac1d7a7deb4b0eba81c383c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:43:17 GMT
RUN apk add --no-cache ca-certificates
# Tue, 07 Nov 2023 20:49:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:49:19 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:49:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:49:36 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:49:36 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:49:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:49:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:49:37 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:12:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:12:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:12:40 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:12:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:12:40 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:12:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:12:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:12:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4459abd186485ffcfbc9a0cc16ba7fc77e7b8af5dd55624328e90ec67ef669`  
		Last Modified: Sat, 21 Oct 2023 00:43:27 GMT  
		Size: 284.9 KB (284882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e47353e44109dd9c41cf34c24ec76dc67e7767decf78622589a90a58c3b2f4`  
		Last Modified: Tue, 07 Nov 2023 20:55:24 GMT  
		Size: 65.8 MB (65751371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed03a7f93d0719301c31ce952f21b9a5a31d7a50775d4ee8bc1070f1ce19f9f`  
		Last Modified: Tue, 07 Nov 2023 20:55:04 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c4b96bb9b7fb0e5321265d67484456c37c1fbd1d5e2565c4f9225f9989acaf`  
		Last Modified: Tue, 07 Nov 2023 21:13:02 GMT  
		Size: 5.0 MB (4964302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82c013a69236b77e239aa51756075002025bfab6a1124e524c8c4f855b72142`  
		Last Modified: Tue, 07 Nov 2023 21:13:02 GMT  
		Size: 1.2 MB (1248664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856961b563a2d5414382e81b6e6a0f242bf2a09bb03623ff004cc79275c9b02c`  
		Last Modified: Tue, 07 Nov 2023 21:13:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:c3408f987d7ee9eedb1a5fcefc1cdf4b24092224fdc2d91a0aae5e4b0ad1e1f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74692592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7150e3216cb69f9c924809d80e3f784b9e25038c5c743f8e415853df8163fd0`
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
# Tue, 07 Nov 2023 21:00:37 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 21:00:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 21:00:51 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 21:00:51 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 21:00:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:00:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 21:00:52 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:25:34 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:25:34 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:25:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:25:36 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:25:36 GMT
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
	-	`sha256:4a3debef18506403ac44cc4950a8cbaaea2e9d311ae1a83607be6f7b78b291ce`  
		Last Modified: Tue, 07 Nov 2023 21:07:30 GMT  
		Size: 65.8 MB (65750717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce90421070593b8c5625d529316d162aac0bcfd55fc9e7507b337aed33c64191`  
		Last Modified: Tue, 07 Nov 2023 21:07:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc6fcb2c4fc6a718864e032be82c1edac9d3564e3b7a5833d5f1c1879365074`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 4.5 MB (4511246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91736d5dba9b84ca32af89f184018cf79348d96d127c913d2721ef9a62c5031`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 1.2 MB (1246088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc61b28fe019881fc188747ffde817dc4796c027b44cb91541a4cb9b08714cf`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b843e7253f9266dbfe42a8aa6ed190a23d4c10856ea0ab900fba06faf579e47f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73974255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b375a225af66400861808f202e662bafd23e07644f836d4e47c6d399b765686d`
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
# Tue, 07 Nov 2023 20:39:55 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:40:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:40:05 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:40:05 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:40:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:40:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:40:06 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:02:44 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:02:44 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:02:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:02:45 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:02:45 GMT
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
	-	`sha256:f9e3860c59e00c3164218e7e9c694435e2bcaaf14693bbc68c2a02a882bcc6a2`  
		Last Modified: Tue, 07 Nov 2023 20:45:13 GMT  
		Size: 64.1 MB (64088686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e79fdc38632695ae6832600d13ce667f701f785944433806d5fbf89a90b675`  
		Last Modified: Tue, 07 Nov 2023 20:45:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f0a09267a67162a19517c78b4e687814d8f7b56bd3f768cada6f09460a11c6`  
		Last Modified: Tue, 07 Nov 2023 21:03:01 GMT  
		Size: 5.1 MB (5068431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5a0da72908eb54180139e187b047089c01454fc561d10071e004ddddbc83b7`  
		Last Modified: Tue, 07 Nov 2023 21:03:01 GMT  
		Size: 1.2 MB (1198449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c321b6ea80f52f37c190337f940f0c24d98385d9a2311b30680a11ff757a30f`  
		Last Modified: Tue, 07 Nov 2023 21:03:00 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:4206943b7073e21d109937a4da710faadb4c2d68b06eed13cca7a2e81a427ed0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74200658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ad7628f7abe471737f92d250481b6d37b0dbc08b27f4fecd6de4b7069255fce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:50:06 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 13:54:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:17:41 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 21:18:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 21:18:05 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 21:18:06 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 21:18:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:18:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 21:18:08 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:43:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:43:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:43:40 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:43:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:43:41 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:43:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:43:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:43:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ea699c459f4e83d317f31dad3d23c45cc29bbd728f76aa22bd9e4a8180feb8`  
		Last Modified: Sat, 21 Oct 2023 00:50:20 GMT  
		Size: 286.7 KB (286665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f7b3697956c8adf732de1fa607b670ec20dad24d26aa13bdfd9b275c65ab7e`  
		Last Modified: Tue, 07 Nov 2023 21:25:46 GMT  
		Size: 64.1 MB (64111773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f1720227a74244550a3b19be823a0538279f71347eea9e055bc39b87306e09`  
		Last Modified: Tue, 07 Nov 2023 21:25:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5aa813cd8b314d1ecc000832dd9d9a65d87b48fe12a3e26e8973a24739e1e5d`  
		Last Modified: Tue, 07 Nov 2023 21:44:02 GMT  
		Size: 5.3 MB (5268975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526c725b224548c8658f358c73e89e88e8e4ed758879e446da57649f8147caa3`  
		Last Modified: Tue, 07 Nov 2023 21:44:01 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5ec0b117cae64f834ae1c8a5f1c6e2eb7d03ed218ac12f9e531fb65d2749ae`  
		Last Modified: Tue, 07 Nov 2023 21:44:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:01d8af8337066c19a93a4af95f039f93092c42c25958cb75f773287862af55fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76087350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45f25b6ed469e7fd4e3d10476165542d74cc1ff9aa294642362d158ea159c841`
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
# Tue, 07 Nov 2023 20:43:18 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:43:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:43:36 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:43:36 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:43:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:43:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:43:37 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:08:19 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:08:19 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:08:20 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:08:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:08:20 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:08:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:08:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:08:21 GMT
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
	-	`sha256:72d99582ceb0709a8c9a1d5fdc62f431b171ef30aafa94a2f14cdc818695abc2`  
		Last Modified: Tue, 07 Nov 2023 20:50:45 GMT  
		Size: 66.2 MB (66209518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd3acc2cfafbeca6b9582dca1e5dca9862e6059e686d6fd717790f4353277cf`  
		Last Modified: Tue, 07 Nov 2023 20:50:34 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad32e6427b3c189cb8976ef70af84e8e86a742134fbfcc46ce989b710509dfc`  
		Last Modified: Tue, 07 Nov 2023 21:08:48 GMT  
		Size: 5.1 MB (5114684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d837cb4f1c5fec0ee05235ea0bb20b16067e00a6f0494f88afa5fb527b5f790`  
		Last Modified: Tue, 07 Nov 2023 21:08:47 GMT  
		Size: 1.3 MB (1262388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf5bb743910ff919d1d7c652a4eeda2079fef5385f4c212839b9345c940c370`  
		Last Modified: Tue, 07 Nov 2023 21:08:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:db8add82121fb31a1612a7e34b5af6a2180acc560a75b5c295c6421ec5854064
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `caddy:2.7-builder-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:823c52d733e025f2f7a994e81853c644a8cb7fc8e2cfaf1759cfbd9f42981bae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2154235329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e51a76e2131305dc407d432736a885084ead87fe0cc9c9a227736e6799405b0`
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
# Thu, 16 Nov 2023 02:49:42 GMT
ENV GOLANG_VERSION=1.21.4
# Thu, 16 Nov 2023 02:52:53 GMT
RUN $url = 'https://dl.google.com/go/go1.21.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '79e5428e068c912d9cfa6cd115c13549856ec689c1332eac17f5d6122e19d595'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:52:55 GMT
WORKDIR C:\go
# Thu, 16 Nov 2023 05:34:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:34:44 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 16 Nov 2023 05:34:45 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:34:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Nov 2023 05:36:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Nov 2023 05:36:01 GMT
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
	-	`sha256:c30930da8ed1e8bdc54250c940331ca68cda0bfb62284a10c659fbd0768848ea`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d113e76a38d50789cec61e62343c448b0f781f2edc2150f8abe914796df72325`  
		Last Modified: Thu, 16 Nov 2023 03:12:14 GMT  
		Size: 69.3 MB (69322889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e233c1968dbb3ae85985bbd8b98ec9454199ca20141c642a7884444c1bc7c7`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 1.6 KB (1580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be3840df58058d3a67a1f4fc3b8987c93be3fba0227a49b9ab08af23db164b3`  
		Last Modified: Thu, 16 Nov 2023 05:38:22 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64072f71e3f7e1d01b75b904e8cb73988c110ba09d61072634272c1c6e0192f5`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be28c184970d229ba318ac93ef72165a50289b21f6822ac961e779c3f7594b2`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fadbb7cc6286a3cc2b7fc543b3a14f8c4527bd76a612ec0e0f971acc57a35a48`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f55e1de34150b2a36b3073acb80b8a2be69b440782f880794957e941f29220`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.7 MB (1661568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be73ad07c8ccee0635f69cb11e8c37458731e7c8791d6b55e3c75a04b533099`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:8e5bb4c8c32d947b3fa0e530ecb103d4dc813be81cf27e924be9b5171dd1a8a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2113; amd64

### `caddy:2.7-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:256d98ebfd54e7da9c594d3a17888987e08a54f31e1a902fdba6062d6475e357
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1983592262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:932ff705341933569835dda3a9df0a381c9efadb23aedbc990ae4c3fe927da37`
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
# Thu, 16 Nov 2023 02:44:31 GMT
ENV GOLANG_VERSION=1.21.4
# Thu, 16 Nov 2023 02:46:51 GMT
RUN $url = 'https://dl.google.com/go/go1.21.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '79e5428e068c912d9cfa6cd115c13549856ec689c1332eac17f5d6122e19d595'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:46:53 GMT
WORKDIR C:\go
# Thu, 16 Nov 2023 05:36:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:36:15 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 16 Nov 2023 05:36:16 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:36:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Nov 2023 05:36:43 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Nov 2023 05:36:44 GMT
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
	-	`sha256:2e99ca1444cc508d00e7f114e5d0ad9c56d99298bd9767a001ab05a1735cacb4`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753e4af07bf1638babc6e18c4a455b8703dfec478e0794970b2e57d76792a281`  
		Last Modified: Thu, 16 Nov 2023 03:11:38 GMT  
		Size: 69.3 MB (69321984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ace7dc382558d5cfabba6fa5df0abb49108d5b6e7ef243a4b4ccfa7639d022`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.6 KB (1572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dee0b52088af84428a19e50ee688425ccee03091d9de2d42ab608d6f4988b90`  
		Last Modified: Thu, 16 Nov 2023 05:38:42 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae08626268dc4e22e38977aa0284b4f4e8aa2a88d8dbf3cfe61c9ffc10292d3`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12154a346b5aa10235e1da2e2c14f346f6de03387fabad1e8b0df50ce81588e5`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33ca4e95a635026944c3bc5da0516b66036a17f0f1a41f8bc2cccfd4afd1015`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37d2fb80d01142c2f56374c7be06d04ac0ddebd778ee3e052d6e627969b6af7`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.7 MB (1667548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41cc79b0b9e584ff384ef15b6bd7d7f1f12e5e73e9105b3e89537f183c38d8d`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1418 bytes)  
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

## `caddy:2.7.5`

```console
$ docker pull caddy@sha256:279a5ff568ff6c9e6185a6151e065aacb01c0f275b85f52dd950ac9ae204d8ab
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

### `caddy:2.7.5` - linux; arm variant v7

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

### `caddy:2.7.5` - linux; arm64 variant v8

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

### `caddy:2.7.5` - linux; ppc64le

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

### `caddy:2.7.5` - windows version 10.0.17763.5122; amd64

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

### `caddy:2.7.5` - windows version 10.0.20348.2113; amd64

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

## `caddy:2.7.5-alpine`

```console
$ docker pull caddy@sha256:8e3595ce7a7ebd91a4e91eb41ee367a10e18eb9a711fb28e47f611a7882b3dcc
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

### `caddy:2.7.5-alpine` - linux; arm variant v7

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

### `caddy:2.7.5-alpine` - linux; arm64 variant v8

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

### `caddy:2.7.5-alpine` - linux; ppc64le

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
$ docker pull caddy@sha256:5b9c67db8969d2d07fbbea52156ed4a9d59c6b20452e5f230c230a686b60c426
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

### `caddy:2.7.5-builder` - linux; amd64

```console
$ docker pull caddy@sha256:9557c75b38fa3d68dee8dc5098bacb77894db187429baffcf2028f41edd5686e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76955142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70f74c1f483f810509bfd9c4187e0a600e5a9e8aa2ca801acd27e9cc06aa8d2e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:10:40 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 18:05:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:20:24 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:20:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:20:35 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:20:35 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:20:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:20:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:20:36 GMT
WORKDIR /go
# Tue, 07 Nov 2023 20:44:48 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 20:44:48 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 20:44:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 20:44:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 20:44:50 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834bccaa730c985b202b64916ba9cbab707b8a165cece04b8aea3801d6a75741`  
		Last Modified: Sat, 21 Oct 2023 03:10:51 GMT  
		Size: 284.7 KB (284695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bde6e5b785726fea08cb0fb123a90298ceca5cbdc7f267aec8af550c401a2f6`  
		Last Modified: Tue, 07 Nov 2023 20:26:52 GMT  
		Size: 67.0 MB (66995661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebe3be3b56eef1186e8ed89cfaaacf25685600944b44bcdbbd57eb8c8d188e4`  
		Last Modified: Tue, 07 Nov 2023 20:26:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2104133a0e423dca65ea3889907e07d16f2aee507a0b4e6c113befd233f3376e`  
		Last Modified: Tue, 07 Nov 2023 20:45:08 GMT  
		Size: 5.0 MB (4970027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3223ac085d84a7150dcade2bc8258b726591b749677608a2b7e3a02664a48ba5`  
		Last Modified: Tue, 07 Nov 2023 20:45:07 GMT  
		Size: 1.3 MB (1302232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3306c1ee0dab13ecea29b0e17a898223583940e47acc99449853e9e59435f3`  
		Last Modified: Tue, 07 Nov 2023 20:45:07 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:925051dfec44d86d69116ecf542f98f048d16edc30ee04e84dd0f94b8a306f28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75395073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:337623b638f4d83149457aa62bc5b13dff2de821cac1d7a7deb4b0eba81c383c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:43:17 GMT
RUN apk add --no-cache ca-certificates
# Tue, 07 Nov 2023 20:49:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:49:19 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:49:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:49:36 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:49:36 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:49:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:49:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:49:37 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:12:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:12:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:12:40 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:12:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:12:40 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:12:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:12:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:12:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4459abd186485ffcfbc9a0cc16ba7fc77e7b8af5dd55624328e90ec67ef669`  
		Last Modified: Sat, 21 Oct 2023 00:43:27 GMT  
		Size: 284.9 KB (284882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e47353e44109dd9c41cf34c24ec76dc67e7767decf78622589a90a58c3b2f4`  
		Last Modified: Tue, 07 Nov 2023 20:55:24 GMT  
		Size: 65.8 MB (65751371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed03a7f93d0719301c31ce952f21b9a5a31d7a50775d4ee8bc1070f1ce19f9f`  
		Last Modified: Tue, 07 Nov 2023 20:55:04 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c4b96bb9b7fb0e5321265d67484456c37c1fbd1d5e2565c4f9225f9989acaf`  
		Last Modified: Tue, 07 Nov 2023 21:13:02 GMT  
		Size: 5.0 MB (4964302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82c013a69236b77e239aa51756075002025bfab6a1124e524c8c4f855b72142`  
		Last Modified: Tue, 07 Nov 2023 21:13:02 GMT  
		Size: 1.2 MB (1248664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856961b563a2d5414382e81b6e6a0f242bf2a09bb03623ff004cc79275c9b02c`  
		Last Modified: Tue, 07 Nov 2023 21:13:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:c3408f987d7ee9eedb1a5fcefc1cdf4b24092224fdc2d91a0aae5e4b0ad1e1f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74692592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7150e3216cb69f9c924809d80e3f784b9e25038c5c743f8e415853df8163fd0`
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
# Tue, 07 Nov 2023 21:00:37 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 21:00:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 21:00:51 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 21:00:51 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 21:00:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:00:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 21:00:52 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:25:34 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:25:34 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:25:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:25:36 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:25:36 GMT
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
	-	`sha256:4a3debef18506403ac44cc4950a8cbaaea2e9d311ae1a83607be6f7b78b291ce`  
		Last Modified: Tue, 07 Nov 2023 21:07:30 GMT  
		Size: 65.8 MB (65750717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce90421070593b8c5625d529316d162aac0bcfd55fc9e7507b337aed33c64191`  
		Last Modified: Tue, 07 Nov 2023 21:07:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc6fcb2c4fc6a718864e032be82c1edac9d3564e3b7a5833d5f1c1879365074`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 4.5 MB (4511246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91736d5dba9b84ca32af89f184018cf79348d96d127c913d2721ef9a62c5031`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 1.2 MB (1246088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc61b28fe019881fc188747ffde817dc4796c027b44cb91541a4cb9b08714cf`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b843e7253f9266dbfe42a8aa6ed190a23d4c10856ea0ab900fba06faf579e47f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73974255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b375a225af66400861808f202e662bafd23e07644f836d4e47c6d399b765686d`
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
# Tue, 07 Nov 2023 20:39:55 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:40:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:40:05 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:40:05 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:40:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:40:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:40:06 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:02:44 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:02:44 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:02:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:02:45 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:02:45 GMT
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
	-	`sha256:f9e3860c59e00c3164218e7e9c694435e2bcaaf14693bbc68c2a02a882bcc6a2`  
		Last Modified: Tue, 07 Nov 2023 20:45:13 GMT  
		Size: 64.1 MB (64088686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e79fdc38632695ae6832600d13ce667f701f785944433806d5fbf89a90b675`  
		Last Modified: Tue, 07 Nov 2023 20:45:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f0a09267a67162a19517c78b4e687814d8f7b56bd3f768cada6f09460a11c6`  
		Last Modified: Tue, 07 Nov 2023 21:03:01 GMT  
		Size: 5.1 MB (5068431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5a0da72908eb54180139e187b047089c01454fc561d10071e004ddddbc83b7`  
		Last Modified: Tue, 07 Nov 2023 21:03:01 GMT  
		Size: 1.2 MB (1198449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c321b6ea80f52f37c190337f940f0c24d98385d9a2311b30680a11ff757a30f`  
		Last Modified: Tue, 07 Nov 2023 21:03:00 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:4206943b7073e21d109937a4da710faadb4c2d68b06eed13cca7a2e81a427ed0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74200658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ad7628f7abe471737f92d250481b6d37b0dbc08b27f4fecd6de4b7069255fce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:50:06 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 13:54:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:17:41 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 21:18:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 21:18:05 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 21:18:06 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 21:18:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:18:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 21:18:08 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:43:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:43:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:43:40 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:43:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:43:41 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:43:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:43:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:43:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ea699c459f4e83d317f31dad3d23c45cc29bbd728f76aa22bd9e4a8180feb8`  
		Last Modified: Sat, 21 Oct 2023 00:50:20 GMT  
		Size: 286.7 KB (286665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f7b3697956c8adf732de1fa607b670ec20dad24d26aa13bdfd9b275c65ab7e`  
		Last Modified: Tue, 07 Nov 2023 21:25:46 GMT  
		Size: 64.1 MB (64111773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f1720227a74244550a3b19be823a0538279f71347eea9e055bc39b87306e09`  
		Last Modified: Tue, 07 Nov 2023 21:25:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5aa813cd8b314d1ecc000832dd9d9a65d87b48fe12a3e26e8973a24739e1e5d`  
		Last Modified: Tue, 07 Nov 2023 21:44:02 GMT  
		Size: 5.3 MB (5268975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526c725b224548c8658f358c73e89e88e8e4ed758879e446da57649f8147caa3`  
		Last Modified: Tue, 07 Nov 2023 21:44:01 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5ec0b117cae64f834ae1c8a5f1c6e2eb7d03ed218ac12f9e531fb65d2749ae`  
		Last Modified: Tue, 07 Nov 2023 21:44:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder` - linux; s390x

```console
$ docker pull caddy@sha256:01d8af8337066c19a93a4af95f039f93092c42c25958cb75f773287862af55fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76087350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45f25b6ed469e7fd4e3d10476165542d74cc1ff9aa294642362d158ea159c841`
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
# Tue, 07 Nov 2023 20:43:18 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:43:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:43:36 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:43:36 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:43:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:43:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:43:37 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:08:19 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:08:19 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:08:20 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:08:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:08:20 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:08:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:08:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:08:21 GMT
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
	-	`sha256:72d99582ceb0709a8c9a1d5fdc62f431b171ef30aafa94a2f14cdc818695abc2`  
		Last Modified: Tue, 07 Nov 2023 20:50:45 GMT  
		Size: 66.2 MB (66209518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd3acc2cfafbeca6b9582dca1e5dca9862e6059e686d6fd717790f4353277cf`  
		Last Modified: Tue, 07 Nov 2023 20:50:34 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad32e6427b3c189cb8976ef70af84e8e86a742134fbfcc46ce989b710509dfc`  
		Last Modified: Tue, 07 Nov 2023 21:08:48 GMT  
		Size: 5.1 MB (5114684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d837cb4f1c5fec0ee05235ea0bb20b16067e00a6f0494f88afa5fb527b5f790`  
		Last Modified: Tue, 07 Nov 2023 21:08:47 GMT  
		Size: 1.3 MB (1262388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf5bb743910ff919d1d7c652a4eeda2079fef5385f4c212839b9345c940c370`  
		Last Modified: Tue, 07 Nov 2023 21:08:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:823c52d733e025f2f7a994e81853c644a8cb7fc8e2cfaf1759cfbd9f42981bae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2154235329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e51a76e2131305dc407d432736a885084ead87fe0cc9c9a227736e6799405b0`
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
# Thu, 16 Nov 2023 02:49:42 GMT
ENV GOLANG_VERSION=1.21.4
# Thu, 16 Nov 2023 02:52:53 GMT
RUN $url = 'https://dl.google.com/go/go1.21.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '79e5428e068c912d9cfa6cd115c13549856ec689c1332eac17f5d6122e19d595'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:52:55 GMT
WORKDIR C:\go
# Thu, 16 Nov 2023 05:34:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:34:44 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 16 Nov 2023 05:34:45 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:34:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Nov 2023 05:36:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Nov 2023 05:36:01 GMT
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
	-	`sha256:c30930da8ed1e8bdc54250c940331ca68cda0bfb62284a10c659fbd0768848ea`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d113e76a38d50789cec61e62343c448b0f781f2edc2150f8abe914796df72325`  
		Last Modified: Thu, 16 Nov 2023 03:12:14 GMT  
		Size: 69.3 MB (69322889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e233c1968dbb3ae85985bbd8b98ec9454199ca20141c642a7884444c1bc7c7`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 1.6 KB (1580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be3840df58058d3a67a1f4fc3b8987c93be3fba0227a49b9ab08af23db164b3`  
		Last Modified: Thu, 16 Nov 2023 05:38:22 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64072f71e3f7e1d01b75b904e8cb73988c110ba09d61072634272c1c6e0192f5`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be28c184970d229ba318ac93ef72165a50289b21f6822ac961e779c3f7594b2`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fadbb7cc6286a3cc2b7fc543b3a14f8c4527bd76a612ec0e0f971acc57a35a48`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f55e1de34150b2a36b3073acb80b8a2be69b440782f880794957e941f29220`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.7 MB (1661568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be73ad07c8ccee0635f69cb11e8c37458731e7c8791d6b55e3c75a04b533099`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:256d98ebfd54e7da9c594d3a17888987e08a54f31e1a902fdba6062d6475e357
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1983592262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:932ff705341933569835dda3a9df0a381c9efadb23aedbc990ae4c3fe927da37`
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
# Thu, 16 Nov 2023 02:44:31 GMT
ENV GOLANG_VERSION=1.21.4
# Thu, 16 Nov 2023 02:46:51 GMT
RUN $url = 'https://dl.google.com/go/go1.21.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '79e5428e068c912d9cfa6cd115c13549856ec689c1332eac17f5d6122e19d595'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:46:53 GMT
WORKDIR C:\go
# Thu, 16 Nov 2023 05:36:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:36:15 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 16 Nov 2023 05:36:16 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:36:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Nov 2023 05:36:43 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Nov 2023 05:36:44 GMT
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
	-	`sha256:2e99ca1444cc508d00e7f114e5d0ad9c56d99298bd9767a001ab05a1735cacb4`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753e4af07bf1638babc6e18c4a455b8703dfec478e0794970b2e57d76792a281`  
		Last Modified: Thu, 16 Nov 2023 03:11:38 GMT  
		Size: 69.3 MB (69321984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ace7dc382558d5cfabba6fa5df0abb49108d5b6e7ef243a4b4ccfa7639d022`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.6 KB (1572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dee0b52088af84428a19e50ee688425ccee03091d9de2d42ab608d6f4988b90`  
		Last Modified: Thu, 16 Nov 2023 05:38:42 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae08626268dc4e22e38977aa0284b4f4e8aa2a88d8dbf3cfe61c9ffc10292d3`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12154a346b5aa10235e1da2e2c14f346f6de03387fabad1e8b0df50ce81588e5`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33ca4e95a635026944c3bc5da0516b66036a17f0f1a41f8bc2cccfd4afd1015`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37d2fb80d01142c2f56374c7be06d04ac0ddebd778ee3e052d6e627969b6af7`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.7 MB (1667548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41cc79b0b9e584ff384ef15b6bd7d7f1f12e5e73e9105b3e89537f183c38d8d`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.5-builder-alpine`

```console
$ docker pull caddy@sha256:a51593964dcf5b43b549589e0e77d0dec7a1c3491fb5054a8e1e93e22505d1a6
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
$ docker pull caddy@sha256:9557c75b38fa3d68dee8dc5098bacb77894db187429baffcf2028f41edd5686e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76955142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70f74c1f483f810509bfd9c4187e0a600e5a9e8aa2ca801acd27e9cc06aa8d2e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:10:40 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 18:05:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:20:24 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:20:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:20:35 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:20:35 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:20:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:20:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:20:36 GMT
WORKDIR /go
# Tue, 07 Nov 2023 20:44:48 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 20:44:48 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 20:44:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 20:44:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 20:44:50 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834bccaa730c985b202b64916ba9cbab707b8a165cece04b8aea3801d6a75741`  
		Last Modified: Sat, 21 Oct 2023 03:10:51 GMT  
		Size: 284.7 KB (284695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bde6e5b785726fea08cb0fb123a90298ceca5cbdc7f267aec8af550c401a2f6`  
		Last Modified: Tue, 07 Nov 2023 20:26:52 GMT  
		Size: 67.0 MB (66995661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebe3be3b56eef1186e8ed89cfaaacf25685600944b44bcdbbd57eb8c8d188e4`  
		Last Modified: Tue, 07 Nov 2023 20:26:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2104133a0e423dca65ea3889907e07d16f2aee507a0b4e6c113befd233f3376e`  
		Last Modified: Tue, 07 Nov 2023 20:45:08 GMT  
		Size: 5.0 MB (4970027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3223ac085d84a7150dcade2bc8258b726591b749677608a2b7e3a02664a48ba5`  
		Last Modified: Tue, 07 Nov 2023 20:45:07 GMT  
		Size: 1.3 MB (1302232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3306c1ee0dab13ecea29b0e17a898223583940e47acc99449853e9e59435f3`  
		Last Modified: Tue, 07 Nov 2023 20:45:07 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:925051dfec44d86d69116ecf542f98f048d16edc30ee04e84dd0f94b8a306f28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75395073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:337623b638f4d83149457aa62bc5b13dff2de821cac1d7a7deb4b0eba81c383c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:43:17 GMT
RUN apk add --no-cache ca-certificates
# Tue, 07 Nov 2023 20:49:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:49:19 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:49:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:49:36 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:49:36 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:49:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:49:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:49:37 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:12:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:12:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:12:40 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:12:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:12:40 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:12:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:12:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:12:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4459abd186485ffcfbc9a0cc16ba7fc77e7b8af5dd55624328e90ec67ef669`  
		Last Modified: Sat, 21 Oct 2023 00:43:27 GMT  
		Size: 284.9 KB (284882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e47353e44109dd9c41cf34c24ec76dc67e7767decf78622589a90a58c3b2f4`  
		Last Modified: Tue, 07 Nov 2023 20:55:24 GMT  
		Size: 65.8 MB (65751371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed03a7f93d0719301c31ce952f21b9a5a31d7a50775d4ee8bc1070f1ce19f9f`  
		Last Modified: Tue, 07 Nov 2023 20:55:04 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c4b96bb9b7fb0e5321265d67484456c37c1fbd1d5e2565c4f9225f9989acaf`  
		Last Modified: Tue, 07 Nov 2023 21:13:02 GMT  
		Size: 5.0 MB (4964302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82c013a69236b77e239aa51756075002025bfab6a1124e524c8c4f855b72142`  
		Last Modified: Tue, 07 Nov 2023 21:13:02 GMT  
		Size: 1.2 MB (1248664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856961b563a2d5414382e81b6e6a0f242bf2a09bb03623ff004cc79275c9b02c`  
		Last Modified: Tue, 07 Nov 2023 21:13:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:c3408f987d7ee9eedb1a5fcefc1cdf4b24092224fdc2d91a0aae5e4b0ad1e1f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74692592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7150e3216cb69f9c924809d80e3f784b9e25038c5c743f8e415853df8163fd0`
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
# Tue, 07 Nov 2023 21:00:37 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 21:00:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 21:00:51 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 21:00:51 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 21:00:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:00:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 21:00:52 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:25:34 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:25:34 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:25:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:25:36 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:25:36 GMT
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
	-	`sha256:4a3debef18506403ac44cc4950a8cbaaea2e9d311ae1a83607be6f7b78b291ce`  
		Last Modified: Tue, 07 Nov 2023 21:07:30 GMT  
		Size: 65.8 MB (65750717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce90421070593b8c5625d529316d162aac0bcfd55fc9e7507b337aed33c64191`  
		Last Modified: Tue, 07 Nov 2023 21:07:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc6fcb2c4fc6a718864e032be82c1edac9d3564e3b7a5833d5f1c1879365074`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 4.5 MB (4511246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91736d5dba9b84ca32af89f184018cf79348d96d127c913d2721ef9a62c5031`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 1.2 MB (1246088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc61b28fe019881fc188747ffde817dc4796c027b44cb91541a4cb9b08714cf`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b843e7253f9266dbfe42a8aa6ed190a23d4c10856ea0ab900fba06faf579e47f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73974255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b375a225af66400861808f202e662bafd23e07644f836d4e47c6d399b765686d`
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
# Tue, 07 Nov 2023 20:39:55 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:40:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:40:05 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:40:05 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:40:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:40:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:40:06 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:02:44 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:02:44 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:02:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:02:45 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:02:45 GMT
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
	-	`sha256:f9e3860c59e00c3164218e7e9c694435e2bcaaf14693bbc68c2a02a882bcc6a2`  
		Last Modified: Tue, 07 Nov 2023 20:45:13 GMT  
		Size: 64.1 MB (64088686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e79fdc38632695ae6832600d13ce667f701f785944433806d5fbf89a90b675`  
		Last Modified: Tue, 07 Nov 2023 20:45:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f0a09267a67162a19517c78b4e687814d8f7b56bd3f768cada6f09460a11c6`  
		Last Modified: Tue, 07 Nov 2023 21:03:01 GMT  
		Size: 5.1 MB (5068431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5a0da72908eb54180139e187b047089c01454fc561d10071e004ddddbc83b7`  
		Last Modified: Tue, 07 Nov 2023 21:03:01 GMT  
		Size: 1.2 MB (1198449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c321b6ea80f52f37c190337f940f0c24d98385d9a2311b30680a11ff757a30f`  
		Last Modified: Tue, 07 Nov 2023 21:03:00 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:4206943b7073e21d109937a4da710faadb4c2d68b06eed13cca7a2e81a427ed0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74200658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ad7628f7abe471737f92d250481b6d37b0dbc08b27f4fecd6de4b7069255fce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:50:06 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 13:54:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:17:41 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 21:18:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 21:18:05 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 21:18:06 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 21:18:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:18:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 21:18:08 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:43:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:43:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:43:40 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:43:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:43:41 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:43:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:43:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:43:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ea699c459f4e83d317f31dad3d23c45cc29bbd728f76aa22bd9e4a8180feb8`  
		Last Modified: Sat, 21 Oct 2023 00:50:20 GMT  
		Size: 286.7 KB (286665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f7b3697956c8adf732de1fa607b670ec20dad24d26aa13bdfd9b275c65ab7e`  
		Last Modified: Tue, 07 Nov 2023 21:25:46 GMT  
		Size: 64.1 MB (64111773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f1720227a74244550a3b19be823a0538279f71347eea9e055bc39b87306e09`  
		Last Modified: Tue, 07 Nov 2023 21:25:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5aa813cd8b314d1ecc000832dd9d9a65d87b48fe12a3e26e8973a24739e1e5d`  
		Last Modified: Tue, 07 Nov 2023 21:44:02 GMT  
		Size: 5.3 MB (5268975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526c725b224548c8658f358c73e89e88e8e4ed758879e446da57649f8147caa3`  
		Last Modified: Tue, 07 Nov 2023 21:44:01 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5ec0b117cae64f834ae1c8a5f1c6e2eb7d03ed218ac12f9e531fb65d2749ae`  
		Last Modified: Tue, 07 Nov 2023 21:44:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.5-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:01d8af8337066c19a93a4af95f039f93092c42c25958cb75f773287862af55fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76087350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45f25b6ed469e7fd4e3d10476165542d74cc1ff9aa294642362d158ea159c841`
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
# Tue, 07 Nov 2023 20:43:18 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:43:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:43:36 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:43:36 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:43:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:43:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:43:37 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:08:19 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:08:19 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:08:20 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:08:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:08:20 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:08:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:08:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:08:21 GMT
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
	-	`sha256:72d99582ceb0709a8c9a1d5fdc62f431b171ef30aafa94a2f14cdc818695abc2`  
		Last Modified: Tue, 07 Nov 2023 20:50:45 GMT  
		Size: 66.2 MB (66209518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd3acc2cfafbeca6b9582dca1e5dca9862e6059e686d6fd717790f4353277cf`  
		Last Modified: Tue, 07 Nov 2023 20:50:34 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad32e6427b3c189cb8976ef70af84e8e86a742134fbfcc46ce989b710509dfc`  
		Last Modified: Tue, 07 Nov 2023 21:08:48 GMT  
		Size: 5.1 MB (5114684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d837cb4f1c5fec0ee05235ea0bb20b16067e00a6f0494f88afa5fb527b5f790`  
		Last Modified: Tue, 07 Nov 2023 21:08:47 GMT  
		Size: 1.3 MB (1262388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf5bb743910ff919d1d7c652a4eeda2079fef5385f4c212839b9345c940c370`  
		Last Modified: Tue, 07 Nov 2023 21:08:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.5-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:db8add82121fb31a1612a7e34b5af6a2180acc560a75b5c295c6421ec5854064
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `caddy:2.7.5-builder-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:823c52d733e025f2f7a994e81853c644a8cb7fc8e2cfaf1759cfbd9f42981bae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2154235329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e51a76e2131305dc407d432736a885084ead87fe0cc9c9a227736e6799405b0`
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
# Thu, 16 Nov 2023 02:49:42 GMT
ENV GOLANG_VERSION=1.21.4
# Thu, 16 Nov 2023 02:52:53 GMT
RUN $url = 'https://dl.google.com/go/go1.21.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '79e5428e068c912d9cfa6cd115c13549856ec689c1332eac17f5d6122e19d595'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:52:55 GMT
WORKDIR C:\go
# Thu, 16 Nov 2023 05:34:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:34:44 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 16 Nov 2023 05:34:45 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:34:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Nov 2023 05:36:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Nov 2023 05:36:01 GMT
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
	-	`sha256:c30930da8ed1e8bdc54250c940331ca68cda0bfb62284a10c659fbd0768848ea`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d113e76a38d50789cec61e62343c448b0f781f2edc2150f8abe914796df72325`  
		Last Modified: Thu, 16 Nov 2023 03:12:14 GMT  
		Size: 69.3 MB (69322889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e233c1968dbb3ae85985bbd8b98ec9454199ca20141c642a7884444c1bc7c7`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 1.6 KB (1580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be3840df58058d3a67a1f4fc3b8987c93be3fba0227a49b9ab08af23db164b3`  
		Last Modified: Thu, 16 Nov 2023 05:38:22 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64072f71e3f7e1d01b75b904e8cb73988c110ba09d61072634272c1c6e0192f5`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be28c184970d229ba318ac93ef72165a50289b21f6822ac961e779c3f7594b2`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fadbb7cc6286a3cc2b7fc543b3a14f8c4527bd76a612ec0e0f971acc57a35a48`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f55e1de34150b2a36b3073acb80b8a2be69b440782f880794957e941f29220`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.7 MB (1661568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be73ad07c8ccee0635f69cb11e8c37458731e7c8791d6b55e3c75a04b533099`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.5-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:8e5bb4c8c32d947b3fa0e530ecb103d4dc813be81cf27e924be9b5171dd1a8a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2113; amd64

### `caddy:2.7.5-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:256d98ebfd54e7da9c594d3a17888987e08a54f31e1a902fdba6062d6475e357
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1983592262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:932ff705341933569835dda3a9df0a381c9efadb23aedbc990ae4c3fe927da37`
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
# Thu, 16 Nov 2023 02:44:31 GMT
ENV GOLANG_VERSION=1.21.4
# Thu, 16 Nov 2023 02:46:51 GMT
RUN $url = 'https://dl.google.com/go/go1.21.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '79e5428e068c912d9cfa6cd115c13549856ec689c1332eac17f5d6122e19d595'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:46:53 GMT
WORKDIR C:\go
# Thu, 16 Nov 2023 05:36:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:36:15 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 16 Nov 2023 05:36:16 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:36:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Nov 2023 05:36:43 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Nov 2023 05:36:44 GMT
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
	-	`sha256:2e99ca1444cc508d00e7f114e5d0ad9c56d99298bd9767a001ab05a1735cacb4`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753e4af07bf1638babc6e18c4a455b8703dfec478e0794970b2e57d76792a281`  
		Last Modified: Thu, 16 Nov 2023 03:11:38 GMT  
		Size: 69.3 MB (69321984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ace7dc382558d5cfabba6fa5df0abb49108d5b6e7ef243a4b4ccfa7639d022`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.6 KB (1572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dee0b52088af84428a19e50ee688425ccee03091d9de2d42ab608d6f4988b90`  
		Last Modified: Thu, 16 Nov 2023 05:38:42 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae08626268dc4e22e38977aa0284b4f4e8aa2a88d8dbf3cfe61c9ffc10292d3`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12154a346b5aa10235e1da2e2c14f346f6de03387fabad1e8b0df50ce81588e5`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33ca4e95a635026944c3bc5da0516b66036a17f0f1a41f8bc2cccfd4afd1015`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37d2fb80d01142c2f56374c7be06d04ac0ddebd778ee3e052d6e627969b6af7`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.7 MB (1667548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41cc79b0b9e584ff384ef15b6bd7d7f1f12e5e73e9105b3e89537f183c38d8d`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.5-windowsservercore`

```console
$ docker pull caddy@sha256:b2a860f9d095b10b5613cfd76162decff7840f5881e3c5ecf4e01d29d829c405
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.5122; amd64
	-	windows version 10.0.20348.2113; amd64

### `caddy:2.7.5-windowsservercore` - windows version 10.0.17763.5122; amd64

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

### `caddy:2.7.5-windowsservercore` - windows version 10.0.20348.2113; amd64

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

## `caddy:2.7.5-windowsservercore-1809`

```console
$ docker pull caddy@sha256:2e8fbf0e299d85c14b2ac578c2ff6ee6f32e2e0c7dbd4afd5f683286575971d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `caddy:2.7.5-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

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

## `caddy:2.7.5-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:7302fa54b56c8f2363f0caf1ac496c297c9eda88207a05836e5e06c40272769b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2113; amd64

### `caddy:2.7.5-windowsservercore-ltsc2022` - windows version 10.0.20348.2113; amd64

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

## `caddy:alpine`

```console
$ docker pull caddy@sha256:8e3595ce7a7ebd91a4e91eb41ee367a10e18eb9a711fb28e47f611a7882b3dcc
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
$ docker pull caddy@sha256:5b9c67db8969d2d07fbbea52156ed4a9d59c6b20452e5f230c230a686b60c426
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
$ docker pull caddy@sha256:9557c75b38fa3d68dee8dc5098bacb77894db187429baffcf2028f41edd5686e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76955142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70f74c1f483f810509bfd9c4187e0a600e5a9e8aa2ca801acd27e9cc06aa8d2e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:10:40 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 18:05:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:20:24 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:20:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:20:35 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:20:35 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:20:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:20:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:20:36 GMT
WORKDIR /go
# Tue, 07 Nov 2023 20:44:48 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 20:44:48 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 20:44:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 20:44:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 20:44:50 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834bccaa730c985b202b64916ba9cbab707b8a165cece04b8aea3801d6a75741`  
		Last Modified: Sat, 21 Oct 2023 03:10:51 GMT  
		Size: 284.7 KB (284695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bde6e5b785726fea08cb0fb123a90298ceca5cbdc7f267aec8af550c401a2f6`  
		Last Modified: Tue, 07 Nov 2023 20:26:52 GMT  
		Size: 67.0 MB (66995661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebe3be3b56eef1186e8ed89cfaaacf25685600944b44bcdbbd57eb8c8d188e4`  
		Last Modified: Tue, 07 Nov 2023 20:26:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2104133a0e423dca65ea3889907e07d16f2aee507a0b4e6c113befd233f3376e`  
		Last Modified: Tue, 07 Nov 2023 20:45:08 GMT  
		Size: 5.0 MB (4970027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3223ac085d84a7150dcade2bc8258b726591b749677608a2b7e3a02664a48ba5`  
		Last Modified: Tue, 07 Nov 2023 20:45:07 GMT  
		Size: 1.3 MB (1302232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3306c1ee0dab13ecea29b0e17a898223583940e47acc99449853e9e59435f3`  
		Last Modified: Tue, 07 Nov 2023 20:45:07 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:925051dfec44d86d69116ecf542f98f048d16edc30ee04e84dd0f94b8a306f28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75395073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:337623b638f4d83149457aa62bc5b13dff2de821cac1d7a7deb4b0eba81c383c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:43:17 GMT
RUN apk add --no-cache ca-certificates
# Tue, 07 Nov 2023 20:49:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:49:19 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:49:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:49:36 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:49:36 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:49:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:49:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:49:37 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:12:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:12:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:12:40 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:12:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:12:40 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:12:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:12:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:12:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4459abd186485ffcfbc9a0cc16ba7fc77e7b8af5dd55624328e90ec67ef669`  
		Last Modified: Sat, 21 Oct 2023 00:43:27 GMT  
		Size: 284.9 KB (284882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e47353e44109dd9c41cf34c24ec76dc67e7767decf78622589a90a58c3b2f4`  
		Last Modified: Tue, 07 Nov 2023 20:55:24 GMT  
		Size: 65.8 MB (65751371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed03a7f93d0719301c31ce952f21b9a5a31d7a50775d4ee8bc1070f1ce19f9f`  
		Last Modified: Tue, 07 Nov 2023 20:55:04 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c4b96bb9b7fb0e5321265d67484456c37c1fbd1d5e2565c4f9225f9989acaf`  
		Last Modified: Tue, 07 Nov 2023 21:13:02 GMT  
		Size: 5.0 MB (4964302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82c013a69236b77e239aa51756075002025bfab6a1124e524c8c4f855b72142`  
		Last Modified: Tue, 07 Nov 2023 21:13:02 GMT  
		Size: 1.2 MB (1248664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856961b563a2d5414382e81b6e6a0f242bf2a09bb03623ff004cc79275c9b02c`  
		Last Modified: Tue, 07 Nov 2023 21:13:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:c3408f987d7ee9eedb1a5fcefc1cdf4b24092224fdc2d91a0aae5e4b0ad1e1f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74692592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7150e3216cb69f9c924809d80e3f784b9e25038c5c743f8e415853df8163fd0`
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
# Tue, 07 Nov 2023 21:00:37 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 21:00:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 21:00:51 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 21:00:51 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 21:00:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:00:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 21:00:52 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:25:34 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:25:34 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:25:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:25:36 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:25:36 GMT
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
	-	`sha256:4a3debef18506403ac44cc4950a8cbaaea2e9d311ae1a83607be6f7b78b291ce`  
		Last Modified: Tue, 07 Nov 2023 21:07:30 GMT  
		Size: 65.8 MB (65750717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce90421070593b8c5625d529316d162aac0bcfd55fc9e7507b337aed33c64191`  
		Last Modified: Tue, 07 Nov 2023 21:07:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc6fcb2c4fc6a718864e032be82c1edac9d3564e3b7a5833d5f1c1879365074`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 4.5 MB (4511246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91736d5dba9b84ca32af89f184018cf79348d96d127c913d2721ef9a62c5031`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 1.2 MB (1246088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc61b28fe019881fc188747ffde817dc4796c027b44cb91541a4cb9b08714cf`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b843e7253f9266dbfe42a8aa6ed190a23d4c10856ea0ab900fba06faf579e47f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73974255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b375a225af66400861808f202e662bafd23e07644f836d4e47c6d399b765686d`
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
# Tue, 07 Nov 2023 20:39:55 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:40:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:40:05 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:40:05 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:40:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:40:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:40:06 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:02:44 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:02:44 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:02:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:02:45 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:02:45 GMT
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
	-	`sha256:f9e3860c59e00c3164218e7e9c694435e2bcaaf14693bbc68c2a02a882bcc6a2`  
		Last Modified: Tue, 07 Nov 2023 20:45:13 GMT  
		Size: 64.1 MB (64088686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e79fdc38632695ae6832600d13ce667f701f785944433806d5fbf89a90b675`  
		Last Modified: Tue, 07 Nov 2023 20:45:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f0a09267a67162a19517c78b4e687814d8f7b56bd3f768cada6f09460a11c6`  
		Last Modified: Tue, 07 Nov 2023 21:03:01 GMT  
		Size: 5.1 MB (5068431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5a0da72908eb54180139e187b047089c01454fc561d10071e004ddddbc83b7`  
		Last Modified: Tue, 07 Nov 2023 21:03:01 GMT  
		Size: 1.2 MB (1198449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c321b6ea80f52f37c190337f940f0c24d98385d9a2311b30680a11ff757a30f`  
		Last Modified: Tue, 07 Nov 2023 21:03:00 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:4206943b7073e21d109937a4da710faadb4c2d68b06eed13cca7a2e81a427ed0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74200658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ad7628f7abe471737f92d250481b6d37b0dbc08b27f4fecd6de4b7069255fce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:50:06 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 13:54:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:17:41 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 21:18:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 21:18:05 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 21:18:06 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 21:18:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:18:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 21:18:08 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:43:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:43:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:43:40 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:43:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:43:41 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:43:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:43:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:43:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ea699c459f4e83d317f31dad3d23c45cc29bbd728f76aa22bd9e4a8180feb8`  
		Last Modified: Sat, 21 Oct 2023 00:50:20 GMT  
		Size: 286.7 KB (286665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f7b3697956c8adf732de1fa607b670ec20dad24d26aa13bdfd9b275c65ab7e`  
		Last Modified: Tue, 07 Nov 2023 21:25:46 GMT  
		Size: 64.1 MB (64111773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f1720227a74244550a3b19be823a0538279f71347eea9e055bc39b87306e09`  
		Last Modified: Tue, 07 Nov 2023 21:25:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5aa813cd8b314d1ecc000832dd9d9a65d87b48fe12a3e26e8973a24739e1e5d`  
		Last Modified: Tue, 07 Nov 2023 21:44:02 GMT  
		Size: 5.3 MB (5268975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526c725b224548c8658f358c73e89e88e8e4ed758879e446da57649f8147caa3`  
		Last Modified: Tue, 07 Nov 2023 21:44:01 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5ec0b117cae64f834ae1c8a5f1c6e2eb7d03ed218ac12f9e531fb65d2749ae`  
		Last Modified: Tue, 07 Nov 2023 21:44:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:01d8af8337066c19a93a4af95f039f93092c42c25958cb75f773287862af55fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76087350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45f25b6ed469e7fd4e3d10476165542d74cc1ff9aa294642362d158ea159c841`
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
# Tue, 07 Nov 2023 20:43:18 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:43:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:43:36 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:43:36 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:43:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:43:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:43:37 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:08:19 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:08:19 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:08:20 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:08:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:08:20 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:08:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:08:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:08:21 GMT
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
	-	`sha256:72d99582ceb0709a8c9a1d5fdc62f431b171ef30aafa94a2f14cdc818695abc2`  
		Last Modified: Tue, 07 Nov 2023 20:50:45 GMT  
		Size: 66.2 MB (66209518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd3acc2cfafbeca6b9582dca1e5dca9862e6059e686d6fd717790f4353277cf`  
		Last Modified: Tue, 07 Nov 2023 20:50:34 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad32e6427b3c189cb8976ef70af84e8e86a742134fbfcc46ce989b710509dfc`  
		Last Modified: Tue, 07 Nov 2023 21:08:48 GMT  
		Size: 5.1 MB (5114684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d837cb4f1c5fec0ee05235ea0bb20b16067e00a6f0494f88afa5fb527b5f790`  
		Last Modified: Tue, 07 Nov 2023 21:08:47 GMT  
		Size: 1.3 MB (1262388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf5bb743910ff919d1d7c652a4eeda2079fef5385f4c212839b9345c940c370`  
		Last Modified: Tue, 07 Nov 2023 21:08:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:823c52d733e025f2f7a994e81853c644a8cb7fc8e2cfaf1759cfbd9f42981bae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2154235329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e51a76e2131305dc407d432736a885084ead87fe0cc9c9a227736e6799405b0`
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
# Thu, 16 Nov 2023 02:49:42 GMT
ENV GOLANG_VERSION=1.21.4
# Thu, 16 Nov 2023 02:52:53 GMT
RUN $url = 'https://dl.google.com/go/go1.21.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '79e5428e068c912d9cfa6cd115c13549856ec689c1332eac17f5d6122e19d595'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:52:55 GMT
WORKDIR C:\go
# Thu, 16 Nov 2023 05:34:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:34:44 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 16 Nov 2023 05:34:45 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:34:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Nov 2023 05:36:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Nov 2023 05:36:01 GMT
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
	-	`sha256:c30930da8ed1e8bdc54250c940331ca68cda0bfb62284a10c659fbd0768848ea`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d113e76a38d50789cec61e62343c448b0f781f2edc2150f8abe914796df72325`  
		Last Modified: Thu, 16 Nov 2023 03:12:14 GMT  
		Size: 69.3 MB (69322889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e233c1968dbb3ae85985bbd8b98ec9454199ca20141c642a7884444c1bc7c7`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 1.6 KB (1580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be3840df58058d3a67a1f4fc3b8987c93be3fba0227a49b9ab08af23db164b3`  
		Last Modified: Thu, 16 Nov 2023 05:38:22 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64072f71e3f7e1d01b75b904e8cb73988c110ba09d61072634272c1c6e0192f5`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be28c184970d229ba318ac93ef72165a50289b21f6822ac961e779c3f7594b2`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fadbb7cc6286a3cc2b7fc543b3a14f8c4527bd76a612ec0e0f971acc57a35a48`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f55e1de34150b2a36b3073acb80b8a2be69b440782f880794957e941f29220`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.7 MB (1661568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be73ad07c8ccee0635f69cb11e8c37458731e7c8791d6b55e3c75a04b533099`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:256d98ebfd54e7da9c594d3a17888987e08a54f31e1a902fdba6062d6475e357
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1983592262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:932ff705341933569835dda3a9df0a381c9efadb23aedbc990ae4c3fe927da37`
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
# Thu, 16 Nov 2023 02:44:31 GMT
ENV GOLANG_VERSION=1.21.4
# Thu, 16 Nov 2023 02:46:51 GMT
RUN $url = 'https://dl.google.com/go/go1.21.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '79e5428e068c912d9cfa6cd115c13549856ec689c1332eac17f5d6122e19d595'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:46:53 GMT
WORKDIR C:\go
# Thu, 16 Nov 2023 05:36:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:36:15 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 16 Nov 2023 05:36:16 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:36:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Nov 2023 05:36:43 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Nov 2023 05:36:44 GMT
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
	-	`sha256:2e99ca1444cc508d00e7f114e5d0ad9c56d99298bd9767a001ab05a1735cacb4`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753e4af07bf1638babc6e18c4a455b8703dfec478e0794970b2e57d76792a281`  
		Last Modified: Thu, 16 Nov 2023 03:11:38 GMT  
		Size: 69.3 MB (69321984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ace7dc382558d5cfabba6fa5df0abb49108d5b6e7ef243a4b4ccfa7639d022`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.6 KB (1572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dee0b52088af84428a19e50ee688425ccee03091d9de2d42ab608d6f4988b90`  
		Last Modified: Thu, 16 Nov 2023 05:38:42 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae08626268dc4e22e38977aa0284b4f4e8aa2a88d8dbf3cfe61c9ffc10292d3`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12154a346b5aa10235e1da2e2c14f346f6de03387fabad1e8b0df50ce81588e5`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33ca4e95a635026944c3bc5da0516b66036a17f0f1a41f8bc2cccfd4afd1015`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37d2fb80d01142c2f56374c7be06d04ac0ddebd778ee3e052d6e627969b6af7`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.7 MB (1667548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41cc79b0b9e584ff384ef15b6bd7d7f1f12e5e73e9105b3e89537f183c38d8d`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:a51593964dcf5b43b549589e0e77d0dec7a1c3491fb5054a8e1e93e22505d1a6
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
$ docker pull caddy@sha256:9557c75b38fa3d68dee8dc5098bacb77894db187429baffcf2028f41edd5686e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76955142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70f74c1f483f810509bfd9c4187e0a600e5a9e8aa2ca801acd27e9cc06aa8d2e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:10:40 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 18:05:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:20:24 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:20:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:20:35 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:20:35 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:20:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:20:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:20:36 GMT
WORKDIR /go
# Tue, 07 Nov 2023 20:44:48 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 20:44:48 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 20:44:48 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 20:44:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 20:44:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 20:44:50 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834bccaa730c985b202b64916ba9cbab707b8a165cece04b8aea3801d6a75741`  
		Last Modified: Sat, 21 Oct 2023 03:10:51 GMT  
		Size: 284.7 KB (284695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bde6e5b785726fea08cb0fb123a90298ceca5cbdc7f267aec8af550c401a2f6`  
		Last Modified: Tue, 07 Nov 2023 20:26:52 GMT  
		Size: 67.0 MB (66995661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebe3be3b56eef1186e8ed89cfaaacf25685600944b44bcdbbd57eb8c8d188e4`  
		Last Modified: Tue, 07 Nov 2023 20:26:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2104133a0e423dca65ea3889907e07d16f2aee507a0b4e6c113befd233f3376e`  
		Last Modified: Tue, 07 Nov 2023 20:45:08 GMT  
		Size: 5.0 MB (4970027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3223ac085d84a7150dcade2bc8258b726591b749677608a2b7e3a02664a48ba5`  
		Last Modified: Tue, 07 Nov 2023 20:45:07 GMT  
		Size: 1.3 MB (1302232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3306c1ee0dab13ecea29b0e17a898223583940e47acc99449853e9e59435f3`  
		Last Modified: Tue, 07 Nov 2023 20:45:07 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:925051dfec44d86d69116ecf542f98f048d16edc30ee04e84dd0f94b8a306f28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75395073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:337623b638f4d83149457aa62bc5b13dff2de821cac1d7a7deb4b0eba81c383c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:43:17 GMT
RUN apk add --no-cache ca-certificates
# Tue, 07 Nov 2023 20:49:19 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:49:19 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:49:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:49:36 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:49:36 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:49:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:49:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:49:37 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:12:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:12:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:12:40 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:12:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:12:40 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:12:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:12:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:12:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4459abd186485ffcfbc9a0cc16ba7fc77e7b8af5dd55624328e90ec67ef669`  
		Last Modified: Sat, 21 Oct 2023 00:43:27 GMT  
		Size: 284.9 KB (284882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e47353e44109dd9c41cf34c24ec76dc67e7767decf78622589a90a58c3b2f4`  
		Last Modified: Tue, 07 Nov 2023 20:55:24 GMT  
		Size: 65.8 MB (65751371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed03a7f93d0719301c31ce952f21b9a5a31d7a50775d4ee8bc1070f1ce19f9f`  
		Last Modified: Tue, 07 Nov 2023 20:55:04 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c4b96bb9b7fb0e5321265d67484456c37c1fbd1d5e2565c4f9225f9989acaf`  
		Last Modified: Tue, 07 Nov 2023 21:13:02 GMT  
		Size: 5.0 MB (4964302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82c013a69236b77e239aa51756075002025bfab6a1124e524c8c4f855b72142`  
		Last Modified: Tue, 07 Nov 2023 21:13:02 GMT  
		Size: 1.2 MB (1248664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856961b563a2d5414382e81b6e6a0f242bf2a09bb03623ff004cc79275c9b02c`  
		Last Modified: Tue, 07 Nov 2023 21:13:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:c3408f987d7ee9eedb1a5fcefc1cdf4b24092224fdc2d91a0aae5e4b0ad1e1f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74692592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7150e3216cb69f9c924809d80e3f784b9e25038c5c743f8e415853df8163fd0`
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
# Tue, 07 Nov 2023 21:00:37 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 21:00:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 21:00:51 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 21:00:51 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 21:00:51 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:00:52 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 21:00:52 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:25:34 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:25:34 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:25:34 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:25:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:25:36 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:25:36 GMT
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
	-	`sha256:4a3debef18506403ac44cc4950a8cbaaea2e9d311ae1a83607be6f7b78b291ce`  
		Last Modified: Tue, 07 Nov 2023 21:07:30 GMT  
		Size: 65.8 MB (65750717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce90421070593b8c5625d529316d162aac0bcfd55fc9e7507b337aed33c64191`  
		Last Modified: Tue, 07 Nov 2023 21:07:14 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc6fcb2c4fc6a718864e032be82c1edac9d3564e3b7a5833d5f1c1879365074`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 4.5 MB (4511246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91736d5dba9b84ca32af89f184018cf79348d96d127c913d2721ef9a62c5031`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 1.2 MB (1246088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc61b28fe019881fc188747ffde817dc4796c027b44cb91541a4cb9b08714cf`  
		Last Modified: Tue, 07 Nov 2023 21:25:53 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b843e7253f9266dbfe42a8aa6ed190a23d4c10856ea0ab900fba06faf579e47f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73974255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b375a225af66400861808f202e662bafd23e07644f836d4e47c6d399b765686d`
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
# Tue, 07 Nov 2023 20:39:55 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:40:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:40:05 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:40:05 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:40:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:40:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:40:06 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:02:44 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:02:44 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:02:44 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:02:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:02:45 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:02:45 GMT
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
	-	`sha256:f9e3860c59e00c3164218e7e9c694435e2bcaaf14693bbc68c2a02a882bcc6a2`  
		Last Modified: Tue, 07 Nov 2023 20:45:13 GMT  
		Size: 64.1 MB (64088686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e79fdc38632695ae6832600d13ce667f701f785944433806d5fbf89a90b675`  
		Last Modified: Tue, 07 Nov 2023 20:45:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f0a09267a67162a19517c78b4e687814d8f7b56bd3f768cada6f09460a11c6`  
		Last Modified: Tue, 07 Nov 2023 21:03:01 GMT  
		Size: 5.1 MB (5068431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5a0da72908eb54180139e187b047089c01454fc561d10071e004ddddbc83b7`  
		Last Modified: Tue, 07 Nov 2023 21:03:01 GMT  
		Size: 1.2 MB (1198449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c321b6ea80f52f37c190337f940f0c24d98385d9a2311b30680a11ff757a30f`  
		Last Modified: Tue, 07 Nov 2023 21:03:00 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:4206943b7073e21d109937a4da710faadb4c2d68b06eed13cca7a2e81a427ed0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74200658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ad7628f7abe471737f92d250481b6d37b0dbc08b27f4fecd6de4b7069255fce`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:50:06 GMT
RUN apk add --no-cache ca-certificates
# Wed, 01 Nov 2023 13:54:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:17:41 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 21:18:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 21:18:05 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 21:18:06 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 21:18:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 21:18:08 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 21:18:08 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:43:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:43:39 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:43:40 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:43:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:43:41 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:43:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:43:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:43:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ea699c459f4e83d317f31dad3d23c45cc29bbd728f76aa22bd9e4a8180feb8`  
		Last Modified: Sat, 21 Oct 2023 00:50:20 GMT  
		Size: 286.7 KB (286665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f7b3697956c8adf732de1fa607b670ec20dad24d26aa13bdfd9b275c65ab7e`  
		Last Modified: Tue, 07 Nov 2023 21:25:46 GMT  
		Size: 64.1 MB (64111773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f1720227a74244550a3b19be823a0538279f71347eea9e055bc39b87306e09`  
		Last Modified: Tue, 07 Nov 2023 21:25:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5aa813cd8b314d1ecc000832dd9d9a65d87b48fe12a3e26e8973a24739e1e5d`  
		Last Modified: Tue, 07 Nov 2023 21:44:02 GMT  
		Size: 5.3 MB (5268975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526c725b224548c8658f358c73e89e88e8e4ed758879e446da57649f8147caa3`  
		Last Modified: Tue, 07 Nov 2023 21:44:01 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5ec0b117cae64f834ae1c8a5f1c6e2eb7d03ed218ac12f9e531fb65d2749ae`  
		Last Modified: Tue, 07 Nov 2023 21:44:01 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:01d8af8337066c19a93a4af95f039f93092c42c25958cb75f773287862af55fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76087350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45f25b6ed469e7fd4e3d10476165542d74cc1ff9aa294642362d158ea159c841`
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
# Tue, 07 Nov 2023 20:43:18 GMT
ENV GOLANG_VERSION=1.21.4
# Tue, 07 Nov 2023 20:43:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			url='https://dl.google.com/go/go1.21.4.linux-amd64.tar.gz'; 			sha256='73cac0215254d0c7d1241fa40837851f3b9a8a742d0b54714cbdfb3feaf8f0af'; 			;; 		'armhf') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'armv7') 			url='https://dl.google.com/go/go1.21.4.linux-armv6l.tar.gz'; 			sha256='6c62e89113750cc77c498194d13a03fadfda22bd2c7d44e8a826fd354db60252'; 			;; 		'aarch64') 			url='https://dl.google.com/go/go1.21.4.linux-arm64.tar.gz'; 			sha256='ce1983a7289856c3a918e1fd26d41e072cc39f928adfb11ba1896440849b95da'; 			;; 		'x86') 			url='https://dl.google.com/go/go1.21.4.linux-386.tar.gz'; 			sha256='64d3e5d295806e137c9e39d1e1f10b00a30fcd5c2f230d72b3298f579bb3c89a'; 			;; 		'ppc64le') 			url='https://dl.google.com/go/go1.21.4.linux-ppc64le.tar.gz'; 			sha256='2c63b36d2adcfb22013102a2ee730f058ec2f93b9f27479793c80b2e3641783f'; 			;; 		'riscv64') 			url='https://dl.google.com/go/go1.21.4.linux-riscv64.tar.gz'; 			sha256='9695edd2109544b364daddb32816f5c7980f1f48b8490c51fa2c167f5b2eca48'; 			;; 		's390x') 			url='https://dl.google.com/go/go1.21.4.linux-s390x.tar.gz'; 			sha256='7a75ba4afc7a96058ca65903d994cd862381825d7dca12b2183f087c757c26c0'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.21.4.src.tar.gz'; 		sha256='47b26a83d2b65a3c1c1bcace273b69bee49a7a7b5168a7604ded3d26a37bd787'; 		echo >&2; 		echo >&2 "warning: current architecture ($arch) does not have a compatible Go binary release; will be building from source"; 		echo >&2; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Nov 2023 20:43:36 GMT
ENV GOTOOLCHAIN=local
# Tue, 07 Nov 2023 20:43:36 GMT
ENV GOPATH=/go
# Tue, 07 Nov 2023 20:43:37 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Nov 2023 20:43:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 07 Nov 2023 20:43:37 GMT
WORKDIR /go
# Tue, 07 Nov 2023 21:08:19 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 07 Nov 2023 21:08:19 GMT
ENV XCADDY_VERSION=v0.3.5
# Tue, 07 Nov 2023 21:08:20 GMT
ENV CADDY_VERSION=v2.7.5
# Tue, 07 Nov 2023 21:08:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 07 Nov 2023 21:08:20 GMT
ENV XCADDY_SETCAP=1
# Tue, 07 Nov 2023 21:08:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 07 Nov 2023 21:08:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 07 Nov 2023 21:08:21 GMT
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
	-	`sha256:72d99582ceb0709a8c9a1d5fdc62f431b171ef30aafa94a2f14cdc818695abc2`  
		Last Modified: Tue, 07 Nov 2023 20:50:45 GMT  
		Size: 66.2 MB (66209518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd3acc2cfafbeca6b9582dca1e5dca9862e6059e686d6fd717790f4353277cf`  
		Last Modified: Tue, 07 Nov 2023 20:50:34 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad32e6427b3c189cb8976ef70af84e8e86a742134fbfcc46ce989b710509dfc`  
		Last Modified: Tue, 07 Nov 2023 21:08:48 GMT  
		Size: 5.1 MB (5114684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d837cb4f1c5fec0ee05235ea0bb20b16067e00a6f0494f88afa5fb527b5f790`  
		Last Modified: Tue, 07 Nov 2023 21:08:47 GMT  
		Size: 1.3 MB (1262388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf5bb743910ff919d1d7c652a4eeda2079fef5385f4c212839b9345c940c370`  
		Last Modified: Tue, 07 Nov 2023 21:08:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:db8add82121fb31a1612a7e34b5af6a2180acc560a75b5c295c6421ec5854064
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull caddy@sha256:823c52d733e025f2f7a994e81853c644a8cb7fc8e2cfaf1759cfbd9f42981bae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2154235329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e51a76e2131305dc407d432736a885084ead87fe0cc9c9a227736e6799405b0`
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
# Thu, 16 Nov 2023 02:49:42 GMT
ENV GOLANG_VERSION=1.21.4
# Thu, 16 Nov 2023 02:52:53 GMT
RUN $url = 'https://dl.google.com/go/go1.21.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '79e5428e068c912d9cfa6cd115c13549856ec689c1332eac17f5d6122e19d595'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:52:55 GMT
WORKDIR C:\go
# Thu, 16 Nov 2023 05:34:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:34:44 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 16 Nov 2023 05:34:45 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:34:46 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Nov 2023 05:36:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Nov 2023 05:36:01 GMT
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
	-	`sha256:c30930da8ed1e8bdc54250c940331ca68cda0bfb62284a10c659fbd0768848ea`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d113e76a38d50789cec61e62343c448b0f781f2edc2150f8abe914796df72325`  
		Last Modified: Thu, 16 Nov 2023 03:12:14 GMT  
		Size: 69.3 MB (69322889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e233c1968dbb3ae85985bbd8b98ec9454199ca20141c642a7884444c1bc7c7`  
		Last Modified: Thu, 16 Nov 2023 03:11:53 GMT  
		Size: 1.6 KB (1580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be3840df58058d3a67a1f4fc3b8987c93be3fba0227a49b9ab08af23db164b3`  
		Last Modified: Thu, 16 Nov 2023 05:38:22 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64072f71e3f7e1d01b75b904e8cb73988c110ba09d61072634272c1c6e0192f5`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be28c184970d229ba318ac93ef72165a50289b21f6822ac961e779c3f7594b2`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fadbb7cc6286a3cc2b7fc543b3a14f8c4527bd76a612ec0e0f971acc57a35a48`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f55e1de34150b2a36b3073acb80b8a2be69b440782f880794957e941f29220`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.7 MB (1661568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be73ad07c8ccee0635f69cb11e8c37458731e7c8791d6b55e3c75a04b533099`  
		Last Modified: Thu, 16 Nov 2023 05:38:20 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:8e5bb4c8c32d947b3fa0e530ecb103d4dc813be81cf27e924be9b5171dd1a8a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2113; amd64

### `caddy:builder-windowsservercore-ltsc2022` - windows version 10.0.20348.2113; amd64

```console
$ docker pull caddy@sha256:256d98ebfd54e7da9c594d3a17888987e08a54f31e1a902fdba6062d6475e357
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1983592262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:932ff705341933569835dda3a9df0a381c9efadb23aedbc990ae4c3fe927da37`
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
# Thu, 16 Nov 2023 02:44:31 GMT
ENV GOLANG_VERSION=1.21.4
# Thu, 16 Nov 2023 02:46:51 GMT
RUN $url = 'https://dl.google.com/go/go1.21.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '79e5428e068c912d9cfa6cd115c13549856ec689c1332eac17f5d6122e19d595'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Nov 2023 02:46:53 GMT
WORKDIR C:\go
# Thu, 16 Nov 2023 05:36:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 05:36:15 GMT
ENV XCADDY_VERSION=v0.3.5
# Thu, 16 Nov 2023 05:36:16 GMT
ENV CADDY_VERSION=v2.7.5
# Thu, 16 Nov 2023 05:36:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Nov 2023 05:36:43 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e7a7b91439669b96bd3dbe347d9fcc84767c02c68ed451b7b80c8d3063c9e4ae2531d4bba0ee51d7d78be29371d36bac56412e39144b92e781e253f265a3883c')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Nov 2023 05:36:44 GMT
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
	-	`sha256:2e99ca1444cc508d00e7f114e5d0ad9c56d99298bd9767a001ab05a1735cacb4`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753e4af07bf1638babc6e18c4a455b8703dfec478e0794970b2e57d76792a281`  
		Last Modified: Thu, 16 Nov 2023 03:11:38 GMT  
		Size: 69.3 MB (69321984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ace7dc382558d5cfabba6fa5df0abb49108d5b6e7ef243a4b4ccfa7639d022`  
		Last Modified: Thu, 16 Nov 2023 03:11:16 GMT  
		Size: 1.6 KB (1572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dee0b52088af84428a19e50ee688425ccee03091d9de2d42ab608d6f4988b90`  
		Last Modified: Thu, 16 Nov 2023 05:38:42 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae08626268dc4e22e38977aa0284b4f4e8aa2a88d8dbf3cfe61c9ffc10292d3`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12154a346b5aa10235e1da2e2c14f346f6de03387fabad1e8b0df50ce81588e5`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33ca4e95a635026944c3bc5da0516b66036a17f0f1a41f8bc2cccfd4afd1015`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37d2fb80d01142c2f56374c7be06d04ac0ddebd778ee3e052d6e627969b6af7`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.7 MB (1667548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41cc79b0b9e584ff384ef15b6bd7d7f1f12e5e73e9105b3e89537f183c38d8d`  
		Last Modified: Thu, 16 Nov 2023 05:38:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:279a5ff568ff6c9e6185a6151e065aacb01c0f275b85f52dd950ac9ae204d8ab
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
