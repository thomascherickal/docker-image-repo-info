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
-	[`caddy:2.7.3`](#caddy273)
-	[`caddy:2.7.3-alpine`](#caddy273-alpine)
-	[`caddy:2.7.3-builder`](#caddy273-builder)
-	[`caddy:2.7.3-builder-alpine`](#caddy273-builder-alpine)
-	[`caddy:2.7.3-builder-windowsservercore-1809`](#caddy273-builder-windowsservercore-1809)
-	[`caddy:2.7.3-builder-windowsservercore-ltsc2022`](#caddy273-builder-windowsservercore-ltsc2022)
-	[`caddy:2.7.3-windowsservercore`](#caddy273-windowsservercore)
-	[`caddy:2.7.3-windowsservercore-1809`](#caddy273-windowsservercore-1809)
-	[`caddy:2.7.3-windowsservercore-ltsc2022`](#caddy273-windowsservercore-ltsc2022)
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
$ docker pull caddy@sha256:6c60e52f0acf862774d17f362aadc4895667d42b24ca6e74ee1e7f09a1363424
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4737; amd64
	-	windows version 10.0.20348.1906; amd64

### `caddy:2` - linux; amd64

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

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:dc698bd1b82521df87ea42fbf48c98d10133ec962497ac80527b65769ceb6a9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17690701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3775ac20cca67f4d547f26f5984a989b9407b0c4129fd6cd86dbb3359249acd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:38:27 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:49:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:49:14 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:49:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:49:16 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:49:16 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:49:18 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:49:18 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:49:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172ef460a93549b8a3e73f6a515bccad93512788d1e8f095e7230ba41967c25a`  
		Last Modified: Wed, 09 Aug 2023 03:38:53 GMT  
		Size: 347.7 KB (347686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7aae78767a581df85fd1a51ccd646619aec320896ca016ef0f05a41b16bcbfe`  
		Last Modified: Mon, 14 Aug 2023 17:49:36 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5244db1c019e66038874df2b8b92c74437f6d355802bfccada90c9d8bd8d29`  
		Last Modified: Mon, 14 Aug 2023 17:49:38 GMT  
		Size: 14.2 MB (14190701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:e9cb1245e1c134e25a0ec0803e5132ba9ba92d0a4ad85db3f73bd2c3188cf70e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17414619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df6e2a1f4c707dc77276814a27ac22a7b5de268780603d8e08324130e1fc563`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:51:41 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:57:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:57:17 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:57:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:57:20 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:57:20 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:57:21 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:57:21 GMT
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
	-	`sha256:46e1b3e18d5e992f1805072b2d52405d575830bdce21726ef99dea99e31d8277`  
		Last Modified: Mon, 14 Aug 2023 17:57:42 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2b7485982d191f9dc0498d5b940d14df575f36ca66876b92d3ca09ff9386b2`  
		Last Modified: Mon, 14 Aug 2023 17:57:48 GMT  
		Size: 14.2 MB (14163172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:db04154ce5f7a7f4d058567375880cdc6b1a3675095ad576f9886f39f1374afc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17329640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:731c0ae21a974e5708c4a8006250893bca5a2ecad43babf2a0a95a60fc61d6cd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:09:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:39:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:39:19 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:39:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:39:21 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:39:21 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:39:22 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:39:22 GMT
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
	-	`sha256:f7488af8b96c79b6db13955a0302653c4e9f314d0833201984ae06c1ed697f06`  
		Last Modified: Mon, 14 Aug 2023 17:39:41 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9600da6e7e51b9083b29f3c7de592fa45e7765ca5ffe8d2abf7cc99c50578fe`  
		Last Modified: Mon, 14 Aug 2023 17:39:43 GMT  
		Size: 13.6 MB (13630728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

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

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:3b3d4b80e160105a760ad62b32c497245d69676e6053c2a7b61bc5c6fc178fd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.0 MB (17984968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a63d05bc7601e47460ff86bc91380fd9407c0b4886b80836ac3aadb436f68e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:14:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:41:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:41:39 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:41:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:41:43 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:41:43 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:41:44 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:41:44 GMT
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
	-	`sha256:308478977890baa82477ee70a3065fb9da2080efcc95facf1a87ac021b06a8e9`  
		Last Modified: Mon, 14 Aug 2023 17:42:17 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fe1cbba37a3c1c2f6ba50e59e5c238c8d83ffca820ef709108b9e3253af757`  
		Last Modified: Mon, 14 Aug 2023 17:42:19 GMT  
		Size: 14.4 MB (14408320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:1b4a86d284b971594d7e30ef09451be59ba84514b612c87b6406e2dfb8e9e23f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2011958834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ae5f48eae2f949ec09ad9f70ff2c2626318e07111bea5b6622116482ac991b0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 02:59:41 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Aug 2023 02:59:41 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:00:57 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('69d2d73c2514ab5ce4f6a60489c79ce4da0e1d4302c85ab584d0a7a7fd0d034bfe5a5caab78c96ac3383ddd7d2e12c3c41fb47c4716909d2a78d448b0289ccec')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Aug 2023 03:00:58 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Aug 2023 03:00:59 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Aug 2023 03:01:00 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Thu, 10 Aug 2023 03:01:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Aug 2023 03:01:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Aug 2023 03:01:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Aug 2023 03:01:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Aug 2023 03:01:03 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Aug 2023 03:01:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Aug 2023 03:01:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Aug 2023 03:01:06 GMT
EXPOSE 80
# Thu, 10 Aug 2023 03:01:06 GMT
EXPOSE 443
# Thu, 10 Aug 2023 03:01:07 GMT
EXPOSE 443/udp
# Thu, 10 Aug 2023 03:01:08 GMT
EXPOSE 2019
# Thu, 10 Aug 2023 03:03:10 GMT
RUN caddy version
# Thu, 10 Aug 2023 03:03:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907ddb8e2b3b8f440ec855971bf77d521900d3faecd1816d7146d89f1c78f408`  
		Last Modified: Thu, 10 Aug 2023 03:07:15 GMT  
		Size: 469.4 KB (469388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d430330f12b22fcc17a5d114d51ba3bb8e62a55f87b67f939d18651c226f927`  
		Last Modified: Thu, 10 Aug 2023 03:07:15 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd493f43c2fb25a7c8540ea353a098f784a6e8d5fe4e9d070e4a1de796cde96c`  
		Last Modified: Thu, 10 Aug 2023 03:07:18 GMT  
		Size: 15.2 MB (15241515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95b32f0fb8252db266318cca24c13f5eea8b8b3c19405b92f1a8b9199e39c5d`  
		Last Modified: Thu, 10 Aug 2023 03:07:14 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7dbc1767506f0f3f5b4d3a9671f97a723014ae1e38cf8056f6257db7917a88`  
		Last Modified: Thu, 10 Aug 2023 03:07:13 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7905b1f85b201367c5a62618ddc55da9a60cbb3da1da40ab60a88c125a5956`  
		Last Modified: Thu, 10 Aug 2023 03:07:13 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce34081b153cf49ce89b2ff4fc81f54a648cefc5d2dbb0f60048b94ba10f43b`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9622cc1048f5f7259d3263b67dd386c5d70ae4cf0a358c33deb3df8cdb316efd`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b1ca0970bf360a0627a1deae2985b658f54b41758f12f4e5448ed1aee3bc82`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503770a8fe554599aa8e6413082b7cb24d7f1faa328deaf28b34ddb2a294972b`  
		Last Modified: Thu, 10 Aug 2023 03:07:11 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea5eee99969c433a1c2f4d0f7fdc838185350144b9d3f20888c2a53cc6f3563`  
		Last Modified: Thu, 10 Aug 2023 03:07:11 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675093fb34c31fff953a92ee1831f09679783e7d3e1d9ff40a962f346d1dc581`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fd64685610dd5572f21efe3fae8cb13537c9deb6693caf4097bf9ec3b4dabe`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540e52aaf0b1acca0c4a9fbb2a60e5ce4bca2c119fbb3bbd86658186b23e3202`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29819bc504b56dacdb0df898ee58e26d8097802c0a5578cd14d4e3ed0655bde7`  
		Last Modified: Thu, 10 Aug 2023 03:07:09 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2157a412d53cd6d3174744de6c1cf5cb0dd03274fe9b36f749525867e4b9bd2`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cfbf0b65ccf78eb536c8a23f0b92fa148268c1fa4a39c1b19c7d9310e53b8d`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7faedca764204aa914e83a3721476c9a6a7f8177d057021e5a1debb81a436808`  
		Last Modified: Thu, 10 Aug 2023 03:07:09 GMT  
		Size: 268.6 KB (268640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86622825a44d72176deccdf0a5e4c9127ebf8f2591211cbdae585e9977363e8`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:144bc31c96841830b174ed1ff2da09ba18881208aae2efd16b3c850953f762f6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1813356270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02028c6ef8441cbf5181f34f78b4740b60dffff030772882302c9ca39f9a6096`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 03:03:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Aug 2023 03:03:52 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:04:21 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('69d2d73c2514ab5ce4f6a60489c79ce4da0e1d4302c85ab584d0a7a7fd0d034bfe5a5caab78c96ac3383ddd7d2e12c3c41fb47c4716909d2a78d448b0289ccec')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Aug 2023 03:04:21 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Aug 2023 03:04:22 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Aug 2023 03:04:23 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Thu, 10 Aug 2023 03:04:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Aug 2023 03:04:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Aug 2023 03:04:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Aug 2023 03:04:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Aug 2023 03:04:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Aug 2023 03:04:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Aug 2023 03:04:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Aug 2023 03:04:29 GMT
EXPOSE 80
# Thu, 10 Aug 2023 03:04:30 GMT
EXPOSE 443
# Thu, 10 Aug 2023 03:04:31 GMT
EXPOSE 443/udp
# Thu, 10 Aug 2023 03:04:32 GMT
EXPOSE 2019
# Thu, 10 Aug 2023 03:04:47 GMT
RUN caddy version
# Thu, 10 Aug 2023 03:04:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee168d3c6067847c3aef71a2a0dfdc70984b0bb6164086b49da7bd27de3ff3e4`  
		Last Modified: Thu, 10 Aug 2023 03:07:41 GMT  
		Size: 462.1 KB (462122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0efe6e8d5895981c45dc711aa05390379a6f7e5ceea618991435f40db1736c5`  
		Last Modified: Thu, 10 Aug 2023 03:07:40 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c66dfda490f2720f8d21e51546bae9f4e21a4b3b76b29f45e18435544c66a7c`  
		Last Modified: Thu, 10 Aug 2023 03:07:44 GMT  
		Size: 15.2 MB (15227189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67327c2fc33a0a30f2e409ada51c37d6663c07a498c7663987be61f888f7a8`  
		Last Modified: Thu, 10 Aug 2023 03:07:40 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c73910f4e5bd8630e3f4a5c23d004a9f6eff60c9f50af18e4b1d9b5f9ac0aa4`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d17a44e8dc24bdc71a9866c99b7022ca1a00e04acc6bf00dbf794c0550bb79d`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851a0578d2d21e2b22a64fe518454ef0283a718573db4e60e3b4a0121bd4081a`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ab80276792afc4370db678044627f33dabc32a9a987d736686239ed1d85a5b`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dcfba0d938817014a224fd3369379868ad4bd05a910cf582eb5e88ca8630ce`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd3ed16ce737bd3530ec90c77867e59892ce05deebca1a42256c570b86ddf1a`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb186d102ae807e026f9de311625fe281b24e140d91adaa2c46298a163035182`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267fad2b6b29094e45425d6b1d39b3f0a295ee7bbce5489aab9e77a659c7ef09`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608cb1e8b46f127167ebb53ec28593783baa810d0ec8e54a929e2907cea85352`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dadf995868b2bcb1e42a4b48f3df0ccd9a979672da04a75dad7970b567bb793`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4209fa97cbb4a651cae617cf81de393ea0652645a1f00b607c18dfa26834c475`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e65f2bc3967a653972ae76ef447ff72659e620a98280fe5230591a0e7c29cd`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9d8975e744e0f5b82190fc02ef017a7f4e7ffa1dda69f5be10f43ffa554d9e`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef526b9884253387824d19beee5d18eee6650c38429c56acd30286c1ea94da03`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 280.0 KB (280042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0266d9103b52d7b0129a0aa08ddab9c5bdfca0694ed3368c0b9c887941c524a`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:00e7c43c571e7036a06830652d919a83c140041d6f98f0ee30c2764f01b8fd6d
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
$ docker pull caddy@sha256:dc698bd1b82521df87ea42fbf48c98d10133ec962497ac80527b65769ceb6a9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17690701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3775ac20cca67f4d547f26f5984a989b9407b0c4129fd6cd86dbb3359249acd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:38:27 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:49:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:49:14 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:49:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:49:16 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:49:16 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:49:18 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:49:18 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:49:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172ef460a93549b8a3e73f6a515bccad93512788d1e8f095e7230ba41967c25a`  
		Last Modified: Wed, 09 Aug 2023 03:38:53 GMT  
		Size: 347.7 KB (347686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7aae78767a581df85fd1a51ccd646619aec320896ca016ef0f05a41b16bcbfe`  
		Last Modified: Mon, 14 Aug 2023 17:49:36 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5244db1c019e66038874df2b8b92c74437f6d355802bfccada90c9d8bd8d29`  
		Last Modified: Mon, 14 Aug 2023 17:49:38 GMT  
		Size: 14.2 MB (14190701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:e9cb1245e1c134e25a0ec0803e5132ba9ba92d0a4ad85db3f73bd2c3188cf70e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17414619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df6e2a1f4c707dc77276814a27ac22a7b5de268780603d8e08324130e1fc563`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:51:41 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:57:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:57:17 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:57:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:57:20 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:57:20 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:57:21 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:57:21 GMT
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
	-	`sha256:46e1b3e18d5e992f1805072b2d52405d575830bdce21726ef99dea99e31d8277`  
		Last Modified: Mon, 14 Aug 2023 17:57:42 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2b7485982d191f9dc0498d5b940d14df575f36ca66876b92d3ca09ff9386b2`  
		Last Modified: Mon, 14 Aug 2023 17:57:48 GMT  
		Size: 14.2 MB (14163172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:db04154ce5f7a7f4d058567375880cdc6b1a3675095ad576f9886f39f1374afc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17329640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:731c0ae21a974e5708c4a8006250893bca5a2ecad43babf2a0a95a60fc61d6cd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:09:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:39:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:39:19 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:39:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:39:21 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:39:21 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:39:22 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:39:22 GMT
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
	-	`sha256:f7488af8b96c79b6db13955a0302653c4e9f314d0833201984ae06c1ed697f06`  
		Last Modified: Mon, 14 Aug 2023 17:39:41 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9600da6e7e51b9083b29f3c7de592fa45e7765ca5ffe8d2abf7cc99c50578fe`  
		Last Modified: Mon, 14 Aug 2023 17:39:43 GMT  
		Size: 13.6 MB (13630728 bytes)  
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
$ docker pull caddy@sha256:3b3d4b80e160105a760ad62b32c497245d69676e6053c2a7b61bc5c6fc178fd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.0 MB (17984968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a63d05bc7601e47460ff86bc91380fd9407c0b4886b80836ac3aadb436f68e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:14:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:41:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:41:39 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:41:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:41:43 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:41:43 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:41:44 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:41:44 GMT
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
	-	`sha256:308478977890baa82477ee70a3065fb9da2080efcc95facf1a87ac021b06a8e9`  
		Last Modified: Mon, 14 Aug 2023 17:42:17 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fe1cbba37a3c1c2f6ba50e59e5c238c8d83ffca820ef709108b9e3253af757`  
		Last Modified: Mon, 14 Aug 2023 17:42:19 GMT  
		Size: 14.4 MB (14408320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:b93978cf962da183e6d11a754d51de5f033da2708c588c9ba27cd0ce2c3b582c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4737; amd64
	-	windows version 10.0.20348.1906; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:7abb7723020bab7b367d33786efcfca5d4a4f884ec306308d4a5513f14cdc20c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110901544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e24e6bda832eff522a3ea76a20f3e8055f2ecefa2f16c9f5485ad066bebf9a14`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:36:47 GMT
RUN apk add --no-cache ca-certificates
# Wed, 09 Aug 2023 04:41:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Aug 2023 04:41:57 GMT
ENV GOLANG_VERSION=1.20.7
# Wed, 09 Aug 2023 04:43:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 09 Aug 2023 04:43:29 GMT
ENV GOPATH=/go
# Wed, 09 Aug 2023 04:43:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Aug 2023 04:43:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 09 Aug 2023 04:43:30 GMT
WORKDIR /go
# Wed, 09 Aug 2023 10:26:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 09 Aug 2023 10:26:17 GMT
ENV XCADDY_VERSION=v0.3.4
# Wed, 09 Aug 2023 10:26:17 GMT
ENV CADDY_VERSION=v2.7.2
# Wed, 09 Aug 2023 10:26:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Aug 2023 10:26:17 GMT
ENV XCADDY_SETCAP=1
# Wed, 09 Aug 2023 10:26:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68ab15d90eb70c23e8b13c3935b194fc1b638f8c0fee6506a109dcee082c20d6e07890320a876b13eb23b5a7a0617daa28fe8af24dcb0dcb3eca9ea74dc76713' ;; 		armhf)   binArch='armv6'; checksum='2853413e63ac29f296b1c44696022febc8b29c4b37fb20442b635903a0b79d523ca00896dfce3e40f5894dd297b345ac007af0ddffccaada843c7de61d334134' ;; 		armv7)   binArch='armv7'; checksum='c59e93ba270705b2312f6a70552f2a345cec91cc3504233785cb46fa4b644a47e520bb29dfbf519f814bb13d0bbea213976fd7b059883eab2b091913f9ed393f' ;; 		aarch64) binArch='arm64'; checksum='df4c58e97931ca58b7a38d245948912b817e952a2961ff583744039ca68a584a303f7cbfdb33392c84d8f76f5b30f206d9f84a04f547043a3d1fa5282b0fd544' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2795d5b7546bd10ff3cd21a393597281e42e1043164536e01e18fb56047ba5b396493a086bb2d90e8ede9a54b5208e947ecaacccca4a8550704fb3f8a17dd771' ;; 		s390x)   binArch='s390x'; checksum='2ed85231aac36e3af873e3fdf4f6b6378b55dcc17743d24b28b3b48d6622fde73aae58eed124082478a0b841c338d64caa0b0be302545a79092a97cf205f1b29' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 09 Aug 2023 10:26:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 09 Aug 2023 10:26:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d48a809fc2256f8aa0aeee47998488d64409855adba00a7cb3007ab9f3286e`  
		Last Modified: Wed, 09 Aug 2023 03:37:02 GMT  
		Size: 284.7 KB (284693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e790db5857269a95a948a96f0e3304c851351e588262d58504700b2e73fb7fe`  
		Last Modified: Wed, 09 Aug 2023 04:47:32 GMT  
		Size: 101.0 MB (100954810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727f4e1a48a681e22437b6c14b04a4e287386f50f1be21ef490a1e28fd276a91`  
		Last Modified: Wed, 09 Aug 2023 04:47:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a272b880a0f8927853947bb9b16e005e2824b1685a89cc015f4e4694c441ed0e`  
		Last Modified: Wed, 09 Aug 2023 10:26:35 GMT  
		Size: 5.0 MB (4958652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e328d3f19ca0bf59908eb26cf5d7b5f94d2aa3e53eb5426f11ddaceca7d024`  
		Last Modified: Wed, 09 Aug 2023 10:26:35 GMT  
		Size: 1.3 MB (1301217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3115a3b8c7625246591f7ffa414a109f6c26f09066d0a9b9c0aba053e2a13c02`  
		Last Modified: Wed, 09 Aug 2023 10:26:35 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:289b1f78db36a7524bbae6562b80b29fe5585984effd44a3e22146fcbf4ab824
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108301221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98ac734398939dbe1f4c664f493d34b5353c438189c6b58b3e6e4d92186a8f80`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:12:05 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:12:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:12:40 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 23:14:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 23:14:36 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 23:14:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:14:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 23:14:37 GMT
WORKDIR /go
# Wed, 09 Aug 2023 03:38:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:49:20 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:49:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:49:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:49:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8564ce36feee688566265012773f1c8c7c046ceefe86ca763eb702682f4e6e75`  
		Last Modified: Tue, 08 Aug 2023 23:15:06 GMT  
		Size: 284.9 KB (284876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b139603b026cc15bf570c9cf012fc165cb74821883c7c7c534fe6ed189b5a2`  
		Last Modified: Tue, 08 Aug 2023 23:16:29 GMT  
		Size: 98.7 MB (98671161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b2f37c2778ffd2e158ad31438d6802c214dfa5d79e06dc9af2d8320828e148`  
		Last Modified: Tue, 08 Aug 2023 23:16:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f22c305527b162efa854ac3e1963e59e7fb8f2c71838222c56462b9809481ed`  
		Last Modified: Wed, 09 Aug 2023 03:39:10 GMT  
		Size: 5.0 MB (4951147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5520daf22ad222fbe3c81bbd6afa0c912b3817f0f432a35a939f9870a8512af`  
		Last Modified: Mon, 14 Aug 2023 17:49:51 GMT  
		Size: 1.2 MB (1248666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f8fe3942ebea0d37a8324080324eb0bca35e859273e7bac44381e31a0fa714`  
		Last Modified: Mon, 14 Aug 2023 17:49:51 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:dcbac62a4e9d8d10345a7f20ac37a814b45633ed4b050a14fa20aef08590597a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107386270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0adee903aaec70e29acbd506823b19cc477dc7788e545d1b88316b9ec0e9c154`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:39:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 01:39:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 01:40:29 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 01:42:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 01:42:12 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 01:42:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 01:42:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 01:42:13 GMT
WORKDIR /go
# Tue, 08 Aug 2023 01:51:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:57:24 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:57:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:57:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:57:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47bd95d78f565e902bafd0264a979eb4f6f71e22c0464011bf9db6feb0579e6`  
		Last Modified: Tue, 08 Aug 2023 01:48:34 GMT  
		Size: 284.1 KB (284073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a674106498848b269b5cb69fb938d3dc97247d02cb1aa3927b7a7469724e950`  
		Last Modified: Tue, 08 Aug 2023 01:49:43 GMT  
		Size: 98.5 MB (98454659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1902a68db0b07b05ab7d2f3e48ca8f1d22951b498f6ff9027bdc91a5e7e830`  
		Last Modified: Tue, 08 Aug 2023 01:49:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9caf1886c556e441f6f89cd1cb00e1b950d9d8fcad8812a988fbb59caf0b0ba5`  
		Last Modified: Tue, 08 Aug 2023 01:52:22 GMT  
		Size: 4.5 MB (4501403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c28b1afe92de619aa5de35a2f610dc68af6b39c6cd300ef8426738a739366a2`  
		Last Modified: Mon, 14 Aug 2023 17:58:00 GMT  
		Size: 1.2 MB (1246092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6fe75fd67d7668d6aeca167419514f45cb72ec61bd61a9fc32e25b5c928dba6`  
		Last Modified: Mon, 14 Aug 2023 17:58:00 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:9ad7390f7aa878bd4d6750dab9611c7397630fc15a7f80304eea3d3f64dcfe4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.0 MB (105987240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c79cdcd45a4a61e8fe257b7917335ede1523a72d1c2ef2eb9115783a5379f5ea`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:10:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:10:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:10:53 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 23:11:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 23:11:59 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 23:11:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:12:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 23:12:00 GMT
WORKDIR /go
# Wed, 09 Aug 2023 10:10:28 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:39:25 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:39:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:39:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:39:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54e960e981301b0098c80d2e61d694333b5ab480a007a3a8d0fa629662d377`  
		Last Modified: Tue, 08 Aug 2023 23:14:21 GMT  
		Size: 286.3 KB (286298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20ccffba14f84f51f896ae916a3dd045a0b0d08dc27d53f7d6a9dc5687c3501`  
		Last Modified: Tue, 08 Aug 2023 23:15:23 GMT  
		Size: 96.1 MB (96117263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d452dd4d3acc29d43b0be67bcc0c121814601787c7fd45e8260687d2cc8983`  
		Last Modified: Tue, 08 Aug 2023 23:15:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d371a704ab9a071c89db966e268fe56aad2288363a849d10eb032d47cd10848b`  
		Last Modified: Wed, 09 Aug 2023 10:10:48 GMT  
		Size: 5.1 MB (5053901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5e38cf28101c20845f7f103114793f73691285da6ac006db5cb28c20bc8000`  
		Last Modified: Mon, 14 Aug 2023 17:39:55 GMT  
		Size: 1.2 MB (1198449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d1b8334b836b303a87ddda4bfba4af764950afa40c2c263cca11ed8b53a8c6`  
		Last Modified: Mon, 14 Aug 2023 17:39:54 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:e3543706f8faff15a067252f4e5760bb4cb3e12ff81b7a932052bc013ecc4151
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106660406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37b7339021535bddbd7f4a89deae282741ae3163c68d69d7d5d035167f7d440`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:25:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 00:25:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 00:26:56 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 00:29:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 00:29:34 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 00:29:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 00:29:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 00:29:36 GMT
WORKDIR /go
# Tue, 08 Aug 2023 00:44:40 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 08 Aug 2023 00:44:41 GMT
ENV XCADDY_VERSION=v0.3.4
# Tue, 08 Aug 2023 00:44:42 GMT
ENV CADDY_VERSION=v2.7.2
# Tue, 08 Aug 2023 00:44:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 08 Aug 2023 00:44:43 GMT
ENV XCADDY_SETCAP=1
# Tue, 08 Aug 2023 00:44:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68ab15d90eb70c23e8b13c3935b194fc1b638f8c0fee6506a109dcee082c20d6e07890320a876b13eb23b5a7a0617daa28fe8af24dcb0dcb3eca9ea74dc76713' ;; 		armhf)   binArch='armv6'; checksum='2853413e63ac29f296b1c44696022febc8b29c4b37fb20442b635903a0b79d523ca00896dfce3e40f5894dd297b345ac007af0ddffccaada843c7de61d334134' ;; 		armv7)   binArch='armv7'; checksum='c59e93ba270705b2312f6a70552f2a345cec91cc3504233785cb46fa4b644a47e520bb29dfbf519f814bb13d0bbea213976fd7b059883eab2b091913f9ed393f' ;; 		aarch64) binArch='arm64'; checksum='df4c58e97931ca58b7a38d245948912b817e952a2961ff583744039ca68a584a303f7cbfdb33392c84d8f76f5b30f206d9f84a04f547043a3d1fa5282b0fd544' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2795d5b7546bd10ff3cd21a393597281e42e1043164536e01e18fb56047ba5b396493a086bb2d90e8ede9a54b5208e947ecaacccca4a8550704fb3f8a17dd771' ;; 		s390x)   binArch='s390x'; checksum='2ed85231aac36e3af873e3fdf4f6b6378b55dcc17743d24b28b3b48d6622fde73aae58eed124082478a0b841c338d64caa0b0be302545a79092a97cf205f1b29' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 08 Aug 2023 00:44:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 08 Aug 2023 00:44:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c966ad2cdd35689da92e7c8fd39bd37cd6080c484e6ccaf00672c154cd4f6c2a`  
		Last Modified: Tue, 08 Aug 2023 00:39:35 GMT  
		Size: 286.7 KB (286662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7816c9df7e6881fdd62dfcc6d743edcc2c3ca9220542437a2e5fdcfa0e4548`  
		Last Modified: Tue, 08 Aug 2023 00:41:09 GMT  
		Size: 96.6 MB (96591770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d34a514a03c5af8a03dfe8c4fbfd50b2ec61591d24080f8be8bf722904f541`  
		Last Modified: Tue, 08 Aug 2023 00:40:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802af1410e20c34900a811878ca2fa2e5dc79daeb92a53b94588831011ad81fc`  
		Last Modified: Tue, 08 Aug 2023 00:45:40 GMT  
		Size: 5.2 MB (5249966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5fe808e6f175a659981d31b9687526a651f4d40bce158c2baa204fcfcf2820`  
		Last Modified: Tue, 08 Aug 2023 00:45:39 GMT  
		Size: 1.2 MB (1185194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681275e7741131c55614b72469583c04861fb9344cde71f5dc2d00b75af4737b`  
		Last Modified: Tue, 08 Aug 2023 00:45:39 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:4c76dac9b235685647bce5e644408f9537fd2a98243936db0666252a4ec24739
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110727449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84fe6eea8994d5e82ec6e85ed4c441f0a89b9cb461829805dd3eeb9d892d49a9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:41 GMT
RUN apk add --no-cache ca-certificates
# Mon, 07 Aug 2023 20:19:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Aug 2023 20:21:06 GMT
ENV GOLANG_VERSION=1.20.7
# Mon, 07 Aug 2023 20:23:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 07 Aug 2023 20:23:05 GMT
ENV GOPATH=/go
# Mon, 07 Aug 2023 20:23:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Aug 2023 20:23:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 07 Aug 2023 20:23:06 GMT
WORKDIR /go
# Tue, 08 Aug 2023 05:25:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:41:51 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:41:52 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:41:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:41:52 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:41:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:41:54 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:41:54 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec90be18226e5c99d10161aed1a143f4134093c55b4d6979bbdbbe4b0683eb11`  
		Last Modified: Mon, 07 Aug 2023 20:30:59 GMT  
		Size: 285.1 KB (285089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c751f85e4ba6e9bbada0b11691d914b2ec2c689bb0dca6b9cbe994488d0e3e`  
		Last Modified: Mon, 07 Aug 2023 20:31:56 GMT  
		Size: 100.9 MB (100865267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2d202223222826c8580d85b8d7dd6baa8ed1cad84ba5cf47dab23eaeeae7e9`  
		Last Modified: Mon, 07 Aug 2023 20:31:43 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0359ada615d16e203e1d40a49b896060013c2952c2982ae73b141cc291305a4c`  
		Last Modified: Tue, 08 Aug 2023 05:25:47 GMT  
		Size: 5.1 MB (5099943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1039996d136f688a91d291dcf3dbb995607af1f245f1741d8ad0c5f73cec1b01`  
		Last Modified: Mon, 14 Aug 2023 17:42:27 GMT  
		Size: 1.3 MB (1262391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17e7bfc7e0d6b6a7f70b22841fe42427f0fb6372b17c71c8063c50d7c8e73c1`  
		Last Modified: Mon, 14 Aug 2023 17:42:27 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:a6ebd264677820f38a44fb346c24e5b3cc1406cf5f975a99a089e14f2cfeb623
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2132345169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec0a81535ff140c0b08b259f2eb43a2face74a8aaeed3cc1ac39ef9b4e90c3f6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:39:54 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:39:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:41:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:41:12 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:42:07 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:53:35 GMT
ENV GOLANG_VERSION=1.20.7
# Thu, 10 Aug 2023 00:56:38 GMT
RUN $url = 'https://dl.google.com/go/go1.20.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '736dc6c7fcab1c96b682c8c93e38d7e371e62a17d34cb2c37d451a1147f66af9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:56:40 GMT
WORKDIR C:\go
# Thu, 10 Aug 2023 03:04:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 03:04:56 GMT
ENV XCADDY_VERSION=v0.3.4
# Thu, 10 Aug 2023 03:04:57 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:04:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Aug 2023 03:06:01 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('542b4c083852d41081186c79757b66ff3c26248f72ed461dbc038b51687d0a8a8ce8eee69e3b5a1d43360c48b3405b611b940fa378debe98aaa0b3c5aebfa218')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 10 Aug 2023 03:06:02 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594083c5c2094c95b4e52723d54c14e0d70881f4f176720c3170012275accc3b`  
		Last Modified: Thu, 10 Aug 2023 01:02:54 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e2c2a5b75ced3a3a50be088c4a6c2d7df926b1fe6515b2d0c021312e3642f4`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d28688050deeec928289543beadf5c75bb2a8246576cb7c066e23818016217`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e5fbc50e7e0fefb7c9e349038ecb00ed5c000bcab8c4d82b1e1000c4273c01`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0544e07bd9df923e11e09c7dc042da614f2f14589eb6fa79005ebbbf2731e97d`  
		Last Modified: Thu, 10 Aug 2023 01:02:57 GMT  
		Size: 25.6 MB (25560980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555a82506c4fcec2bd90ae77756e5b03788e30c89f1a3820aa0b6a7ae6ad58ae`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bcfb422b104764156fc5ba099b5e3ae9fa9f760fd2db1c21acd8969b3d73de`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 220.8 KB (220796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c6aa0a5a1689ed800c4ef72c1b9febf207840fd2c6abfe4bb460e2e2bfb0b0`  
		Last Modified: Thu, 10 Aug 2023 01:05:03 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53d3379322a67b2413189cc2b779d22cb4093124343c8bb17fdf720b7b49fda`  
		Last Modified: Thu, 10 Aug 2023 01:05:25 GMT  
		Size: 108.9 MB (108911716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b60ccf92610ddbc47a05664785c95215a123e8930afbf6e3e2cefc80e693fd2`  
		Last Modified: Thu, 10 Aug 2023 01:05:04 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2c7d6253e62d61e5e0d2ad331a96cff5175f6c608b2ab4657825b3e3b4b4d0`  
		Last Modified: Thu, 10 Aug 2023 03:08:03 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c54227291fad3a25beb98d755de6f26fee6576e1b807e42c0bb70aa45793b3`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d107b434fabbe0d8d3916744b92501e6f5f8dabf7621ce44432d53d3853b4b8`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b0bcd286241a360f34f20c3842b90b6f53c31abe4d60fcb8f1148e8ba191a3`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5677a754ea49eeeb0b5ed56da2ac0d43c11e3c935c36adc2cc71b95dc7b99c0f`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.7 MB (1679125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4626f9b6f575add3a8f4ac9248f4342e9cb80f9abf696deff5a7bd9aff57fbf1`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:44aba8da329d3ea3489327b5c94e41477f815f943659f4464a2c859ad400dcfd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1933815424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d095c2914283b4b75e4dbb95eb3e7f5ff6db80079dc6981bf1c5fa8355036c99`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:36:23 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:36:24 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:36:25 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:36:26 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:36:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:37:00 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:37:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:50:52 GMT
ENV GOLANG_VERSION=1.20.7
# Thu, 10 Aug 2023 00:53:17 GMT
RUN $url = 'https://dl.google.com/go/go1.20.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '736dc6c7fcab1c96b682c8c93e38d7e371e62a17d34cb2c37d451a1147f66af9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:53:18 GMT
WORKDIR C:\go
# Thu, 10 Aug 2023 03:06:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 03:06:10 GMT
ENV XCADDY_VERSION=v0.3.4
# Thu, 10 Aug 2023 03:06:11 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:06:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Aug 2023 03:06:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('542b4c083852d41081186c79757b66ff3c26248f72ed461dbc038b51687d0a8a8ce8eee69e3b5a1d43360c48b3405b611b940fa378debe98aaa0b3c5aebfa218')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 10 Aug 2023 03:06:35 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877256a6389e5e2563da79ad5bd201e7ee136abf14ff7cb0d4efbf3b24e5f127`  
		Last Modified: Thu, 10 Aug 2023 01:02:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a39df29b3c0b2f7e691c47273110db4a46e5c8e299f6bb95f77a9c61f79872`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8574d63bce1547e3177d0b76237a782a9b016d4880375dcd1a7b6a1c5dee3dc`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ef34b3c96316bcdd92e24c8c4eebdc3a35f245c013ef87edfae0dde091a305`  
		Last Modified: Thu, 10 Aug 2023 01:02:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a481babc5b629f694446a96dba8d77c020257c98334c605aff94162b9a917279`  
		Last Modified: Thu, 10 Aug 2023 01:02:23 GMT  
		Size: 25.6 MB (25554169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281178ea1c103ff07ea7e4fb647eb0dbe4f865742da6ef9944e04f37974fc27c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b5d34adf2aacfe87580143f3e17c635dc8dbd4068377b79b35d665f49bbad9`  
		Last Modified: Thu, 10 Aug 2023 01:02:16 GMT  
		Size: 275.9 KB (275946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02a2e79b5a05c2145c733eefb2add45d1ebefb7a16b93c321f5883c8ced6f1a`  
		Last Modified: Thu, 10 Aug 2023 01:04:30 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd9991b8cfbc481c153abf1625143209f4c4fd40d9443a5a19f4e3613336ad2`  
		Last Modified: Thu, 10 Aug 2023 01:04:53 GMT  
		Size: 108.9 MB (108927695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dc6778f41c3c7d50b8e71668e22880153d6c6794f24c4661fc3d6aa089d0a5`  
		Last Modified: Thu, 10 Aug 2023 01:04:30 GMT  
		Size: 1.5 KB (1547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c5985f015e143065716f5aabf0ecaed537103c5ec07e6c57360204a7787d02`  
		Last Modified: Thu, 10 Aug 2023 03:08:23 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd9cf527e30318df5bccd0be2c9a9716dc073b1f84c1d2c5cadc85adcf2af02`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604bc0fdaac29b943186656363f9267b86b2744da35d6b519a428d494d0a6bd3`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b527a45b48b4328e0ea94e3e2d3f239ed4f960d30ea0b9272cd902aec85c8b`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9ae10f93498ae3f8bbfef69dd561e41337584fb8dcc09fe82ed4971f9787be`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.7 MB (1675642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6218363385083ee3dbece9e5e2fd5c9086be201ca76bd6818b46bb6e591688eb`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:f921c48f48fcc6d6b234fd185f35b3762f339365402630553bfcca85a8376dbb
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
$ docker pull caddy@sha256:7abb7723020bab7b367d33786efcfca5d4a4f884ec306308d4a5513f14cdc20c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110901544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e24e6bda832eff522a3ea76a20f3e8055f2ecefa2f16c9f5485ad066bebf9a14`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:36:47 GMT
RUN apk add --no-cache ca-certificates
# Wed, 09 Aug 2023 04:41:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Aug 2023 04:41:57 GMT
ENV GOLANG_VERSION=1.20.7
# Wed, 09 Aug 2023 04:43:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 09 Aug 2023 04:43:29 GMT
ENV GOPATH=/go
# Wed, 09 Aug 2023 04:43:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Aug 2023 04:43:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 09 Aug 2023 04:43:30 GMT
WORKDIR /go
# Wed, 09 Aug 2023 10:26:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 09 Aug 2023 10:26:17 GMT
ENV XCADDY_VERSION=v0.3.4
# Wed, 09 Aug 2023 10:26:17 GMT
ENV CADDY_VERSION=v2.7.2
# Wed, 09 Aug 2023 10:26:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Aug 2023 10:26:17 GMT
ENV XCADDY_SETCAP=1
# Wed, 09 Aug 2023 10:26:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68ab15d90eb70c23e8b13c3935b194fc1b638f8c0fee6506a109dcee082c20d6e07890320a876b13eb23b5a7a0617daa28fe8af24dcb0dcb3eca9ea74dc76713' ;; 		armhf)   binArch='armv6'; checksum='2853413e63ac29f296b1c44696022febc8b29c4b37fb20442b635903a0b79d523ca00896dfce3e40f5894dd297b345ac007af0ddffccaada843c7de61d334134' ;; 		armv7)   binArch='armv7'; checksum='c59e93ba270705b2312f6a70552f2a345cec91cc3504233785cb46fa4b644a47e520bb29dfbf519f814bb13d0bbea213976fd7b059883eab2b091913f9ed393f' ;; 		aarch64) binArch='arm64'; checksum='df4c58e97931ca58b7a38d245948912b817e952a2961ff583744039ca68a584a303f7cbfdb33392c84d8f76f5b30f206d9f84a04f547043a3d1fa5282b0fd544' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2795d5b7546bd10ff3cd21a393597281e42e1043164536e01e18fb56047ba5b396493a086bb2d90e8ede9a54b5208e947ecaacccca4a8550704fb3f8a17dd771' ;; 		s390x)   binArch='s390x'; checksum='2ed85231aac36e3af873e3fdf4f6b6378b55dcc17743d24b28b3b48d6622fde73aae58eed124082478a0b841c338d64caa0b0be302545a79092a97cf205f1b29' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 09 Aug 2023 10:26:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 09 Aug 2023 10:26:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d48a809fc2256f8aa0aeee47998488d64409855adba00a7cb3007ab9f3286e`  
		Last Modified: Wed, 09 Aug 2023 03:37:02 GMT  
		Size: 284.7 KB (284693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e790db5857269a95a948a96f0e3304c851351e588262d58504700b2e73fb7fe`  
		Last Modified: Wed, 09 Aug 2023 04:47:32 GMT  
		Size: 101.0 MB (100954810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727f4e1a48a681e22437b6c14b04a4e287386f50f1be21ef490a1e28fd276a91`  
		Last Modified: Wed, 09 Aug 2023 04:47:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a272b880a0f8927853947bb9b16e005e2824b1685a89cc015f4e4694c441ed0e`  
		Last Modified: Wed, 09 Aug 2023 10:26:35 GMT  
		Size: 5.0 MB (4958652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e328d3f19ca0bf59908eb26cf5d7b5f94d2aa3e53eb5426f11ddaceca7d024`  
		Last Modified: Wed, 09 Aug 2023 10:26:35 GMT  
		Size: 1.3 MB (1301217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3115a3b8c7625246591f7ffa414a109f6c26f09066d0a9b9c0aba053e2a13c02`  
		Last Modified: Wed, 09 Aug 2023 10:26:35 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:289b1f78db36a7524bbae6562b80b29fe5585984effd44a3e22146fcbf4ab824
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108301221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98ac734398939dbe1f4c664f493d34b5353c438189c6b58b3e6e4d92186a8f80`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:12:05 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:12:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:12:40 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 23:14:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 23:14:36 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 23:14:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:14:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 23:14:37 GMT
WORKDIR /go
# Wed, 09 Aug 2023 03:38:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:49:20 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:49:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:49:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:49:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8564ce36feee688566265012773f1c8c7c046ceefe86ca763eb702682f4e6e75`  
		Last Modified: Tue, 08 Aug 2023 23:15:06 GMT  
		Size: 284.9 KB (284876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b139603b026cc15bf570c9cf012fc165cb74821883c7c7c534fe6ed189b5a2`  
		Last Modified: Tue, 08 Aug 2023 23:16:29 GMT  
		Size: 98.7 MB (98671161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b2f37c2778ffd2e158ad31438d6802c214dfa5d79e06dc9af2d8320828e148`  
		Last Modified: Tue, 08 Aug 2023 23:16:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f22c305527b162efa854ac3e1963e59e7fb8f2c71838222c56462b9809481ed`  
		Last Modified: Wed, 09 Aug 2023 03:39:10 GMT  
		Size: 5.0 MB (4951147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5520daf22ad222fbe3c81bbd6afa0c912b3817f0f432a35a939f9870a8512af`  
		Last Modified: Mon, 14 Aug 2023 17:49:51 GMT  
		Size: 1.2 MB (1248666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f8fe3942ebea0d37a8324080324eb0bca35e859273e7bac44381e31a0fa714`  
		Last Modified: Mon, 14 Aug 2023 17:49:51 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:dcbac62a4e9d8d10345a7f20ac37a814b45633ed4b050a14fa20aef08590597a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107386270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0adee903aaec70e29acbd506823b19cc477dc7788e545d1b88316b9ec0e9c154`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:39:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 01:39:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 01:40:29 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 01:42:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 01:42:12 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 01:42:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 01:42:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 01:42:13 GMT
WORKDIR /go
# Tue, 08 Aug 2023 01:51:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:57:24 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:57:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:57:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:57:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47bd95d78f565e902bafd0264a979eb4f6f71e22c0464011bf9db6feb0579e6`  
		Last Modified: Tue, 08 Aug 2023 01:48:34 GMT  
		Size: 284.1 KB (284073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a674106498848b269b5cb69fb938d3dc97247d02cb1aa3927b7a7469724e950`  
		Last Modified: Tue, 08 Aug 2023 01:49:43 GMT  
		Size: 98.5 MB (98454659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1902a68db0b07b05ab7d2f3e48ca8f1d22951b498f6ff9027bdc91a5e7e830`  
		Last Modified: Tue, 08 Aug 2023 01:49:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9caf1886c556e441f6f89cd1cb00e1b950d9d8fcad8812a988fbb59caf0b0ba5`  
		Last Modified: Tue, 08 Aug 2023 01:52:22 GMT  
		Size: 4.5 MB (4501403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c28b1afe92de619aa5de35a2f610dc68af6b39c6cd300ef8426738a739366a2`  
		Last Modified: Mon, 14 Aug 2023 17:58:00 GMT  
		Size: 1.2 MB (1246092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6fe75fd67d7668d6aeca167419514f45cb72ec61bd61a9fc32e25b5c928dba6`  
		Last Modified: Mon, 14 Aug 2023 17:58:00 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:9ad7390f7aa878bd4d6750dab9611c7397630fc15a7f80304eea3d3f64dcfe4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.0 MB (105987240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c79cdcd45a4a61e8fe257b7917335ede1523a72d1c2ef2eb9115783a5379f5ea`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:10:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:10:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:10:53 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 23:11:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 23:11:59 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 23:11:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:12:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 23:12:00 GMT
WORKDIR /go
# Wed, 09 Aug 2023 10:10:28 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:39:25 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:39:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:39:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:39:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54e960e981301b0098c80d2e61d694333b5ab480a007a3a8d0fa629662d377`  
		Last Modified: Tue, 08 Aug 2023 23:14:21 GMT  
		Size: 286.3 KB (286298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20ccffba14f84f51f896ae916a3dd045a0b0d08dc27d53f7d6a9dc5687c3501`  
		Last Modified: Tue, 08 Aug 2023 23:15:23 GMT  
		Size: 96.1 MB (96117263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d452dd4d3acc29d43b0be67bcc0c121814601787c7fd45e8260687d2cc8983`  
		Last Modified: Tue, 08 Aug 2023 23:15:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d371a704ab9a071c89db966e268fe56aad2288363a849d10eb032d47cd10848b`  
		Last Modified: Wed, 09 Aug 2023 10:10:48 GMT  
		Size: 5.1 MB (5053901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5e38cf28101c20845f7f103114793f73691285da6ac006db5cb28c20bc8000`  
		Last Modified: Mon, 14 Aug 2023 17:39:55 GMT  
		Size: 1.2 MB (1198449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d1b8334b836b303a87ddda4bfba4af764950afa40c2c263cca11ed8b53a8c6`  
		Last Modified: Mon, 14 Aug 2023 17:39:54 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:e3543706f8faff15a067252f4e5760bb4cb3e12ff81b7a932052bc013ecc4151
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106660406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37b7339021535bddbd7f4a89deae282741ae3163c68d69d7d5d035167f7d440`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:25:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 00:25:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 00:26:56 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 00:29:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 00:29:34 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 00:29:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 00:29:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 00:29:36 GMT
WORKDIR /go
# Tue, 08 Aug 2023 00:44:40 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 08 Aug 2023 00:44:41 GMT
ENV XCADDY_VERSION=v0.3.4
# Tue, 08 Aug 2023 00:44:42 GMT
ENV CADDY_VERSION=v2.7.2
# Tue, 08 Aug 2023 00:44:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 08 Aug 2023 00:44:43 GMT
ENV XCADDY_SETCAP=1
# Tue, 08 Aug 2023 00:44:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68ab15d90eb70c23e8b13c3935b194fc1b638f8c0fee6506a109dcee082c20d6e07890320a876b13eb23b5a7a0617daa28fe8af24dcb0dcb3eca9ea74dc76713' ;; 		armhf)   binArch='armv6'; checksum='2853413e63ac29f296b1c44696022febc8b29c4b37fb20442b635903a0b79d523ca00896dfce3e40f5894dd297b345ac007af0ddffccaada843c7de61d334134' ;; 		armv7)   binArch='armv7'; checksum='c59e93ba270705b2312f6a70552f2a345cec91cc3504233785cb46fa4b644a47e520bb29dfbf519f814bb13d0bbea213976fd7b059883eab2b091913f9ed393f' ;; 		aarch64) binArch='arm64'; checksum='df4c58e97931ca58b7a38d245948912b817e952a2961ff583744039ca68a584a303f7cbfdb33392c84d8f76f5b30f206d9f84a04f547043a3d1fa5282b0fd544' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2795d5b7546bd10ff3cd21a393597281e42e1043164536e01e18fb56047ba5b396493a086bb2d90e8ede9a54b5208e947ecaacccca4a8550704fb3f8a17dd771' ;; 		s390x)   binArch='s390x'; checksum='2ed85231aac36e3af873e3fdf4f6b6378b55dcc17743d24b28b3b48d6622fde73aae58eed124082478a0b841c338d64caa0b0be302545a79092a97cf205f1b29' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 08 Aug 2023 00:44:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 08 Aug 2023 00:44:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c966ad2cdd35689da92e7c8fd39bd37cd6080c484e6ccaf00672c154cd4f6c2a`  
		Last Modified: Tue, 08 Aug 2023 00:39:35 GMT  
		Size: 286.7 KB (286662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7816c9df7e6881fdd62dfcc6d743edcc2c3ca9220542437a2e5fdcfa0e4548`  
		Last Modified: Tue, 08 Aug 2023 00:41:09 GMT  
		Size: 96.6 MB (96591770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d34a514a03c5af8a03dfe8c4fbfd50b2ec61591d24080f8be8bf722904f541`  
		Last Modified: Tue, 08 Aug 2023 00:40:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802af1410e20c34900a811878ca2fa2e5dc79daeb92a53b94588831011ad81fc`  
		Last Modified: Tue, 08 Aug 2023 00:45:40 GMT  
		Size: 5.2 MB (5249966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5fe808e6f175a659981d31b9687526a651f4d40bce158c2baa204fcfcf2820`  
		Last Modified: Tue, 08 Aug 2023 00:45:39 GMT  
		Size: 1.2 MB (1185194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681275e7741131c55614b72469583c04861fb9344cde71f5dc2d00b75af4737b`  
		Last Modified: Tue, 08 Aug 2023 00:45:39 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:4c76dac9b235685647bce5e644408f9537fd2a98243936db0666252a4ec24739
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110727449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84fe6eea8994d5e82ec6e85ed4c441f0a89b9cb461829805dd3eeb9d892d49a9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:41 GMT
RUN apk add --no-cache ca-certificates
# Mon, 07 Aug 2023 20:19:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Aug 2023 20:21:06 GMT
ENV GOLANG_VERSION=1.20.7
# Mon, 07 Aug 2023 20:23:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 07 Aug 2023 20:23:05 GMT
ENV GOPATH=/go
# Mon, 07 Aug 2023 20:23:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Aug 2023 20:23:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 07 Aug 2023 20:23:06 GMT
WORKDIR /go
# Tue, 08 Aug 2023 05:25:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:41:51 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:41:52 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:41:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:41:52 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:41:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:41:54 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:41:54 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec90be18226e5c99d10161aed1a143f4134093c55b4d6979bbdbbe4b0683eb11`  
		Last Modified: Mon, 07 Aug 2023 20:30:59 GMT  
		Size: 285.1 KB (285089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c751f85e4ba6e9bbada0b11691d914b2ec2c689bb0dca6b9cbe994488d0e3e`  
		Last Modified: Mon, 07 Aug 2023 20:31:56 GMT  
		Size: 100.9 MB (100865267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2d202223222826c8580d85b8d7dd6baa8ed1cad84ba5cf47dab23eaeeae7e9`  
		Last Modified: Mon, 07 Aug 2023 20:31:43 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0359ada615d16e203e1d40a49b896060013c2952c2982ae73b141cc291305a4c`  
		Last Modified: Tue, 08 Aug 2023 05:25:47 GMT  
		Size: 5.1 MB (5099943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1039996d136f688a91d291dcf3dbb995607af1f245f1741d8ad0c5f73cec1b01`  
		Last Modified: Mon, 14 Aug 2023 17:42:27 GMT  
		Size: 1.3 MB (1262391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17e7bfc7e0d6b6a7f70b22841fe42427f0fb6372b17c71c8063c50d7c8e73c1`  
		Last Modified: Mon, 14 Aug 2023 17:42:27 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:e47c546e0564931b55495f764fdfb59d8d81d4e51ff9a221952688b1dcf6d462
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:a6ebd264677820f38a44fb346c24e5b3cc1406cf5f975a99a089e14f2cfeb623
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2132345169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec0a81535ff140c0b08b259f2eb43a2face74a8aaeed3cc1ac39ef9b4e90c3f6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:39:54 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:39:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:41:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:41:12 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:42:07 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:53:35 GMT
ENV GOLANG_VERSION=1.20.7
# Thu, 10 Aug 2023 00:56:38 GMT
RUN $url = 'https://dl.google.com/go/go1.20.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '736dc6c7fcab1c96b682c8c93e38d7e371e62a17d34cb2c37d451a1147f66af9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:56:40 GMT
WORKDIR C:\go
# Thu, 10 Aug 2023 03:04:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 03:04:56 GMT
ENV XCADDY_VERSION=v0.3.4
# Thu, 10 Aug 2023 03:04:57 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:04:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Aug 2023 03:06:01 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('542b4c083852d41081186c79757b66ff3c26248f72ed461dbc038b51687d0a8a8ce8eee69e3b5a1d43360c48b3405b611b940fa378debe98aaa0b3c5aebfa218')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 10 Aug 2023 03:06:02 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594083c5c2094c95b4e52723d54c14e0d70881f4f176720c3170012275accc3b`  
		Last Modified: Thu, 10 Aug 2023 01:02:54 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e2c2a5b75ced3a3a50be088c4a6c2d7df926b1fe6515b2d0c021312e3642f4`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d28688050deeec928289543beadf5c75bb2a8246576cb7c066e23818016217`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e5fbc50e7e0fefb7c9e349038ecb00ed5c000bcab8c4d82b1e1000c4273c01`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0544e07bd9df923e11e09c7dc042da614f2f14589eb6fa79005ebbbf2731e97d`  
		Last Modified: Thu, 10 Aug 2023 01:02:57 GMT  
		Size: 25.6 MB (25560980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555a82506c4fcec2bd90ae77756e5b03788e30c89f1a3820aa0b6a7ae6ad58ae`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bcfb422b104764156fc5ba099b5e3ae9fa9f760fd2db1c21acd8969b3d73de`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 220.8 KB (220796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c6aa0a5a1689ed800c4ef72c1b9febf207840fd2c6abfe4bb460e2e2bfb0b0`  
		Last Modified: Thu, 10 Aug 2023 01:05:03 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53d3379322a67b2413189cc2b779d22cb4093124343c8bb17fdf720b7b49fda`  
		Last Modified: Thu, 10 Aug 2023 01:05:25 GMT  
		Size: 108.9 MB (108911716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b60ccf92610ddbc47a05664785c95215a123e8930afbf6e3e2cefc80e693fd2`  
		Last Modified: Thu, 10 Aug 2023 01:05:04 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2c7d6253e62d61e5e0d2ad331a96cff5175f6c608b2ab4657825b3e3b4b4d0`  
		Last Modified: Thu, 10 Aug 2023 03:08:03 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c54227291fad3a25beb98d755de6f26fee6576e1b807e42c0bb70aa45793b3`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d107b434fabbe0d8d3916744b92501e6f5f8dabf7621ce44432d53d3853b4b8`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b0bcd286241a360f34f20c3842b90b6f53c31abe4d60fcb8f1148e8ba191a3`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5677a754ea49eeeb0b5ed56da2ac0d43c11e3c935c36adc2cc71b95dc7b99c0f`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.7 MB (1679125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4626f9b6f575add3a8f4ac9248f4342e9cb80f9abf696deff5a7bd9aff57fbf1`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:b21f945f75a0af5f372c03cead52a84f725ba635c6f414ff9bcdfd81c64008c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1906; amd64

### `caddy:2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:44aba8da329d3ea3489327b5c94e41477f815f943659f4464a2c859ad400dcfd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1933815424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d095c2914283b4b75e4dbb95eb3e7f5ff6db80079dc6981bf1c5fa8355036c99`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:36:23 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:36:24 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:36:25 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:36:26 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:36:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:37:00 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:37:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:50:52 GMT
ENV GOLANG_VERSION=1.20.7
# Thu, 10 Aug 2023 00:53:17 GMT
RUN $url = 'https://dl.google.com/go/go1.20.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '736dc6c7fcab1c96b682c8c93e38d7e371e62a17d34cb2c37d451a1147f66af9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:53:18 GMT
WORKDIR C:\go
# Thu, 10 Aug 2023 03:06:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 03:06:10 GMT
ENV XCADDY_VERSION=v0.3.4
# Thu, 10 Aug 2023 03:06:11 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:06:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Aug 2023 03:06:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('542b4c083852d41081186c79757b66ff3c26248f72ed461dbc038b51687d0a8a8ce8eee69e3b5a1d43360c48b3405b611b940fa378debe98aaa0b3c5aebfa218')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 10 Aug 2023 03:06:35 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877256a6389e5e2563da79ad5bd201e7ee136abf14ff7cb0d4efbf3b24e5f127`  
		Last Modified: Thu, 10 Aug 2023 01:02:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a39df29b3c0b2f7e691c47273110db4a46e5c8e299f6bb95f77a9c61f79872`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8574d63bce1547e3177d0b76237a782a9b016d4880375dcd1a7b6a1c5dee3dc`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ef34b3c96316bcdd92e24c8c4eebdc3a35f245c013ef87edfae0dde091a305`  
		Last Modified: Thu, 10 Aug 2023 01:02:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a481babc5b629f694446a96dba8d77c020257c98334c605aff94162b9a917279`  
		Last Modified: Thu, 10 Aug 2023 01:02:23 GMT  
		Size: 25.6 MB (25554169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281178ea1c103ff07ea7e4fb647eb0dbe4f865742da6ef9944e04f37974fc27c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b5d34adf2aacfe87580143f3e17c635dc8dbd4068377b79b35d665f49bbad9`  
		Last Modified: Thu, 10 Aug 2023 01:02:16 GMT  
		Size: 275.9 KB (275946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02a2e79b5a05c2145c733eefb2add45d1ebefb7a16b93c321f5883c8ced6f1a`  
		Last Modified: Thu, 10 Aug 2023 01:04:30 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd9991b8cfbc481c153abf1625143209f4c4fd40d9443a5a19f4e3613336ad2`  
		Last Modified: Thu, 10 Aug 2023 01:04:53 GMT  
		Size: 108.9 MB (108927695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dc6778f41c3c7d50b8e71668e22880153d6c6794f24c4661fc3d6aa089d0a5`  
		Last Modified: Thu, 10 Aug 2023 01:04:30 GMT  
		Size: 1.5 KB (1547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c5985f015e143065716f5aabf0ecaed537103c5ec07e6c57360204a7787d02`  
		Last Modified: Thu, 10 Aug 2023 03:08:23 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd9cf527e30318df5bccd0be2c9a9716dc073b1f84c1d2c5cadc85adcf2af02`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604bc0fdaac29b943186656363f9267b86b2744da35d6b519a428d494d0a6bd3`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b527a45b48b4328e0ea94e3e2d3f239ed4f960d30ea0b9272cd902aec85c8b`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9ae10f93498ae3f8bbfef69dd561e41337584fb8dcc09fe82ed4971f9787be`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.7 MB (1675642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6218363385083ee3dbece9e5e2fd5c9086be201ca76bd6818b46bb6e591688eb`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:ee77e6dfe66fce930f6e92b862071843a872dfc67ee4b8ad9c0e843a0c4103fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4737; amd64
	-	windows version 10.0.20348.1906; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:1b4a86d284b971594d7e30ef09451be59ba84514b612c87b6406e2dfb8e9e23f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2011958834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ae5f48eae2f949ec09ad9f70ff2c2626318e07111bea5b6622116482ac991b0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 02:59:41 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Aug 2023 02:59:41 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:00:57 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('69d2d73c2514ab5ce4f6a60489c79ce4da0e1d4302c85ab584d0a7a7fd0d034bfe5a5caab78c96ac3383ddd7d2e12c3c41fb47c4716909d2a78d448b0289ccec')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Aug 2023 03:00:58 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Aug 2023 03:00:59 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Aug 2023 03:01:00 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Thu, 10 Aug 2023 03:01:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Aug 2023 03:01:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Aug 2023 03:01:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Aug 2023 03:01:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Aug 2023 03:01:03 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Aug 2023 03:01:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Aug 2023 03:01:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Aug 2023 03:01:06 GMT
EXPOSE 80
# Thu, 10 Aug 2023 03:01:06 GMT
EXPOSE 443
# Thu, 10 Aug 2023 03:01:07 GMT
EXPOSE 443/udp
# Thu, 10 Aug 2023 03:01:08 GMT
EXPOSE 2019
# Thu, 10 Aug 2023 03:03:10 GMT
RUN caddy version
# Thu, 10 Aug 2023 03:03:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907ddb8e2b3b8f440ec855971bf77d521900d3faecd1816d7146d89f1c78f408`  
		Last Modified: Thu, 10 Aug 2023 03:07:15 GMT  
		Size: 469.4 KB (469388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d430330f12b22fcc17a5d114d51ba3bb8e62a55f87b67f939d18651c226f927`  
		Last Modified: Thu, 10 Aug 2023 03:07:15 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd493f43c2fb25a7c8540ea353a098f784a6e8d5fe4e9d070e4a1de796cde96c`  
		Last Modified: Thu, 10 Aug 2023 03:07:18 GMT  
		Size: 15.2 MB (15241515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95b32f0fb8252db266318cca24c13f5eea8b8b3c19405b92f1a8b9199e39c5d`  
		Last Modified: Thu, 10 Aug 2023 03:07:14 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7dbc1767506f0f3f5b4d3a9671f97a723014ae1e38cf8056f6257db7917a88`  
		Last Modified: Thu, 10 Aug 2023 03:07:13 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7905b1f85b201367c5a62618ddc55da9a60cbb3da1da40ab60a88c125a5956`  
		Last Modified: Thu, 10 Aug 2023 03:07:13 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce34081b153cf49ce89b2ff4fc81f54a648cefc5d2dbb0f60048b94ba10f43b`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9622cc1048f5f7259d3263b67dd386c5d70ae4cf0a358c33deb3df8cdb316efd`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b1ca0970bf360a0627a1deae2985b658f54b41758f12f4e5448ed1aee3bc82`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503770a8fe554599aa8e6413082b7cb24d7f1faa328deaf28b34ddb2a294972b`  
		Last Modified: Thu, 10 Aug 2023 03:07:11 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea5eee99969c433a1c2f4d0f7fdc838185350144b9d3f20888c2a53cc6f3563`  
		Last Modified: Thu, 10 Aug 2023 03:07:11 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675093fb34c31fff953a92ee1831f09679783e7d3e1d9ff40a962f346d1dc581`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fd64685610dd5572f21efe3fae8cb13537c9deb6693caf4097bf9ec3b4dabe`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540e52aaf0b1acca0c4a9fbb2a60e5ce4bca2c119fbb3bbd86658186b23e3202`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29819bc504b56dacdb0df898ee58e26d8097802c0a5578cd14d4e3ed0655bde7`  
		Last Modified: Thu, 10 Aug 2023 03:07:09 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2157a412d53cd6d3174744de6c1cf5cb0dd03274fe9b36f749525867e4b9bd2`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cfbf0b65ccf78eb536c8a23f0b92fa148268c1fa4a39c1b19c7d9310e53b8d`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7faedca764204aa914e83a3721476c9a6a7f8177d057021e5a1debb81a436808`  
		Last Modified: Thu, 10 Aug 2023 03:07:09 GMT  
		Size: 268.6 KB (268640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86622825a44d72176deccdf0a5e4c9127ebf8f2591211cbdae585e9977363e8`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:144bc31c96841830b174ed1ff2da09ba18881208aae2efd16b3c850953f762f6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1813356270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02028c6ef8441cbf5181f34f78b4740b60dffff030772882302c9ca39f9a6096`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 03:03:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Aug 2023 03:03:52 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:04:21 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('69d2d73c2514ab5ce4f6a60489c79ce4da0e1d4302c85ab584d0a7a7fd0d034bfe5a5caab78c96ac3383ddd7d2e12c3c41fb47c4716909d2a78d448b0289ccec')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Aug 2023 03:04:21 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Aug 2023 03:04:22 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Aug 2023 03:04:23 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Thu, 10 Aug 2023 03:04:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Aug 2023 03:04:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Aug 2023 03:04:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Aug 2023 03:04:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Aug 2023 03:04:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Aug 2023 03:04:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Aug 2023 03:04:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Aug 2023 03:04:29 GMT
EXPOSE 80
# Thu, 10 Aug 2023 03:04:30 GMT
EXPOSE 443
# Thu, 10 Aug 2023 03:04:31 GMT
EXPOSE 443/udp
# Thu, 10 Aug 2023 03:04:32 GMT
EXPOSE 2019
# Thu, 10 Aug 2023 03:04:47 GMT
RUN caddy version
# Thu, 10 Aug 2023 03:04:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee168d3c6067847c3aef71a2a0dfdc70984b0bb6164086b49da7bd27de3ff3e4`  
		Last Modified: Thu, 10 Aug 2023 03:07:41 GMT  
		Size: 462.1 KB (462122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0efe6e8d5895981c45dc711aa05390379a6f7e5ceea618991435f40db1736c5`  
		Last Modified: Thu, 10 Aug 2023 03:07:40 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c66dfda490f2720f8d21e51546bae9f4e21a4b3b76b29f45e18435544c66a7c`  
		Last Modified: Thu, 10 Aug 2023 03:07:44 GMT  
		Size: 15.2 MB (15227189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67327c2fc33a0a30f2e409ada51c37d6663c07a498c7663987be61f888f7a8`  
		Last Modified: Thu, 10 Aug 2023 03:07:40 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c73910f4e5bd8630e3f4a5c23d004a9f6eff60c9f50af18e4b1d9b5f9ac0aa4`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d17a44e8dc24bdc71a9866c99b7022ca1a00e04acc6bf00dbf794c0550bb79d`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851a0578d2d21e2b22a64fe518454ef0283a718573db4e60e3b4a0121bd4081a`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ab80276792afc4370db678044627f33dabc32a9a987d736686239ed1d85a5b`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dcfba0d938817014a224fd3369379868ad4bd05a910cf582eb5e88ca8630ce`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd3ed16ce737bd3530ec90c77867e59892ce05deebca1a42256c570b86ddf1a`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb186d102ae807e026f9de311625fe281b24e140d91adaa2c46298a163035182`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267fad2b6b29094e45425d6b1d39b3f0a295ee7bbce5489aab9e77a659c7ef09`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608cb1e8b46f127167ebb53ec28593783baa810d0ec8e54a929e2907cea85352`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dadf995868b2bcb1e42a4b48f3df0ccd9a979672da04a75dad7970b567bb793`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4209fa97cbb4a651cae617cf81de393ea0652645a1f00b607c18dfa26834c475`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e65f2bc3967a653972ae76ef447ff72659e620a98280fe5230591a0e7c29cd`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9d8975e744e0f5b82190fc02ef017a7f4e7ffa1dda69f5be10f43ffa554d9e`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef526b9884253387824d19beee5d18eee6650c38429c56acd30286c1ea94da03`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 280.0 KB (280042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0266d9103b52d7b0129a0aa08ddab9c5bdfca0694ed3368c0b9c887941c524a`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:40d5f0aa53bb62f81ccb8625ca40ae2b0057b977b8432daa5d3a76079b9737e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:1b4a86d284b971594d7e30ef09451be59ba84514b612c87b6406e2dfb8e9e23f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2011958834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ae5f48eae2f949ec09ad9f70ff2c2626318e07111bea5b6622116482ac991b0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 02:59:41 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Aug 2023 02:59:41 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:00:57 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('69d2d73c2514ab5ce4f6a60489c79ce4da0e1d4302c85ab584d0a7a7fd0d034bfe5a5caab78c96ac3383ddd7d2e12c3c41fb47c4716909d2a78d448b0289ccec')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Aug 2023 03:00:58 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Aug 2023 03:00:59 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Aug 2023 03:01:00 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Thu, 10 Aug 2023 03:01:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Aug 2023 03:01:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Aug 2023 03:01:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Aug 2023 03:01:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Aug 2023 03:01:03 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Aug 2023 03:01:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Aug 2023 03:01:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Aug 2023 03:01:06 GMT
EXPOSE 80
# Thu, 10 Aug 2023 03:01:06 GMT
EXPOSE 443
# Thu, 10 Aug 2023 03:01:07 GMT
EXPOSE 443/udp
# Thu, 10 Aug 2023 03:01:08 GMT
EXPOSE 2019
# Thu, 10 Aug 2023 03:03:10 GMT
RUN caddy version
# Thu, 10 Aug 2023 03:03:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907ddb8e2b3b8f440ec855971bf77d521900d3faecd1816d7146d89f1c78f408`  
		Last Modified: Thu, 10 Aug 2023 03:07:15 GMT  
		Size: 469.4 KB (469388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d430330f12b22fcc17a5d114d51ba3bb8e62a55f87b67f939d18651c226f927`  
		Last Modified: Thu, 10 Aug 2023 03:07:15 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd493f43c2fb25a7c8540ea353a098f784a6e8d5fe4e9d070e4a1de796cde96c`  
		Last Modified: Thu, 10 Aug 2023 03:07:18 GMT  
		Size: 15.2 MB (15241515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95b32f0fb8252db266318cca24c13f5eea8b8b3c19405b92f1a8b9199e39c5d`  
		Last Modified: Thu, 10 Aug 2023 03:07:14 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7dbc1767506f0f3f5b4d3a9671f97a723014ae1e38cf8056f6257db7917a88`  
		Last Modified: Thu, 10 Aug 2023 03:07:13 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7905b1f85b201367c5a62618ddc55da9a60cbb3da1da40ab60a88c125a5956`  
		Last Modified: Thu, 10 Aug 2023 03:07:13 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce34081b153cf49ce89b2ff4fc81f54a648cefc5d2dbb0f60048b94ba10f43b`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9622cc1048f5f7259d3263b67dd386c5d70ae4cf0a358c33deb3df8cdb316efd`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b1ca0970bf360a0627a1deae2985b658f54b41758f12f4e5448ed1aee3bc82`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503770a8fe554599aa8e6413082b7cb24d7f1faa328deaf28b34ddb2a294972b`  
		Last Modified: Thu, 10 Aug 2023 03:07:11 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea5eee99969c433a1c2f4d0f7fdc838185350144b9d3f20888c2a53cc6f3563`  
		Last Modified: Thu, 10 Aug 2023 03:07:11 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675093fb34c31fff953a92ee1831f09679783e7d3e1d9ff40a962f346d1dc581`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fd64685610dd5572f21efe3fae8cb13537c9deb6693caf4097bf9ec3b4dabe`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540e52aaf0b1acca0c4a9fbb2a60e5ce4bca2c119fbb3bbd86658186b23e3202`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29819bc504b56dacdb0df898ee58e26d8097802c0a5578cd14d4e3ed0655bde7`  
		Last Modified: Thu, 10 Aug 2023 03:07:09 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2157a412d53cd6d3174744de6c1cf5cb0dd03274fe9b36f749525867e4b9bd2`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cfbf0b65ccf78eb536c8a23f0b92fa148268c1fa4a39c1b19c7d9310e53b8d`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7faedca764204aa914e83a3721476c9a6a7f8177d057021e5a1debb81a436808`  
		Last Modified: Thu, 10 Aug 2023 03:07:09 GMT  
		Size: 268.6 KB (268640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86622825a44d72176deccdf0a5e4c9127ebf8f2591211cbdae585e9977363e8`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:32d0082c4ae3fdb4c834f812d8c65442f02e9ea2e037e23a5fa80b0399bbf314
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1906; amd64

### `caddy:2-windowsservercore-ltsc2022` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:144bc31c96841830b174ed1ff2da09ba18881208aae2efd16b3c850953f762f6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1813356270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02028c6ef8441cbf5181f34f78b4740b60dffff030772882302c9ca39f9a6096`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 03:03:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Aug 2023 03:03:52 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:04:21 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('69d2d73c2514ab5ce4f6a60489c79ce4da0e1d4302c85ab584d0a7a7fd0d034bfe5a5caab78c96ac3383ddd7d2e12c3c41fb47c4716909d2a78d448b0289ccec')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Aug 2023 03:04:21 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Aug 2023 03:04:22 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Aug 2023 03:04:23 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Thu, 10 Aug 2023 03:04:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Aug 2023 03:04:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Aug 2023 03:04:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Aug 2023 03:04:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Aug 2023 03:04:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Aug 2023 03:04:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Aug 2023 03:04:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Aug 2023 03:04:29 GMT
EXPOSE 80
# Thu, 10 Aug 2023 03:04:30 GMT
EXPOSE 443
# Thu, 10 Aug 2023 03:04:31 GMT
EXPOSE 443/udp
# Thu, 10 Aug 2023 03:04:32 GMT
EXPOSE 2019
# Thu, 10 Aug 2023 03:04:47 GMT
RUN caddy version
# Thu, 10 Aug 2023 03:04:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee168d3c6067847c3aef71a2a0dfdc70984b0bb6164086b49da7bd27de3ff3e4`  
		Last Modified: Thu, 10 Aug 2023 03:07:41 GMT  
		Size: 462.1 KB (462122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0efe6e8d5895981c45dc711aa05390379a6f7e5ceea618991435f40db1736c5`  
		Last Modified: Thu, 10 Aug 2023 03:07:40 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c66dfda490f2720f8d21e51546bae9f4e21a4b3b76b29f45e18435544c66a7c`  
		Last Modified: Thu, 10 Aug 2023 03:07:44 GMT  
		Size: 15.2 MB (15227189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67327c2fc33a0a30f2e409ada51c37d6663c07a498c7663987be61f888f7a8`  
		Last Modified: Thu, 10 Aug 2023 03:07:40 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c73910f4e5bd8630e3f4a5c23d004a9f6eff60c9f50af18e4b1d9b5f9ac0aa4`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d17a44e8dc24bdc71a9866c99b7022ca1a00e04acc6bf00dbf794c0550bb79d`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851a0578d2d21e2b22a64fe518454ef0283a718573db4e60e3b4a0121bd4081a`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ab80276792afc4370db678044627f33dabc32a9a987d736686239ed1d85a5b`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dcfba0d938817014a224fd3369379868ad4bd05a910cf582eb5e88ca8630ce`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd3ed16ce737bd3530ec90c77867e59892ce05deebca1a42256c570b86ddf1a`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb186d102ae807e026f9de311625fe281b24e140d91adaa2c46298a163035182`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267fad2b6b29094e45425d6b1d39b3f0a295ee7bbce5489aab9e77a659c7ef09`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608cb1e8b46f127167ebb53ec28593783baa810d0ec8e54a929e2907cea85352`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dadf995868b2bcb1e42a4b48f3df0ccd9a979672da04a75dad7970b567bb793`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4209fa97cbb4a651cae617cf81de393ea0652645a1f00b607c18dfa26834c475`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e65f2bc3967a653972ae76ef447ff72659e620a98280fe5230591a0e7c29cd`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9d8975e744e0f5b82190fc02ef017a7f4e7ffa1dda69f5be10f43ffa554d9e`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef526b9884253387824d19beee5d18eee6650c38429c56acd30286c1ea94da03`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 280.0 KB (280042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0266d9103b52d7b0129a0aa08ddab9c5bdfca0694ed3368c0b9c887941c524a`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7`

```console
$ docker pull caddy@sha256:6c60e52f0acf862774d17f362aadc4895667d42b24ca6e74ee1e7f09a1363424
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4737; amd64
	-	windows version 10.0.20348.1906; amd64

### `caddy:2.7` - linux; amd64

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

### `caddy:2.7` - linux; arm variant v6

```console
$ docker pull caddy@sha256:dc698bd1b82521df87ea42fbf48c98d10133ec962497ac80527b65769ceb6a9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17690701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3775ac20cca67f4d547f26f5984a989b9407b0c4129fd6cd86dbb3359249acd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:38:27 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:49:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:49:14 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:49:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:49:16 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:49:16 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:49:18 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:49:18 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:49:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172ef460a93549b8a3e73f6a515bccad93512788d1e8f095e7230ba41967c25a`  
		Last Modified: Wed, 09 Aug 2023 03:38:53 GMT  
		Size: 347.7 KB (347686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7aae78767a581df85fd1a51ccd646619aec320896ca016ef0f05a41b16bcbfe`  
		Last Modified: Mon, 14 Aug 2023 17:49:36 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5244db1c019e66038874df2b8b92c74437f6d355802bfccada90c9d8bd8d29`  
		Last Modified: Mon, 14 Aug 2023 17:49:38 GMT  
		Size: 14.2 MB (14190701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - linux; arm variant v7

```console
$ docker pull caddy@sha256:e9cb1245e1c134e25a0ec0803e5132ba9ba92d0a4ad85db3f73bd2c3188cf70e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17414619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df6e2a1f4c707dc77276814a27ac22a7b5de268780603d8e08324130e1fc563`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:51:41 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:57:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:57:17 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:57:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:57:20 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:57:20 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:57:21 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:57:21 GMT
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
	-	`sha256:46e1b3e18d5e992f1805072b2d52405d575830bdce21726ef99dea99e31d8277`  
		Last Modified: Mon, 14 Aug 2023 17:57:42 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2b7485982d191f9dc0498d5b940d14df575f36ca66876b92d3ca09ff9386b2`  
		Last Modified: Mon, 14 Aug 2023 17:57:48 GMT  
		Size: 14.2 MB (14163172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:db04154ce5f7a7f4d058567375880cdc6b1a3675095ad576f9886f39f1374afc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17329640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:731c0ae21a974e5708c4a8006250893bca5a2ecad43babf2a0a95a60fc61d6cd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:09:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:39:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:39:19 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:39:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:39:21 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:39:21 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:39:22 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:39:22 GMT
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
	-	`sha256:f7488af8b96c79b6db13955a0302653c4e9f314d0833201984ae06c1ed697f06`  
		Last Modified: Mon, 14 Aug 2023 17:39:41 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9600da6e7e51b9083b29f3c7de592fa45e7765ca5ffe8d2abf7cc99c50578fe`  
		Last Modified: Mon, 14 Aug 2023 17:39:43 GMT  
		Size: 13.6 MB (13630728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - linux; ppc64le

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

### `caddy:2.7` - linux; s390x

```console
$ docker pull caddy@sha256:3b3d4b80e160105a760ad62b32c497245d69676e6053c2a7b61bc5c6fc178fd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.0 MB (17984968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a63d05bc7601e47460ff86bc91380fd9407c0b4886b80836ac3aadb436f68e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:14:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:41:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:41:39 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:41:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:41:43 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:41:43 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:41:44 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:41:44 GMT
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
	-	`sha256:308478977890baa82477ee70a3065fb9da2080efcc95facf1a87ac021b06a8e9`  
		Last Modified: Mon, 14 Aug 2023 17:42:17 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fe1cbba37a3c1c2f6ba50e59e5c238c8d83ffca820ef709108b9e3253af757`  
		Last Modified: Mon, 14 Aug 2023 17:42:19 GMT  
		Size: 14.4 MB (14408320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:1b4a86d284b971594d7e30ef09451be59ba84514b612c87b6406e2dfb8e9e23f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2011958834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ae5f48eae2f949ec09ad9f70ff2c2626318e07111bea5b6622116482ac991b0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 02:59:41 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Aug 2023 02:59:41 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:00:57 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('69d2d73c2514ab5ce4f6a60489c79ce4da0e1d4302c85ab584d0a7a7fd0d034bfe5a5caab78c96ac3383ddd7d2e12c3c41fb47c4716909d2a78d448b0289ccec')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Aug 2023 03:00:58 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Aug 2023 03:00:59 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Aug 2023 03:01:00 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Thu, 10 Aug 2023 03:01:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Aug 2023 03:01:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Aug 2023 03:01:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Aug 2023 03:01:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Aug 2023 03:01:03 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Aug 2023 03:01:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Aug 2023 03:01:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Aug 2023 03:01:06 GMT
EXPOSE 80
# Thu, 10 Aug 2023 03:01:06 GMT
EXPOSE 443
# Thu, 10 Aug 2023 03:01:07 GMT
EXPOSE 443/udp
# Thu, 10 Aug 2023 03:01:08 GMT
EXPOSE 2019
# Thu, 10 Aug 2023 03:03:10 GMT
RUN caddy version
# Thu, 10 Aug 2023 03:03:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907ddb8e2b3b8f440ec855971bf77d521900d3faecd1816d7146d89f1c78f408`  
		Last Modified: Thu, 10 Aug 2023 03:07:15 GMT  
		Size: 469.4 KB (469388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d430330f12b22fcc17a5d114d51ba3bb8e62a55f87b67f939d18651c226f927`  
		Last Modified: Thu, 10 Aug 2023 03:07:15 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd493f43c2fb25a7c8540ea353a098f784a6e8d5fe4e9d070e4a1de796cde96c`  
		Last Modified: Thu, 10 Aug 2023 03:07:18 GMT  
		Size: 15.2 MB (15241515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95b32f0fb8252db266318cca24c13f5eea8b8b3c19405b92f1a8b9199e39c5d`  
		Last Modified: Thu, 10 Aug 2023 03:07:14 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7dbc1767506f0f3f5b4d3a9671f97a723014ae1e38cf8056f6257db7917a88`  
		Last Modified: Thu, 10 Aug 2023 03:07:13 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7905b1f85b201367c5a62618ddc55da9a60cbb3da1da40ab60a88c125a5956`  
		Last Modified: Thu, 10 Aug 2023 03:07:13 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce34081b153cf49ce89b2ff4fc81f54a648cefc5d2dbb0f60048b94ba10f43b`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9622cc1048f5f7259d3263b67dd386c5d70ae4cf0a358c33deb3df8cdb316efd`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b1ca0970bf360a0627a1deae2985b658f54b41758f12f4e5448ed1aee3bc82`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503770a8fe554599aa8e6413082b7cb24d7f1faa328deaf28b34ddb2a294972b`  
		Last Modified: Thu, 10 Aug 2023 03:07:11 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea5eee99969c433a1c2f4d0f7fdc838185350144b9d3f20888c2a53cc6f3563`  
		Last Modified: Thu, 10 Aug 2023 03:07:11 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675093fb34c31fff953a92ee1831f09679783e7d3e1d9ff40a962f346d1dc581`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fd64685610dd5572f21efe3fae8cb13537c9deb6693caf4097bf9ec3b4dabe`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540e52aaf0b1acca0c4a9fbb2a60e5ce4bca2c119fbb3bbd86658186b23e3202`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29819bc504b56dacdb0df898ee58e26d8097802c0a5578cd14d4e3ed0655bde7`  
		Last Modified: Thu, 10 Aug 2023 03:07:09 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2157a412d53cd6d3174744de6c1cf5cb0dd03274fe9b36f749525867e4b9bd2`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cfbf0b65ccf78eb536c8a23f0b92fa148268c1fa4a39c1b19c7d9310e53b8d`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7faedca764204aa914e83a3721476c9a6a7f8177d057021e5a1debb81a436808`  
		Last Modified: Thu, 10 Aug 2023 03:07:09 GMT  
		Size: 268.6 KB (268640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86622825a44d72176deccdf0a5e4c9127ebf8f2591211cbdae585e9977363e8`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:144bc31c96841830b174ed1ff2da09ba18881208aae2efd16b3c850953f762f6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1813356270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02028c6ef8441cbf5181f34f78b4740b60dffff030772882302c9ca39f9a6096`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 03:03:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Aug 2023 03:03:52 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:04:21 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('69d2d73c2514ab5ce4f6a60489c79ce4da0e1d4302c85ab584d0a7a7fd0d034bfe5a5caab78c96ac3383ddd7d2e12c3c41fb47c4716909d2a78d448b0289ccec')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Aug 2023 03:04:21 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Aug 2023 03:04:22 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Aug 2023 03:04:23 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Thu, 10 Aug 2023 03:04:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Aug 2023 03:04:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Aug 2023 03:04:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Aug 2023 03:04:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Aug 2023 03:04:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Aug 2023 03:04:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Aug 2023 03:04:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Aug 2023 03:04:29 GMT
EXPOSE 80
# Thu, 10 Aug 2023 03:04:30 GMT
EXPOSE 443
# Thu, 10 Aug 2023 03:04:31 GMT
EXPOSE 443/udp
# Thu, 10 Aug 2023 03:04:32 GMT
EXPOSE 2019
# Thu, 10 Aug 2023 03:04:47 GMT
RUN caddy version
# Thu, 10 Aug 2023 03:04:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee168d3c6067847c3aef71a2a0dfdc70984b0bb6164086b49da7bd27de3ff3e4`  
		Last Modified: Thu, 10 Aug 2023 03:07:41 GMT  
		Size: 462.1 KB (462122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0efe6e8d5895981c45dc711aa05390379a6f7e5ceea618991435f40db1736c5`  
		Last Modified: Thu, 10 Aug 2023 03:07:40 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c66dfda490f2720f8d21e51546bae9f4e21a4b3b76b29f45e18435544c66a7c`  
		Last Modified: Thu, 10 Aug 2023 03:07:44 GMT  
		Size: 15.2 MB (15227189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67327c2fc33a0a30f2e409ada51c37d6663c07a498c7663987be61f888f7a8`  
		Last Modified: Thu, 10 Aug 2023 03:07:40 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c73910f4e5bd8630e3f4a5c23d004a9f6eff60c9f50af18e4b1d9b5f9ac0aa4`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d17a44e8dc24bdc71a9866c99b7022ca1a00e04acc6bf00dbf794c0550bb79d`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851a0578d2d21e2b22a64fe518454ef0283a718573db4e60e3b4a0121bd4081a`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ab80276792afc4370db678044627f33dabc32a9a987d736686239ed1d85a5b`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dcfba0d938817014a224fd3369379868ad4bd05a910cf582eb5e88ca8630ce`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd3ed16ce737bd3530ec90c77867e59892ce05deebca1a42256c570b86ddf1a`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb186d102ae807e026f9de311625fe281b24e140d91adaa2c46298a163035182`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267fad2b6b29094e45425d6b1d39b3f0a295ee7bbce5489aab9e77a659c7ef09`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608cb1e8b46f127167ebb53ec28593783baa810d0ec8e54a929e2907cea85352`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dadf995868b2bcb1e42a4b48f3df0ccd9a979672da04a75dad7970b567bb793`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4209fa97cbb4a651cae617cf81de393ea0652645a1f00b607c18dfa26834c475`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e65f2bc3967a653972ae76ef447ff72659e620a98280fe5230591a0e7c29cd`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9d8975e744e0f5b82190fc02ef017a7f4e7ffa1dda69f5be10f43ffa554d9e`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef526b9884253387824d19beee5d18eee6650c38429c56acd30286c1ea94da03`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 280.0 KB (280042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0266d9103b52d7b0129a0aa08ddab9c5bdfca0694ed3368c0b9c887941c524a`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-alpine`

```console
$ docker pull caddy@sha256:00e7c43c571e7036a06830652d919a83c140041d6f98f0ee30c2764f01b8fd6d
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

### `caddy:2.7-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:dc698bd1b82521df87ea42fbf48c98d10133ec962497ac80527b65769ceb6a9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17690701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3775ac20cca67f4d547f26f5984a989b9407b0c4129fd6cd86dbb3359249acd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:38:27 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:49:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:49:14 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:49:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:49:16 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:49:16 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:49:18 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:49:18 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:49:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172ef460a93549b8a3e73f6a515bccad93512788d1e8f095e7230ba41967c25a`  
		Last Modified: Wed, 09 Aug 2023 03:38:53 GMT  
		Size: 347.7 KB (347686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7aae78767a581df85fd1a51ccd646619aec320896ca016ef0f05a41b16bcbfe`  
		Last Modified: Mon, 14 Aug 2023 17:49:36 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5244db1c019e66038874df2b8b92c74437f6d355802bfccada90c9d8bd8d29`  
		Last Modified: Mon, 14 Aug 2023 17:49:38 GMT  
		Size: 14.2 MB (14190701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:e9cb1245e1c134e25a0ec0803e5132ba9ba92d0a4ad85db3f73bd2c3188cf70e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17414619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df6e2a1f4c707dc77276814a27ac22a7b5de268780603d8e08324130e1fc563`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:51:41 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:57:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:57:17 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:57:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:57:20 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:57:20 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:57:21 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:57:21 GMT
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
	-	`sha256:46e1b3e18d5e992f1805072b2d52405d575830bdce21726ef99dea99e31d8277`  
		Last Modified: Mon, 14 Aug 2023 17:57:42 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2b7485982d191f9dc0498d5b940d14df575f36ca66876b92d3ca09ff9386b2`  
		Last Modified: Mon, 14 Aug 2023 17:57:48 GMT  
		Size: 14.2 MB (14163172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:db04154ce5f7a7f4d058567375880cdc6b1a3675095ad576f9886f39f1374afc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17329640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:731c0ae21a974e5708c4a8006250893bca5a2ecad43babf2a0a95a60fc61d6cd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:09:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:39:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:39:19 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:39:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:39:21 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:39:21 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:39:22 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:39:22 GMT
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
	-	`sha256:f7488af8b96c79b6db13955a0302653c4e9f314d0833201984ae06c1ed697f06`  
		Last Modified: Mon, 14 Aug 2023 17:39:41 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9600da6e7e51b9083b29f3c7de592fa45e7765ca5ffe8d2abf7cc99c50578fe`  
		Last Modified: Mon, 14 Aug 2023 17:39:43 GMT  
		Size: 13.6 MB (13630728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-alpine` - linux; ppc64le

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

### `caddy:2.7-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:3b3d4b80e160105a760ad62b32c497245d69676e6053c2a7b61bc5c6fc178fd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.0 MB (17984968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a63d05bc7601e47460ff86bc91380fd9407c0b4886b80836ac3aadb436f68e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:14:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:41:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:41:39 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:41:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:41:43 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:41:43 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:41:44 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:41:44 GMT
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
	-	`sha256:308478977890baa82477ee70a3065fb9da2080efcc95facf1a87ac021b06a8e9`  
		Last Modified: Mon, 14 Aug 2023 17:42:17 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fe1cbba37a3c1c2f6ba50e59e5c238c8d83ffca820ef709108b9e3253af757`  
		Last Modified: Mon, 14 Aug 2023 17:42:19 GMT  
		Size: 14.4 MB (14408320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-builder`

```console
$ docker pull caddy@sha256:b93978cf962da183e6d11a754d51de5f033da2708c588c9ba27cd0ce2c3b582c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4737; amd64
	-	windows version 10.0.20348.1906; amd64

### `caddy:2.7-builder` - linux; amd64

```console
$ docker pull caddy@sha256:7abb7723020bab7b367d33786efcfca5d4a4f884ec306308d4a5513f14cdc20c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110901544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e24e6bda832eff522a3ea76a20f3e8055f2ecefa2f16c9f5485ad066bebf9a14`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:36:47 GMT
RUN apk add --no-cache ca-certificates
# Wed, 09 Aug 2023 04:41:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Aug 2023 04:41:57 GMT
ENV GOLANG_VERSION=1.20.7
# Wed, 09 Aug 2023 04:43:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 09 Aug 2023 04:43:29 GMT
ENV GOPATH=/go
# Wed, 09 Aug 2023 04:43:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Aug 2023 04:43:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 09 Aug 2023 04:43:30 GMT
WORKDIR /go
# Wed, 09 Aug 2023 10:26:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 09 Aug 2023 10:26:17 GMT
ENV XCADDY_VERSION=v0.3.4
# Wed, 09 Aug 2023 10:26:17 GMT
ENV CADDY_VERSION=v2.7.2
# Wed, 09 Aug 2023 10:26:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Aug 2023 10:26:17 GMT
ENV XCADDY_SETCAP=1
# Wed, 09 Aug 2023 10:26:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68ab15d90eb70c23e8b13c3935b194fc1b638f8c0fee6506a109dcee082c20d6e07890320a876b13eb23b5a7a0617daa28fe8af24dcb0dcb3eca9ea74dc76713' ;; 		armhf)   binArch='armv6'; checksum='2853413e63ac29f296b1c44696022febc8b29c4b37fb20442b635903a0b79d523ca00896dfce3e40f5894dd297b345ac007af0ddffccaada843c7de61d334134' ;; 		armv7)   binArch='armv7'; checksum='c59e93ba270705b2312f6a70552f2a345cec91cc3504233785cb46fa4b644a47e520bb29dfbf519f814bb13d0bbea213976fd7b059883eab2b091913f9ed393f' ;; 		aarch64) binArch='arm64'; checksum='df4c58e97931ca58b7a38d245948912b817e952a2961ff583744039ca68a584a303f7cbfdb33392c84d8f76f5b30f206d9f84a04f547043a3d1fa5282b0fd544' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2795d5b7546bd10ff3cd21a393597281e42e1043164536e01e18fb56047ba5b396493a086bb2d90e8ede9a54b5208e947ecaacccca4a8550704fb3f8a17dd771' ;; 		s390x)   binArch='s390x'; checksum='2ed85231aac36e3af873e3fdf4f6b6378b55dcc17743d24b28b3b48d6622fde73aae58eed124082478a0b841c338d64caa0b0be302545a79092a97cf205f1b29' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 09 Aug 2023 10:26:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 09 Aug 2023 10:26:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d48a809fc2256f8aa0aeee47998488d64409855adba00a7cb3007ab9f3286e`  
		Last Modified: Wed, 09 Aug 2023 03:37:02 GMT  
		Size: 284.7 KB (284693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e790db5857269a95a948a96f0e3304c851351e588262d58504700b2e73fb7fe`  
		Last Modified: Wed, 09 Aug 2023 04:47:32 GMT  
		Size: 101.0 MB (100954810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727f4e1a48a681e22437b6c14b04a4e287386f50f1be21ef490a1e28fd276a91`  
		Last Modified: Wed, 09 Aug 2023 04:47:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a272b880a0f8927853947bb9b16e005e2824b1685a89cc015f4e4694c441ed0e`  
		Last Modified: Wed, 09 Aug 2023 10:26:35 GMT  
		Size: 5.0 MB (4958652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e328d3f19ca0bf59908eb26cf5d7b5f94d2aa3e53eb5426f11ddaceca7d024`  
		Last Modified: Wed, 09 Aug 2023 10:26:35 GMT  
		Size: 1.3 MB (1301217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3115a3b8c7625246591f7ffa414a109f6c26f09066d0a9b9c0aba053e2a13c02`  
		Last Modified: Wed, 09 Aug 2023 10:26:35 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:289b1f78db36a7524bbae6562b80b29fe5585984effd44a3e22146fcbf4ab824
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108301221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98ac734398939dbe1f4c664f493d34b5353c438189c6b58b3e6e4d92186a8f80`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:12:05 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:12:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:12:40 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 23:14:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 23:14:36 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 23:14:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:14:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 23:14:37 GMT
WORKDIR /go
# Wed, 09 Aug 2023 03:38:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:49:20 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:49:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:49:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:49:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8564ce36feee688566265012773f1c8c7c046ceefe86ca763eb702682f4e6e75`  
		Last Modified: Tue, 08 Aug 2023 23:15:06 GMT  
		Size: 284.9 KB (284876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b139603b026cc15bf570c9cf012fc165cb74821883c7c7c534fe6ed189b5a2`  
		Last Modified: Tue, 08 Aug 2023 23:16:29 GMT  
		Size: 98.7 MB (98671161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b2f37c2778ffd2e158ad31438d6802c214dfa5d79e06dc9af2d8320828e148`  
		Last Modified: Tue, 08 Aug 2023 23:16:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f22c305527b162efa854ac3e1963e59e7fb8f2c71838222c56462b9809481ed`  
		Last Modified: Wed, 09 Aug 2023 03:39:10 GMT  
		Size: 5.0 MB (4951147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5520daf22ad222fbe3c81bbd6afa0c912b3817f0f432a35a939f9870a8512af`  
		Last Modified: Mon, 14 Aug 2023 17:49:51 GMT  
		Size: 1.2 MB (1248666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f8fe3942ebea0d37a8324080324eb0bca35e859273e7bac44381e31a0fa714`  
		Last Modified: Mon, 14 Aug 2023 17:49:51 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:dcbac62a4e9d8d10345a7f20ac37a814b45633ed4b050a14fa20aef08590597a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107386270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0adee903aaec70e29acbd506823b19cc477dc7788e545d1b88316b9ec0e9c154`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:39:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 01:39:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 01:40:29 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 01:42:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 01:42:12 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 01:42:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 01:42:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 01:42:13 GMT
WORKDIR /go
# Tue, 08 Aug 2023 01:51:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:57:24 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:57:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:57:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:57:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47bd95d78f565e902bafd0264a979eb4f6f71e22c0464011bf9db6feb0579e6`  
		Last Modified: Tue, 08 Aug 2023 01:48:34 GMT  
		Size: 284.1 KB (284073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a674106498848b269b5cb69fb938d3dc97247d02cb1aa3927b7a7469724e950`  
		Last Modified: Tue, 08 Aug 2023 01:49:43 GMT  
		Size: 98.5 MB (98454659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1902a68db0b07b05ab7d2f3e48ca8f1d22951b498f6ff9027bdc91a5e7e830`  
		Last Modified: Tue, 08 Aug 2023 01:49:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9caf1886c556e441f6f89cd1cb00e1b950d9d8fcad8812a988fbb59caf0b0ba5`  
		Last Modified: Tue, 08 Aug 2023 01:52:22 GMT  
		Size: 4.5 MB (4501403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c28b1afe92de619aa5de35a2f610dc68af6b39c6cd300ef8426738a739366a2`  
		Last Modified: Mon, 14 Aug 2023 17:58:00 GMT  
		Size: 1.2 MB (1246092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6fe75fd67d7668d6aeca167419514f45cb72ec61bd61a9fc32e25b5c928dba6`  
		Last Modified: Mon, 14 Aug 2023 17:58:00 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:9ad7390f7aa878bd4d6750dab9611c7397630fc15a7f80304eea3d3f64dcfe4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.0 MB (105987240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c79cdcd45a4a61e8fe257b7917335ede1523a72d1c2ef2eb9115783a5379f5ea`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:10:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:10:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:10:53 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 23:11:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 23:11:59 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 23:11:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:12:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 23:12:00 GMT
WORKDIR /go
# Wed, 09 Aug 2023 10:10:28 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:39:25 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:39:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:39:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:39:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54e960e981301b0098c80d2e61d694333b5ab480a007a3a8d0fa629662d377`  
		Last Modified: Tue, 08 Aug 2023 23:14:21 GMT  
		Size: 286.3 KB (286298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20ccffba14f84f51f896ae916a3dd045a0b0d08dc27d53f7d6a9dc5687c3501`  
		Last Modified: Tue, 08 Aug 2023 23:15:23 GMT  
		Size: 96.1 MB (96117263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d452dd4d3acc29d43b0be67bcc0c121814601787c7fd45e8260687d2cc8983`  
		Last Modified: Tue, 08 Aug 2023 23:15:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d371a704ab9a071c89db966e268fe56aad2288363a849d10eb032d47cd10848b`  
		Last Modified: Wed, 09 Aug 2023 10:10:48 GMT  
		Size: 5.1 MB (5053901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5e38cf28101c20845f7f103114793f73691285da6ac006db5cb28c20bc8000`  
		Last Modified: Mon, 14 Aug 2023 17:39:55 GMT  
		Size: 1.2 MB (1198449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d1b8334b836b303a87ddda4bfba4af764950afa40c2c263cca11ed8b53a8c6`  
		Last Modified: Mon, 14 Aug 2023 17:39:54 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:e3543706f8faff15a067252f4e5760bb4cb3e12ff81b7a932052bc013ecc4151
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106660406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37b7339021535bddbd7f4a89deae282741ae3163c68d69d7d5d035167f7d440`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:25:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 00:25:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 00:26:56 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 00:29:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 00:29:34 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 00:29:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 00:29:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 00:29:36 GMT
WORKDIR /go
# Tue, 08 Aug 2023 00:44:40 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 08 Aug 2023 00:44:41 GMT
ENV XCADDY_VERSION=v0.3.4
# Tue, 08 Aug 2023 00:44:42 GMT
ENV CADDY_VERSION=v2.7.2
# Tue, 08 Aug 2023 00:44:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 08 Aug 2023 00:44:43 GMT
ENV XCADDY_SETCAP=1
# Tue, 08 Aug 2023 00:44:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68ab15d90eb70c23e8b13c3935b194fc1b638f8c0fee6506a109dcee082c20d6e07890320a876b13eb23b5a7a0617daa28fe8af24dcb0dcb3eca9ea74dc76713' ;; 		armhf)   binArch='armv6'; checksum='2853413e63ac29f296b1c44696022febc8b29c4b37fb20442b635903a0b79d523ca00896dfce3e40f5894dd297b345ac007af0ddffccaada843c7de61d334134' ;; 		armv7)   binArch='armv7'; checksum='c59e93ba270705b2312f6a70552f2a345cec91cc3504233785cb46fa4b644a47e520bb29dfbf519f814bb13d0bbea213976fd7b059883eab2b091913f9ed393f' ;; 		aarch64) binArch='arm64'; checksum='df4c58e97931ca58b7a38d245948912b817e952a2961ff583744039ca68a584a303f7cbfdb33392c84d8f76f5b30f206d9f84a04f547043a3d1fa5282b0fd544' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2795d5b7546bd10ff3cd21a393597281e42e1043164536e01e18fb56047ba5b396493a086bb2d90e8ede9a54b5208e947ecaacccca4a8550704fb3f8a17dd771' ;; 		s390x)   binArch='s390x'; checksum='2ed85231aac36e3af873e3fdf4f6b6378b55dcc17743d24b28b3b48d6622fde73aae58eed124082478a0b841c338d64caa0b0be302545a79092a97cf205f1b29' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 08 Aug 2023 00:44:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 08 Aug 2023 00:44:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c966ad2cdd35689da92e7c8fd39bd37cd6080c484e6ccaf00672c154cd4f6c2a`  
		Last Modified: Tue, 08 Aug 2023 00:39:35 GMT  
		Size: 286.7 KB (286662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7816c9df7e6881fdd62dfcc6d743edcc2c3ca9220542437a2e5fdcfa0e4548`  
		Last Modified: Tue, 08 Aug 2023 00:41:09 GMT  
		Size: 96.6 MB (96591770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d34a514a03c5af8a03dfe8c4fbfd50b2ec61591d24080f8be8bf722904f541`  
		Last Modified: Tue, 08 Aug 2023 00:40:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802af1410e20c34900a811878ca2fa2e5dc79daeb92a53b94588831011ad81fc`  
		Last Modified: Tue, 08 Aug 2023 00:45:40 GMT  
		Size: 5.2 MB (5249966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5fe808e6f175a659981d31b9687526a651f4d40bce158c2baa204fcfcf2820`  
		Last Modified: Tue, 08 Aug 2023 00:45:39 GMT  
		Size: 1.2 MB (1185194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681275e7741131c55614b72469583c04861fb9344cde71f5dc2d00b75af4737b`  
		Last Modified: Tue, 08 Aug 2023 00:45:39 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - linux; s390x

```console
$ docker pull caddy@sha256:4c76dac9b235685647bce5e644408f9537fd2a98243936db0666252a4ec24739
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110727449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84fe6eea8994d5e82ec6e85ed4c441f0a89b9cb461829805dd3eeb9d892d49a9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:41 GMT
RUN apk add --no-cache ca-certificates
# Mon, 07 Aug 2023 20:19:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Aug 2023 20:21:06 GMT
ENV GOLANG_VERSION=1.20.7
# Mon, 07 Aug 2023 20:23:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 07 Aug 2023 20:23:05 GMT
ENV GOPATH=/go
# Mon, 07 Aug 2023 20:23:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Aug 2023 20:23:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 07 Aug 2023 20:23:06 GMT
WORKDIR /go
# Tue, 08 Aug 2023 05:25:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:41:51 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:41:52 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:41:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:41:52 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:41:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:41:54 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:41:54 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec90be18226e5c99d10161aed1a143f4134093c55b4d6979bbdbbe4b0683eb11`  
		Last Modified: Mon, 07 Aug 2023 20:30:59 GMT  
		Size: 285.1 KB (285089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c751f85e4ba6e9bbada0b11691d914b2ec2c689bb0dca6b9cbe994488d0e3e`  
		Last Modified: Mon, 07 Aug 2023 20:31:56 GMT  
		Size: 100.9 MB (100865267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2d202223222826c8580d85b8d7dd6baa8ed1cad84ba5cf47dab23eaeeae7e9`  
		Last Modified: Mon, 07 Aug 2023 20:31:43 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0359ada615d16e203e1d40a49b896060013c2952c2982ae73b141cc291305a4c`  
		Last Modified: Tue, 08 Aug 2023 05:25:47 GMT  
		Size: 5.1 MB (5099943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1039996d136f688a91d291dcf3dbb995607af1f245f1741d8ad0c5f73cec1b01`  
		Last Modified: Mon, 14 Aug 2023 17:42:27 GMT  
		Size: 1.3 MB (1262391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17e7bfc7e0d6b6a7f70b22841fe42427f0fb6372b17c71c8063c50d7c8e73c1`  
		Last Modified: Mon, 14 Aug 2023 17:42:27 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:a6ebd264677820f38a44fb346c24e5b3cc1406cf5f975a99a089e14f2cfeb623
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2132345169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec0a81535ff140c0b08b259f2eb43a2face74a8aaeed3cc1ac39ef9b4e90c3f6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:39:54 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:39:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:41:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:41:12 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:42:07 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:53:35 GMT
ENV GOLANG_VERSION=1.20.7
# Thu, 10 Aug 2023 00:56:38 GMT
RUN $url = 'https://dl.google.com/go/go1.20.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '736dc6c7fcab1c96b682c8c93e38d7e371e62a17d34cb2c37d451a1147f66af9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:56:40 GMT
WORKDIR C:\go
# Thu, 10 Aug 2023 03:04:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 03:04:56 GMT
ENV XCADDY_VERSION=v0.3.4
# Thu, 10 Aug 2023 03:04:57 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:04:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Aug 2023 03:06:01 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('542b4c083852d41081186c79757b66ff3c26248f72ed461dbc038b51687d0a8a8ce8eee69e3b5a1d43360c48b3405b611b940fa378debe98aaa0b3c5aebfa218')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 10 Aug 2023 03:06:02 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594083c5c2094c95b4e52723d54c14e0d70881f4f176720c3170012275accc3b`  
		Last Modified: Thu, 10 Aug 2023 01:02:54 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e2c2a5b75ced3a3a50be088c4a6c2d7df926b1fe6515b2d0c021312e3642f4`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d28688050deeec928289543beadf5c75bb2a8246576cb7c066e23818016217`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e5fbc50e7e0fefb7c9e349038ecb00ed5c000bcab8c4d82b1e1000c4273c01`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0544e07bd9df923e11e09c7dc042da614f2f14589eb6fa79005ebbbf2731e97d`  
		Last Modified: Thu, 10 Aug 2023 01:02:57 GMT  
		Size: 25.6 MB (25560980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555a82506c4fcec2bd90ae77756e5b03788e30c89f1a3820aa0b6a7ae6ad58ae`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bcfb422b104764156fc5ba099b5e3ae9fa9f760fd2db1c21acd8969b3d73de`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 220.8 KB (220796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c6aa0a5a1689ed800c4ef72c1b9febf207840fd2c6abfe4bb460e2e2bfb0b0`  
		Last Modified: Thu, 10 Aug 2023 01:05:03 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53d3379322a67b2413189cc2b779d22cb4093124343c8bb17fdf720b7b49fda`  
		Last Modified: Thu, 10 Aug 2023 01:05:25 GMT  
		Size: 108.9 MB (108911716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b60ccf92610ddbc47a05664785c95215a123e8930afbf6e3e2cefc80e693fd2`  
		Last Modified: Thu, 10 Aug 2023 01:05:04 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2c7d6253e62d61e5e0d2ad331a96cff5175f6c608b2ab4657825b3e3b4b4d0`  
		Last Modified: Thu, 10 Aug 2023 03:08:03 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c54227291fad3a25beb98d755de6f26fee6576e1b807e42c0bb70aa45793b3`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d107b434fabbe0d8d3916744b92501e6f5f8dabf7621ce44432d53d3853b4b8`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b0bcd286241a360f34f20c3842b90b6f53c31abe4d60fcb8f1148e8ba191a3`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5677a754ea49eeeb0b5ed56da2ac0d43c11e3c935c36adc2cc71b95dc7b99c0f`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.7 MB (1679125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4626f9b6f575add3a8f4ac9248f4342e9cb80f9abf696deff5a7bd9aff57fbf1`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:44aba8da329d3ea3489327b5c94e41477f815f943659f4464a2c859ad400dcfd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1933815424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d095c2914283b4b75e4dbb95eb3e7f5ff6db80079dc6981bf1c5fa8355036c99`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:36:23 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:36:24 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:36:25 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:36:26 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:36:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:37:00 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:37:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:50:52 GMT
ENV GOLANG_VERSION=1.20.7
# Thu, 10 Aug 2023 00:53:17 GMT
RUN $url = 'https://dl.google.com/go/go1.20.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '736dc6c7fcab1c96b682c8c93e38d7e371e62a17d34cb2c37d451a1147f66af9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:53:18 GMT
WORKDIR C:\go
# Thu, 10 Aug 2023 03:06:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 03:06:10 GMT
ENV XCADDY_VERSION=v0.3.4
# Thu, 10 Aug 2023 03:06:11 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:06:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Aug 2023 03:06:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('542b4c083852d41081186c79757b66ff3c26248f72ed461dbc038b51687d0a8a8ce8eee69e3b5a1d43360c48b3405b611b940fa378debe98aaa0b3c5aebfa218')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 10 Aug 2023 03:06:35 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877256a6389e5e2563da79ad5bd201e7ee136abf14ff7cb0d4efbf3b24e5f127`  
		Last Modified: Thu, 10 Aug 2023 01:02:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a39df29b3c0b2f7e691c47273110db4a46e5c8e299f6bb95f77a9c61f79872`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8574d63bce1547e3177d0b76237a782a9b016d4880375dcd1a7b6a1c5dee3dc`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ef34b3c96316bcdd92e24c8c4eebdc3a35f245c013ef87edfae0dde091a305`  
		Last Modified: Thu, 10 Aug 2023 01:02:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a481babc5b629f694446a96dba8d77c020257c98334c605aff94162b9a917279`  
		Last Modified: Thu, 10 Aug 2023 01:02:23 GMT  
		Size: 25.6 MB (25554169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281178ea1c103ff07ea7e4fb647eb0dbe4f865742da6ef9944e04f37974fc27c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b5d34adf2aacfe87580143f3e17c635dc8dbd4068377b79b35d665f49bbad9`  
		Last Modified: Thu, 10 Aug 2023 01:02:16 GMT  
		Size: 275.9 KB (275946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02a2e79b5a05c2145c733eefb2add45d1ebefb7a16b93c321f5883c8ced6f1a`  
		Last Modified: Thu, 10 Aug 2023 01:04:30 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd9991b8cfbc481c153abf1625143209f4c4fd40d9443a5a19f4e3613336ad2`  
		Last Modified: Thu, 10 Aug 2023 01:04:53 GMT  
		Size: 108.9 MB (108927695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dc6778f41c3c7d50b8e71668e22880153d6c6794f24c4661fc3d6aa089d0a5`  
		Last Modified: Thu, 10 Aug 2023 01:04:30 GMT  
		Size: 1.5 KB (1547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c5985f015e143065716f5aabf0ecaed537103c5ec07e6c57360204a7787d02`  
		Last Modified: Thu, 10 Aug 2023 03:08:23 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd9cf527e30318df5bccd0be2c9a9716dc073b1f84c1d2c5cadc85adcf2af02`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604bc0fdaac29b943186656363f9267b86b2744da35d6b519a428d494d0a6bd3`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b527a45b48b4328e0ea94e3e2d3f239ed4f960d30ea0b9272cd902aec85c8b`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9ae10f93498ae3f8bbfef69dd561e41337584fb8dcc09fe82ed4971f9787be`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.7 MB (1675642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6218363385083ee3dbece9e5e2fd5c9086be201ca76bd6818b46bb6e591688eb`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-builder-alpine`

```console
$ docker pull caddy@sha256:f921c48f48fcc6d6b234fd185f35b3762f339365402630553bfcca85a8376dbb
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
$ docker pull caddy@sha256:7abb7723020bab7b367d33786efcfca5d4a4f884ec306308d4a5513f14cdc20c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110901544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e24e6bda832eff522a3ea76a20f3e8055f2ecefa2f16c9f5485ad066bebf9a14`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:36:47 GMT
RUN apk add --no-cache ca-certificates
# Wed, 09 Aug 2023 04:41:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Aug 2023 04:41:57 GMT
ENV GOLANG_VERSION=1.20.7
# Wed, 09 Aug 2023 04:43:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 09 Aug 2023 04:43:29 GMT
ENV GOPATH=/go
# Wed, 09 Aug 2023 04:43:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Aug 2023 04:43:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 09 Aug 2023 04:43:30 GMT
WORKDIR /go
# Wed, 09 Aug 2023 10:26:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 09 Aug 2023 10:26:17 GMT
ENV XCADDY_VERSION=v0.3.4
# Wed, 09 Aug 2023 10:26:17 GMT
ENV CADDY_VERSION=v2.7.2
# Wed, 09 Aug 2023 10:26:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Aug 2023 10:26:17 GMT
ENV XCADDY_SETCAP=1
# Wed, 09 Aug 2023 10:26:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68ab15d90eb70c23e8b13c3935b194fc1b638f8c0fee6506a109dcee082c20d6e07890320a876b13eb23b5a7a0617daa28fe8af24dcb0dcb3eca9ea74dc76713' ;; 		armhf)   binArch='armv6'; checksum='2853413e63ac29f296b1c44696022febc8b29c4b37fb20442b635903a0b79d523ca00896dfce3e40f5894dd297b345ac007af0ddffccaada843c7de61d334134' ;; 		armv7)   binArch='armv7'; checksum='c59e93ba270705b2312f6a70552f2a345cec91cc3504233785cb46fa4b644a47e520bb29dfbf519f814bb13d0bbea213976fd7b059883eab2b091913f9ed393f' ;; 		aarch64) binArch='arm64'; checksum='df4c58e97931ca58b7a38d245948912b817e952a2961ff583744039ca68a584a303f7cbfdb33392c84d8f76f5b30f206d9f84a04f547043a3d1fa5282b0fd544' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2795d5b7546bd10ff3cd21a393597281e42e1043164536e01e18fb56047ba5b396493a086bb2d90e8ede9a54b5208e947ecaacccca4a8550704fb3f8a17dd771' ;; 		s390x)   binArch='s390x'; checksum='2ed85231aac36e3af873e3fdf4f6b6378b55dcc17743d24b28b3b48d6622fde73aae58eed124082478a0b841c338d64caa0b0be302545a79092a97cf205f1b29' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 09 Aug 2023 10:26:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 09 Aug 2023 10:26:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d48a809fc2256f8aa0aeee47998488d64409855adba00a7cb3007ab9f3286e`  
		Last Modified: Wed, 09 Aug 2023 03:37:02 GMT  
		Size: 284.7 KB (284693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e790db5857269a95a948a96f0e3304c851351e588262d58504700b2e73fb7fe`  
		Last Modified: Wed, 09 Aug 2023 04:47:32 GMT  
		Size: 101.0 MB (100954810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727f4e1a48a681e22437b6c14b04a4e287386f50f1be21ef490a1e28fd276a91`  
		Last Modified: Wed, 09 Aug 2023 04:47:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a272b880a0f8927853947bb9b16e005e2824b1685a89cc015f4e4694c441ed0e`  
		Last Modified: Wed, 09 Aug 2023 10:26:35 GMT  
		Size: 5.0 MB (4958652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e328d3f19ca0bf59908eb26cf5d7b5f94d2aa3e53eb5426f11ddaceca7d024`  
		Last Modified: Wed, 09 Aug 2023 10:26:35 GMT  
		Size: 1.3 MB (1301217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3115a3b8c7625246591f7ffa414a109f6c26f09066d0a9b9c0aba053e2a13c02`  
		Last Modified: Wed, 09 Aug 2023 10:26:35 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:289b1f78db36a7524bbae6562b80b29fe5585984effd44a3e22146fcbf4ab824
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108301221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98ac734398939dbe1f4c664f493d34b5353c438189c6b58b3e6e4d92186a8f80`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:12:05 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:12:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:12:40 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 23:14:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 23:14:36 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 23:14:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:14:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 23:14:37 GMT
WORKDIR /go
# Wed, 09 Aug 2023 03:38:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:49:20 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:49:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:49:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:49:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8564ce36feee688566265012773f1c8c7c046ceefe86ca763eb702682f4e6e75`  
		Last Modified: Tue, 08 Aug 2023 23:15:06 GMT  
		Size: 284.9 KB (284876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b139603b026cc15bf570c9cf012fc165cb74821883c7c7c534fe6ed189b5a2`  
		Last Modified: Tue, 08 Aug 2023 23:16:29 GMT  
		Size: 98.7 MB (98671161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b2f37c2778ffd2e158ad31438d6802c214dfa5d79e06dc9af2d8320828e148`  
		Last Modified: Tue, 08 Aug 2023 23:16:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f22c305527b162efa854ac3e1963e59e7fb8f2c71838222c56462b9809481ed`  
		Last Modified: Wed, 09 Aug 2023 03:39:10 GMT  
		Size: 5.0 MB (4951147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5520daf22ad222fbe3c81bbd6afa0c912b3817f0f432a35a939f9870a8512af`  
		Last Modified: Mon, 14 Aug 2023 17:49:51 GMT  
		Size: 1.2 MB (1248666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f8fe3942ebea0d37a8324080324eb0bca35e859273e7bac44381e31a0fa714`  
		Last Modified: Mon, 14 Aug 2023 17:49:51 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:dcbac62a4e9d8d10345a7f20ac37a814b45633ed4b050a14fa20aef08590597a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107386270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0adee903aaec70e29acbd506823b19cc477dc7788e545d1b88316b9ec0e9c154`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:39:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 01:39:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 01:40:29 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 01:42:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 01:42:12 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 01:42:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 01:42:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 01:42:13 GMT
WORKDIR /go
# Tue, 08 Aug 2023 01:51:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:57:24 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:57:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:57:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:57:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47bd95d78f565e902bafd0264a979eb4f6f71e22c0464011bf9db6feb0579e6`  
		Last Modified: Tue, 08 Aug 2023 01:48:34 GMT  
		Size: 284.1 KB (284073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a674106498848b269b5cb69fb938d3dc97247d02cb1aa3927b7a7469724e950`  
		Last Modified: Tue, 08 Aug 2023 01:49:43 GMT  
		Size: 98.5 MB (98454659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1902a68db0b07b05ab7d2f3e48ca8f1d22951b498f6ff9027bdc91a5e7e830`  
		Last Modified: Tue, 08 Aug 2023 01:49:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9caf1886c556e441f6f89cd1cb00e1b950d9d8fcad8812a988fbb59caf0b0ba5`  
		Last Modified: Tue, 08 Aug 2023 01:52:22 GMT  
		Size: 4.5 MB (4501403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c28b1afe92de619aa5de35a2f610dc68af6b39c6cd300ef8426738a739366a2`  
		Last Modified: Mon, 14 Aug 2023 17:58:00 GMT  
		Size: 1.2 MB (1246092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6fe75fd67d7668d6aeca167419514f45cb72ec61bd61a9fc32e25b5c928dba6`  
		Last Modified: Mon, 14 Aug 2023 17:58:00 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:9ad7390f7aa878bd4d6750dab9611c7397630fc15a7f80304eea3d3f64dcfe4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.0 MB (105987240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c79cdcd45a4a61e8fe257b7917335ede1523a72d1c2ef2eb9115783a5379f5ea`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:10:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:10:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:10:53 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 23:11:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 23:11:59 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 23:11:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:12:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 23:12:00 GMT
WORKDIR /go
# Wed, 09 Aug 2023 10:10:28 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:39:25 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:39:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:39:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:39:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54e960e981301b0098c80d2e61d694333b5ab480a007a3a8d0fa629662d377`  
		Last Modified: Tue, 08 Aug 2023 23:14:21 GMT  
		Size: 286.3 KB (286298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20ccffba14f84f51f896ae916a3dd045a0b0d08dc27d53f7d6a9dc5687c3501`  
		Last Modified: Tue, 08 Aug 2023 23:15:23 GMT  
		Size: 96.1 MB (96117263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d452dd4d3acc29d43b0be67bcc0c121814601787c7fd45e8260687d2cc8983`  
		Last Modified: Tue, 08 Aug 2023 23:15:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d371a704ab9a071c89db966e268fe56aad2288363a849d10eb032d47cd10848b`  
		Last Modified: Wed, 09 Aug 2023 10:10:48 GMT  
		Size: 5.1 MB (5053901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5e38cf28101c20845f7f103114793f73691285da6ac006db5cb28c20bc8000`  
		Last Modified: Mon, 14 Aug 2023 17:39:55 GMT  
		Size: 1.2 MB (1198449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d1b8334b836b303a87ddda4bfba4af764950afa40c2c263cca11ed8b53a8c6`  
		Last Modified: Mon, 14 Aug 2023 17:39:54 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:e3543706f8faff15a067252f4e5760bb4cb3e12ff81b7a932052bc013ecc4151
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106660406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37b7339021535bddbd7f4a89deae282741ae3163c68d69d7d5d035167f7d440`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:25:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 00:25:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 00:26:56 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 00:29:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 00:29:34 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 00:29:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 00:29:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 00:29:36 GMT
WORKDIR /go
# Tue, 08 Aug 2023 00:44:40 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 08 Aug 2023 00:44:41 GMT
ENV XCADDY_VERSION=v0.3.4
# Tue, 08 Aug 2023 00:44:42 GMT
ENV CADDY_VERSION=v2.7.2
# Tue, 08 Aug 2023 00:44:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 08 Aug 2023 00:44:43 GMT
ENV XCADDY_SETCAP=1
# Tue, 08 Aug 2023 00:44:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68ab15d90eb70c23e8b13c3935b194fc1b638f8c0fee6506a109dcee082c20d6e07890320a876b13eb23b5a7a0617daa28fe8af24dcb0dcb3eca9ea74dc76713' ;; 		armhf)   binArch='armv6'; checksum='2853413e63ac29f296b1c44696022febc8b29c4b37fb20442b635903a0b79d523ca00896dfce3e40f5894dd297b345ac007af0ddffccaada843c7de61d334134' ;; 		armv7)   binArch='armv7'; checksum='c59e93ba270705b2312f6a70552f2a345cec91cc3504233785cb46fa4b644a47e520bb29dfbf519f814bb13d0bbea213976fd7b059883eab2b091913f9ed393f' ;; 		aarch64) binArch='arm64'; checksum='df4c58e97931ca58b7a38d245948912b817e952a2961ff583744039ca68a584a303f7cbfdb33392c84d8f76f5b30f206d9f84a04f547043a3d1fa5282b0fd544' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2795d5b7546bd10ff3cd21a393597281e42e1043164536e01e18fb56047ba5b396493a086bb2d90e8ede9a54b5208e947ecaacccca4a8550704fb3f8a17dd771' ;; 		s390x)   binArch='s390x'; checksum='2ed85231aac36e3af873e3fdf4f6b6378b55dcc17743d24b28b3b48d6622fde73aae58eed124082478a0b841c338d64caa0b0be302545a79092a97cf205f1b29' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 08 Aug 2023 00:44:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 08 Aug 2023 00:44:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c966ad2cdd35689da92e7c8fd39bd37cd6080c484e6ccaf00672c154cd4f6c2a`  
		Last Modified: Tue, 08 Aug 2023 00:39:35 GMT  
		Size: 286.7 KB (286662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7816c9df7e6881fdd62dfcc6d743edcc2c3ca9220542437a2e5fdcfa0e4548`  
		Last Modified: Tue, 08 Aug 2023 00:41:09 GMT  
		Size: 96.6 MB (96591770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d34a514a03c5af8a03dfe8c4fbfd50b2ec61591d24080f8be8bf722904f541`  
		Last Modified: Tue, 08 Aug 2023 00:40:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802af1410e20c34900a811878ca2fa2e5dc79daeb92a53b94588831011ad81fc`  
		Last Modified: Tue, 08 Aug 2023 00:45:40 GMT  
		Size: 5.2 MB (5249966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5fe808e6f175a659981d31b9687526a651f4d40bce158c2baa204fcfcf2820`  
		Last Modified: Tue, 08 Aug 2023 00:45:39 GMT  
		Size: 1.2 MB (1185194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681275e7741131c55614b72469583c04861fb9344cde71f5dc2d00b75af4737b`  
		Last Modified: Tue, 08 Aug 2023 00:45:39 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:4c76dac9b235685647bce5e644408f9537fd2a98243936db0666252a4ec24739
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110727449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84fe6eea8994d5e82ec6e85ed4c441f0a89b9cb461829805dd3eeb9d892d49a9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:41 GMT
RUN apk add --no-cache ca-certificates
# Mon, 07 Aug 2023 20:19:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Aug 2023 20:21:06 GMT
ENV GOLANG_VERSION=1.20.7
# Mon, 07 Aug 2023 20:23:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 07 Aug 2023 20:23:05 GMT
ENV GOPATH=/go
# Mon, 07 Aug 2023 20:23:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Aug 2023 20:23:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 07 Aug 2023 20:23:06 GMT
WORKDIR /go
# Tue, 08 Aug 2023 05:25:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:41:51 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:41:52 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:41:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:41:52 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:41:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:41:54 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:41:54 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec90be18226e5c99d10161aed1a143f4134093c55b4d6979bbdbbe4b0683eb11`  
		Last Modified: Mon, 07 Aug 2023 20:30:59 GMT  
		Size: 285.1 KB (285089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c751f85e4ba6e9bbada0b11691d914b2ec2c689bb0dca6b9cbe994488d0e3e`  
		Last Modified: Mon, 07 Aug 2023 20:31:56 GMT  
		Size: 100.9 MB (100865267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2d202223222826c8580d85b8d7dd6baa8ed1cad84ba5cf47dab23eaeeae7e9`  
		Last Modified: Mon, 07 Aug 2023 20:31:43 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0359ada615d16e203e1d40a49b896060013c2952c2982ae73b141cc291305a4c`  
		Last Modified: Tue, 08 Aug 2023 05:25:47 GMT  
		Size: 5.1 MB (5099943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1039996d136f688a91d291dcf3dbb995607af1f245f1741d8ad0c5f73cec1b01`  
		Last Modified: Mon, 14 Aug 2023 17:42:27 GMT  
		Size: 1.3 MB (1262391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17e7bfc7e0d6b6a7f70b22841fe42427f0fb6372b17c71c8063c50d7c8e73c1`  
		Last Modified: Mon, 14 Aug 2023 17:42:27 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:e47c546e0564931b55495f764fdfb59d8d81d4e51ff9a221952688b1dcf6d462
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `caddy:2.7-builder-windowsservercore-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:a6ebd264677820f38a44fb346c24e5b3cc1406cf5f975a99a089e14f2cfeb623
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2132345169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec0a81535ff140c0b08b259f2eb43a2face74a8aaeed3cc1ac39ef9b4e90c3f6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:39:54 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:39:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:41:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:41:12 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:42:07 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:53:35 GMT
ENV GOLANG_VERSION=1.20.7
# Thu, 10 Aug 2023 00:56:38 GMT
RUN $url = 'https://dl.google.com/go/go1.20.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '736dc6c7fcab1c96b682c8c93e38d7e371e62a17d34cb2c37d451a1147f66af9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:56:40 GMT
WORKDIR C:\go
# Thu, 10 Aug 2023 03:04:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 03:04:56 GMT
ENV XCADDY_VERSION=v0.3.4
# Thu, 10 Aug 2023 03:04:57 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:04:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Aug 2023 03:06:01 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('542b4c083852d41081186c79757b66ff3c26248f72ed461dbc038b51687d0a8a8ce8eee69e3b5a1d43360c48b3405b611b940fa378debe98aaa0b3c5aebfa218')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 10 Aug 2023 03:06:02 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594083c5c2094c95b4e52723d54c14e0d70881f4f176720c3170012275accc3b`  
		Last Modified: Thu, 10 Aug 2023 01:02:54 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e2c2a5b75ced3a3a50be088c4a6c2d7df926b1fe6515b2d0c021312e3642f4`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d28688050deeec928289543beadf5c75bb2a8246576cb7c066e23818016217`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e5fbc50e7e0fefb7c9e349038ecb00ed5c000bcab8c4d82b1e1000c4273c01`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0544e07bd9df923e11e09c7dc042da614f2f14589eb6fa79005ebbbf2731e97d`  
		Last Modified: Thu, 10 Aug 2023 01:02:57 GMT  
		Size: 25.6 MB (25560980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555a82506c4fcec2bd90ae77756e5b03788e30c89f1a3820aa0b6a7ae6ad58ae`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bcfb422b104764156fc5ba099b5e3ae9fa9f760fd2db1c21acd8969b3d73de`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 220.8 KB (220796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c6aa0a5a1689ed800c4ef72c1b9febf207840fd2c6abfe4bb460e2e2bfb0b0`  
		Last Modified: Thu, 10 Aug 2023 01:05:03 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53d3379322a67b2413189cc2b779d22cb4093124343c8bb17fdf720b7b49fda`  
		Last Modified: Thu, 10 Aug 2023 01:05:25 GMT  
		Size: 108.9 MB (108911716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b60ccf92610ddbc47a05664785c95215a123e8930afbf6e3e2cefc80e693fd2`  
		Last Modified: Thu, 10 Aug 2023 01:05:04 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2c7d6253e62d61e5e0d2ad331a96cff5175f6c608b2ab4657825b3e3b4b4d0`  
		Last Modified: Thu, 10 Aug 2023 03:08:03 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c54227291fad3a25beb98d755de6f26fee6576e1b807e42c0bb70aa45793b3`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d107b434fabbe0d8d3916744b92501e6f5f8dabf7621ce44432d53d3853b4b8`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b0bcd286241a360f34f20c3842b90b6f53c31abe4d60fcb8f1148e8ba191a3`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5677a754ea49eeeb0b5ed56da2ac0d43c11e3c935c36adc2cc71b95dc7b99c0f`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.7 MB (1679125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4626f9b6f575add3a8f4ac9248f4342e9cb80f9abf696deff5a7bd9aff57fbf1`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:b21f945f75a0af5f372c03cead52a84f725ba635c6f414ff9bcdfd81c64008c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1906; amd64

### `caddy:2.7-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:44aba8da329d3ea3489327b5c94e41477f815f943659f4464a2c859ad400dcfd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1933815424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d095c2914283b4b75e4dbb95eb3e7f5ff6db80079dc6981bf1c5fa8355036c99`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:36:23 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:36:24 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:36:25 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:36:26 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:36:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:37:00 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:37:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:50:52 GMT
ENV GOLANG_VERSION=1.20.7
# Thu, 10 Aug 2023 00:53:17 GMT
RUN $url = 'https://dl.google.com/go/go1.20.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '736dc6c7fcab1c96b682c8c93e38d7e371e62a17d34cb2c37d451a1147f66af9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:53:18 GMT
WORKDIR C:\go
# Thu, 10 Aug 2023 03:06:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 03:06:10 GMT
ENV XCADDY_VERSION=v0.3.4
# Thu, 10 Aug 2023 03:06:11 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:06:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Aug 2023 03:06:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('542b4c083852d41081186c79757b66ff3c26248f72ed461dbc038b51687d0a8a8ce8eee69e3b5a1d43360c48b3405b611b940fa378debe98aaa0b3c5aebfa218')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 10 Aug 2023 03:06:35 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877256a6389e5e2563da79ad5bd201e7ee136abf14ff7cb0d4efbf3b24e5f127`  
		Last Modified: Thu, 10 Aug 2023 01:02:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a39df29b3c0b2f7e691c47273110db4a46e5c8e299f6bb95f77a9c61f79872`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8574d63bce1547e3177d0b76237a782a9b016d4880375dcd1a7b6a1c5dee3dc`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ef34b3c96316bcdd92e24c8c4eebdc3a35f245c013ef87edfae0dde091a305`  
		Last Modified: Thu, 10 Aug 2023 01:02:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a481babc5b629f694446a96dba8d77c020257c98334c605aff94162b9a917279`  
		Last Modified: Thu, 10 Aug 2023 01:02:23 GMT  
		Size: 25.6 MB (25554169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281178ea1c103ff07ea7e4fb647eb0dbe4f865742da6ef9944e04f37974fc27c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b5d34adf2aacfe87580143f3e17c635dc8dbd4068377b79b35d665f49bbad9`  
		Last Modified: Thu, 10 Aug 2023 01:02:16 GMT  
		Size: 275.9 KB (275946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02a2e79b5a05c2145c733eefb2add45d1ebefb7a16b93c321f5883c8ced6f1a`  
		Last Modified: Thu, 10 Aug 2023 01:04:30 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd9991b8cfbc481c153abf1625143209f4c4fd40d9443a5a19f4e3613336ad2`  
		Last Modified: Thu, 10 Aug 2023 01:04:53 GMT  
		Size: 108.9 MB (108927695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dc6778f41c3c7d50b8e71668e22880153d6c6794f24c4661fc3d6aa089d0a5`  
		Last Modified: Thu, 10 Aug 2023 01:04:30 GMT  
		Size: 1.5 KB (1547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c5985f015e143065716f5aabf0ecaed537103c5ec07e6c57360204a7787d02`  
		Last Modified: Thu, 10 Aug 2023 03:08:23 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd9cf527e30318df5bccd0be2c9a9716dc073b1f84c1d2c5cadc85adcf2af02`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604bc0fdaac29b943186656363f9267b86b2744da35d6b519a428d494d0a6bd3`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b527a45b48b4328e0ea94e3e2d3f239ed4f960d30ea0b9272cd902aec85c8b`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9ae10f93498ae3f8bbfef69dd561e41337584fb8dcc09fe82ed4971f9787be`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.7 MB (1675642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6218363385083ee3dbece9e5e2fd5c9086be201ca76bd6818b46bb6e591688eb`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-windowsservercore`

```console
$ docker pull caddy@sha256:ee77e6dfe66fce930f6e92b862071843a872dfc67ee4b8ad9c0e843a0c4103fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4737; amd64
	-	windows version 10.0.20348.1906; amd64

### `caddy:2.7-windowsservercore` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:1b4a86d284b971594d7e30ef09451be59ba84514b612c87b6406e2dfb8e9e23f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2011958834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ae5f48eae2f949ec09ad9f70ff2c2626318e07111bea5b6622116482ac991b0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 02:59:41 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Aug 2023 02:59:41 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:00:57 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('69d2d73c2514ab5ce4f6a60489c79ce4da0e1d4302c85ab584d0a7a7fd0d034bfe5a5caab78c96ac3383ddd7d2e12c3c41fb47c4716909d2a78d448b0289ccec')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Aug 2023 03:00:58 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Aug 2023 03:00:59 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Aug 2023 03:01:00 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Thu, 10 Aug 2023 03:01:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Aug 2023 03:01:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Aug 2023 03:01:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Aug 2023 03:01:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Aug 2023 03:01:03 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Aug 2023 03:01:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Aug 2023 03:01:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Aug 2023 03:01:06 GMT
EXPOSE 80
# Thu, 10 Aug 2023 03:01:06 GMT
EXPOSE 443
# Thu, 10 Aug 2023 03:01:07 GMT
EXPOSE 443/udp
# Thu, 10 Aug 2023 03:01:08 GMT
EXPOSE 2019
# Thu, 10 Aug 2023 03:03:10 GMT
RUN caddy version
# Thu, 10 Aug 2023 03:03:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907ddb8e2b3b8f440ec855971bf77d521900d3faecd1816d7146d89f1c78f408`  
		Last Modified: Thu, 10 Aug 2023 03:07:15 GMT  
		Size: 469.4 KB (469388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d430330f12b22fcc17a5d114d51ba3bb8e62a55f87b67f939d18651c226f927`  
		Last Modified: Thu, 10 Aug 2023 03:07:15 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd493f43c2fb25a7c8540ea353a098f784a6e8d5fe4e9d070e4a1de796cde96c`  
		Last Modified: Thu, 10 Aug 2023 03:07:18 GMT  
		Size: 15.2 MB (15241515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95b32f0fb8252db266318cca24c13f5eea8b8b3c19405b92f1a8b9199e39c5d`  
		Last Modified: Thu, 10 Aug 2023 03:07:14 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7dbc1767506f0f3f5b4d3a9671f97a723014ae1e38cf8056f6257db7917a88`  
		Last Modified: Thu, 10 Aug 2023 03:07:13 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7905b1f85b201367c5a62618ddc55da9a60cbb3da1da40ab60a88c125a5956`  
		Last Modified: Thu, 10 Aug 2023 03:07:13 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce34081b153cf49ce89b2ff4fc81f54a648cefc5d2dbb0f60048b94ba10f43b`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9622cc1048f5f7259d3263b67dd386c5d70ae4cf0a358c33deb3df8cdb316efd`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b1ca0970bf360a0627a1deae2985b658f54b41758f12f4e5448ed1aee3bc82`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503770a8fe554599aa8e6413082b7cb24d7f1faa328deaf28b34ddb2a294972b`  
		Last Modified: Thu, 10 Aug 2023 03:07:11 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea5eee99969c433a1c2f4d0f7fdc838185350144b9d3f20888c2a53cc6f3563`  
		Last Modified: Thu, 10 Aug 2023 03:07:11 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675093fb34c31fff953a92ee1831f09679783e7d3e1d9ff40a962f346d1dc581`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fd64685610dd5572f21efe3fae8cb13537c9deb6693caf4097bf9ec3b4dabe`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540e52aaf0b1acca0c4a9fbb2a60e5ce4bca2c119fbb3bbd86658186b23e3202`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29819bc504b56dacdb0df898ee58e26d8097802c0a5578cd14d4e3ed0655bde7`  
		Last Modified: Thu, 10 Aug 2023 03:07:09 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2157a412d53cd6d3174744de6c1cf5cb0dd03274fe9b36f749525867e4b9bd2`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cfbf0b65ccf78eb536c8a23f0b92fa148268c1fa4a39c1b19c7d9310e53b8d`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7faedca764204aa914e83a3721476c9a6a7f8177d057021e5a1debb81a436808`  
		Last Modified: Thu, 10 Aug 2023 03:07:09 GMT  
		Size: 268.6 KB (268640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86622825a44d72176deccdf0a5e4c9127ebf8f2591211cbdae585e9977363e8`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7-windowsservercore` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:144bc31c96841830b174ed1ff2da09ba18881208aae2efd16b3c850953f762f6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1813356270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02028c6ef8441cbf5181f34f78b4740b60dffff030772882302c9ca39f9a6096`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 03:03:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Aug 2023 03:03:52 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:04:21 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('69d2d73c2514ab5ce4f6a60489c79ce4da0e1d4302c85ab584d0a7a7fd0d034bfe5a5caab78c96ac3383ddd7d2e12c3c41fb47c4716909d2a78d448b0289ccec')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Aug 2023 03:04:21 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Aug 2023 03:04:22 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Aug 2023 03:04:23 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Thu, 10 Aug 2023 03:04:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Aug 2023 03:04:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Aug 2023 03:04:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Aug 2023 03:04:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Aug 2023 03:04:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Aug 2023 03:04:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Aug 2023 03:04:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Aug 2023 03:04:29 GMT
EXPOSE 80
# Thu, 10 Aug 2023 03:04:30 GMT
EXPOSE 443
# Thu, 10 Aug 2023 03:04:31 GMT
EXPOSE 443/udp
# Thu, 10 Aug 2023 03:04:32 GMT
EXPOSE 2019
# Thu, 10 Aug 2023 03:04:47 GMT
RUN caddy version
# Thu, 10 Aug 2023 03:04:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee168d3c6067847c3aef71a2a0dfdc70984b0bb6164086b49da7bd27de3ff3e4`  
		Last Modified: Thu, 10 Aug 2023 03:07:41 GMT  
		Size: 462.1 KB (462122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0efe6e8d5895981c45dc711aa05390379a6f7e5ceea618991435f40db1736c5`  
		Last Modified: Thu, 10 Aug 2023 03:07:40 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c66dfda490f2720f8d21e51546bae9f4e21a4b3b76b29f45e18435544c66a7c`  
		Last Modified: Thu, 10 Aug 2023 03:07:44 GMT  
		Size: 15.2 MB (15227189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67327c2fc33a0a30f2e409ada51c37d6663c07a498c7663987be61f888f7a8`  
		Last Modified: Thu, 10 Aug 2023 03:07:40 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c73910f4e5bd8630e3f4a5c23d004a9f6eff60c9f50af18e4b1d9b5f9ac0aa4`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d17a44e8dc24bdc71a9866c99b7022ca1a00e04acc6bf00dbf794c0550bb79d`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851a0578d2d21e2b22a64fe518454ef0283a718573db4e60e3b4a0121bd4081a`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ab80276792afc4370db678044627f33dabc32a9a987d736686239ed1d85a5b`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dcfba0d938817014a224fd3369379868ad4bd05a910cf582eb5e88ca8630ce`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd3ed16ce737bd3530ec90c77867e59892ce05deebca1a42256c570b86ddf1a`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb186d102ae807e026f9de311625fe281b24e140d91adaa2c46298a163035182`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267fad2b6b29094e45425d6b1d39b3f0a295ee7bbce5489aab9e77a659c7ef09`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608cb1e8b46f127167ebb53ec28593783baa810d0ec8e54a929e2907cea85352`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dadf995868b2bcb1e42a4b48f3df0ccd9a979672da04a75dad7970b567bb793`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4209fa97cbb4a651cae617cf81de393ea0652645a1f00b607c18dfa26834c475`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e65f2bc3967a653972ae76ef447ff72659e620a98280fe5230591a0e7c29cd`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9d8975e744e0f5b82190fc02ef017a7f4e7ffa1dda69f5be10f43ffa554d9e`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef526b9884253387824d19beee5d18eee6650c38429c56acd30286c1ea94da03`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 280.0 KB (280042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0266d9103b52d7b0129a0aa08ddab9c5bdfca0694ed3368c0b9c887941c524a`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-windowsservercore-1809`

```console
$ docker pull caddy@sha256:40d5f0aa53bb62f81ccb8625ca40ae2b0057b977b8432daa5d3a76079b9737e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `caddy:2.7-windowsservercore-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:1b4a86d284b971594d7e30ef09451be59ba84514b612c87b6406e2dfb8e9e23f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2011958834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ae5f48eae2f949ec09ad9f70ff2c2626318e07111bea5b6622116482ac991b0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 02:59:41 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Aug 2023 02:59:41 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:00:57 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('69d2d73c2514ab5ce4f6a60489c79ce4da0e1d4302c85ab584d0a7a7fd0d034bfe5a5caab78c96ac3383ddd7d2e12c3c41fb47c4716909d2a78d448b0289ccec')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Aug 2023 03:00:58 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Aug 2023 03:00:59 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Aug 2023 03:01:00 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Thu, 10 Aug 2023 03:01:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Aug 2023 03:01:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Aug 2023 03:01:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Aug 2023 03:01:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Aug 2023 03:01:03 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Aug 2023 03:01:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Aug 2023 03:01:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Aug 2023 03:01:06 GMT
EXPOSE 80
# Thu, 10 Aug 2023 03:01:06 GMT
EXPOSE 443
# Thu, 10 Aug 2023 03:01:07 GMT
EXPOSE 443/udp
# Thu, 10 Aug 2023 03:01:08 GMT
EXPOSE 2019
# Thu, 10 Aug 2023 03:03:10 GMT
RUN caddy version
# Thu, 10 Aug 2023 03:03:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907ddb8e2b3b8f440ec855971bf77d521900d3faecd1816d7146d89f1c78f408`  
		Last Modified: Thu, 10 Aug 2023 03:07:15 GMT  
		Size: 469.4 KB (469388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d430330f12b22fcc17a5d114d51ba3bb8e62a55f87b67f939d18651c226f927`  
		Last Modified: Thu, 10 Aug 2023 03:07:15 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd493f43c2fb25a7c8540ea353a098f784a6e8d5fe4e9d070e4a1de796cde96c`  
		Last Modified: Thu, 10 Aug 2023 03:07:18 GMT  
		Size: 15.2 MB (15241515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95b32f0fb8252db266318cca24c13f5eea8b8b3c19405b92f1a8b9199e39c5d`  
		Last Modified: Thu, 10 Aug 2023 03:07:14 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7dbc1767506f0f3f5b4d3a9671f97a723014ae1e38cf8056f6257db7917a88`  
		Last Modified: Thu, 10 Aug 2023 03:07:13 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7905b1f85b201367c5a62618ddc55da9a60cbb3da1da40ab60a88c125a5956`  
		Last Modified: Thu, 10 Aug 2023 03:07:13 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce34081b153cf49ce89b2ff4fc81f54a648cefc5d2dbb0f60048b94ba10f43b`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9622cc1048f5f7259d3263b67dd386c5d70ae4cf0a358c33deb3df8cdb316efd`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b1ca0970bf360a0627a1deae2985b658f54b41758f12f4e5448ed1aee3bc82`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503770a8fe554599aa8e6413082b7cb24d7f1faa328deaf28b34ddb2a294972b`  
		Last Modified: Thu, 10 Aug 2023 03:07:11 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea5eee99969c433a1c2f4d0f7fdc838185350144b9d3f20888c2a53cc6f3563`  
		Last Modified: Thu, 10 Aug 2023 03:07:11 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675093fb34c31fff953a92ee1831f09679783e7d3e1d9ff40a962f346d1dc581`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fd64685610dd5572f21efe3fae8cb13537c9deb6693caf4097bf9ec3b4dabe`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540e52aaf0b1acca0c4a9fbb2a60e5ce4bca2c119fbb3bbd86658186b23e3202`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29819bc504b56dacdb0df898ee58e26d8097802c0a5578cd14d4e3ed0655bde7`  
		Last Modified: Thu, 10 Aug 2023 03:07:09 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2157a412d53cd6d3174744de6c1cf5cb0dd03274fe9b36f749525867e4b9bd2`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cfbf0b65ccf78eb536c8a23f0b92fa148268c1fa4a39c1b19c7d9310e53b8d`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7faedca764204aa914e83a3721476c9a6a7f8177d057021e5a1debb81a436808`  
		Last Modified: Thu, 10 Aug 2023 03:07:09 GMT  
		Size: 268.6 KB (268640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86622825a44d72176deccdf0a5e4c9127ebf8f2591211cbdae585e9977363e8`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:32d0082c4ae3fdb4c834f812d8c65442f02e9ea2e037e23a5fa80b0399bbf314
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1906; amd64

### `caddy:2.7-windowsservercore-ltsc2022` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:144bc31c96841830b174ed1ff2da09ba18881208aae2efd16b3c850953f762f6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1813356270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02028c6ef8441cbf5181f34f78b4740b60dffff030772882302c9ca39f9a6096`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 03:03:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Aug 2023 03:03:52 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:04:21 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('69d2d73c2514ab5ce4f6a60489c79ce4da0e1d4302c85ab584d0a7a7fd0d034bfe5a5caab78c96ac3383ddd7d2e12c3c41fb47c4716909d2a78d448b0289ccec')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Aug 2023 03:04:21 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Aug 2023 03:04:22 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Aug 2023 03:04:23 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Thu, 10 Aug 2023 03:04:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Aug 2023 03:04:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Aug 2023 03:04:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Aug 2023 03:04:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Aug 2023 03:04:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Aug 2023 03:04:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Aug 2023 03:04:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Aug 2023 03:04:29 GMT
EXPOSE 80
# Thu, 10 Aug 2023 03:04:30 GMT
EXPOSE 443
# Thu, 10 Aug 2023 03:04:31 GMT
EXPOSE 443/udp
# Thu, 10 Aug 2023 03:04:32 GMT
EXPOSE 2019
# Thu, 10 Aug 2023 03:04:47 GMT
RUN caddy version
# Thu, 10 Aug 2023 03:04:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee168d3c6067847c3aef71a2a0dfdc70984b0bb6164086b49da7bd27de3ff3e4`  
		Last Modified: Thu, 10 Aug 2023 03:07:41 GMT  
		Size: 462.1 KB (462122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0efe6e8d5895981c45dc711aa05390379a6f7e5ceea618991435f40db1736c5`  
		Last Modified: Thu, 10 Aug 2023 03:07:40 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c66dfda490f2720f8d21e51546bae9f4e21a4b3b76b29f45e18435544c66a7c`  
		Last Modified: Thu, 10 Aug 2023 03:07:44 GMT  
		Size: 15.2 MB (15227189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67327c2fc33a0a30f2e409ada51c37d6663c07a498c7663987be61f888f7a8`  
		Last Modified: Thu, 10 Aug 2023 03:07:40 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c73910f4e5bd8630e3f4a5c23d004a9f6eff60c9f50af18e4b1d9b5f9ac0aa4`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d17a44e8dc24bdc71a9866c99b7022ca1a00e04acc6bf00dbf794c0550bb79d`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851a0578d2d21e2b22a64fe518454ef0283a718573db4e60e3b4a0121bd4081a`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ab80276792afc4370db678044627f33dabc32a9a987d736686239ed1d85a5b`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dcfba0d938817014a224fd3369379868ad4bd05a910cf582eb5e88ca8630ce`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd3ed16ce737bd3530ec90c77867e59892ce05deebca1a42256c570b86ddf1a`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb186d102ae807e026f9de311625fe281b24e140d91adaa2c46298a163035182`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267fad2b6b29094e45425d6b1d39b3f0a295ee7bbce5489aab9e77a659c7ef09`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608cb1e8b46f127167ebb53ec28593783baa810d0ec8e54a929e2907cea85352`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dadf995868b2bcb1e42a4b48f3df0ccd9a979672da04a75dad7970b567bb793`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4209fa97cbb4a651cae617cf81de393ea0652645a1f00b607c18dfa26834c475`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e65f2bc3967a653972ae76ef447ff72659e620a98280fe5230591a0e7c29cd`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9d8975e744e0f5b82190fc02ef017a7f4e7ffa1dda69f5be10f43ffa554d9e`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef526b9884253387824d19beee5d18eee6650c38429c56acd30286c1ea94da03`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 280.0 KB (280042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0266d9103b52d7b0129a0aa08ddab9c5bdfca0694ed3368c0b9c887941c524a`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.3`

```console
$ docker pull caddy@sha256:a289cd8272ae7d9785e30057e369986136ea804ddb193a9f5445ddb867f850ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; s390x

### `caddy:2.7.3` - linux; arm variant v6

```console
$ docker pull caddy@sha256:dc698bd1b82521df87ea42fbf48c98d10133ec962497ac80527b65769ceb6a9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17690701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3775ac20cca67f4d547f26f5984a989b9407b0c4129fd6cd86dbb3359249acd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:38:27 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:49:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:49:14 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:49:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:49:16 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:49:16 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:49:18 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:49:18 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:49:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172ef460a93549b8a3e73f6a515bccad93512788d1e8f095e7230ba41967c25a`  
		Last Modified: Wed, 09 Aug 2023 03:38:53 GMT  
		Size: 347.7 KB (347686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7aae78767a581df85fd1a51ccd646619aec320896ca016ef0f05a41b16bcbfe`  
		Last Modified: Mon, 14 Aug 2023 17:49:36 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5244db1c019e66038874df2b8b92c74437f6d355802bfccada90c9d8bd8d29`  
		Last Modified: Mon, 14 Aug 2023 17:49:38 GMT  
		Size: 14.2 MB (14190701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.3` - linux; arm variant v7

```console
$ docker pull caddy@sha256:e9cb1245e1c134e25a0ec0803e5132ba9ba92d0a4ad85db3f73bd2c3188cf70e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17414619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df6e2a1f4c707dc77276814a27ac22a7b5de268780603d8e08324130e1fc563`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:51:41 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:57:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:57:17 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:57:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:57:20 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:57:20 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:57:21 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:57:21 GMT
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
	-	`sha256:46e1b3e18d5e992f1805072b2d52405d575830bdce21726ef99dea99e31d8277`  
		Last Modified: Mon, 14 Aug 2023 17:57:42 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2b7485982d191f9dc0498d5b940d14df575f36ca66876b92d3ca09ff9386b2`  
		Last Modified: Mon, 14 Aug 2023 17:57:48 GMT  
		Size: 14.2 MB (14163172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.3` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:db04154ce5f7a7f4d058567375880cdc6b1a3675095ad576f9886f39f1374afc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17329640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:731c0ae21a974e5708c4a8006250893bca5a2ecad43babf2a0a95a60fc61d6cd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:09:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:39:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:39:19 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:39:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:39:21 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:39:21 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:39:22 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:39:22 GMT
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
	-	`sha256:f7488af8b96c79b6db13955a0302653c4e9f314d0833201984ae06c1ed697f06`  
		Last Modified: Mon, 14 Aug 2023 17:39:41 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9600da6e7e51b9083b29f3c7de592fa45e7765ca5ffe8d2abf7cc99c50578fe`  
		Last Modified: Mon, 14 Aug 2023 17:39:43 GMT  
		Size: 13.6 MB (13630728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.3` - linux; s390x

```console
$ docker pull caddy@sha256:3b3d4b80e160105a760ad62b32c497245d69676e6053c2a7b61bc5c6fc178fd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.0 MB (17984968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a63d05bc7601e47460ff86bc91380fd9407c0b4886b80836ac3aadb436f68e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:14:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:41:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:41:39 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:41:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:41:43 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:41:43 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:41:44 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:41:44 GMT
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
	-	`sha256:308478977890baa82477ee70a3065fb9da2080efcc95facf1a87ac021b06a8e9`  
		Last Modified: Mon, 14 Aug 2023 17:42:17 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fe1cbba37a3c1c2f6ba50e59e5c238c8d83ffca820ef709108b9e3253af757`  
		Last Modified: Mon, 14 Aug 2023 17:42:19 GMT  
		Size: 14.4 MB (14408320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.3-alpine`

```console
$ docker pull caddy@sha256:a289cd8272ae7d9785e30057e369986136ea804ddb193a9f5445ddb867f850ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; s390x

### `caddy:2.7.3-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:dc698bd1b82521df87ea42fbf48c98d10133ec962497ac80527b65769ceb6a9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17690701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3775ac20cca67f4d547f26f5984a989b9407b0c4129fd6cd86dbb3359249acd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:38:27 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:49:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:49:14 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:49:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:49:16 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:49:16 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:49:18 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:49:18 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:49:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172ef460a93549b8a3e73f6a515bccad93512788d1e8f095e7230ba41967c25a`  
		Last Modified: Wed, 09 Aug 2023 03:38:53 GMT  
		Size: 347.7 KB (347686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7aae78767a581df85fd1a51ccd646619aec320896ca016ef0f05a41b16bcbfe`  
		Last Modified: Mon, 14 Aug 2023 17:49:36 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5244db1c019e66038874df2b8b92c74437f6d355802bfccada90c9d8bd8d29`  
		Last Modified: Mon, 14 Aug 2023 17:49:38 GMT  
		Size: 14.2 MB (14190701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.3-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:e9cb1245e1c134e25a0ec0803e5132ba9ba92d0a4ad85db3f73bd2c3188cf70e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17414619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df6e2a1f4c707dc77276814a27ac22a7b5de268780603d8e08324130e1fc563`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:51:41 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:57:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:57:17 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:57:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:57:20 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:57:20 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:57:21 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:57:21 GMT
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
	-	`sha256:46e1b3e18d5e992f1805072b2d52405d575830bdce21726ef99dea99e31d8277`  
		Last Modified: Mon, 14 Aug 2023 17:57:42 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2b7485982d191f9dc0498d5b940d14df575f36ca66876b92d3ca09ff9386b2`  
		Last Modified: Mon, 14 Aug 2023 17:57:48 GMT  
		Size: 14.2 MB (14163172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.3-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:db04154ce5f7a7f4d058567375880cdc6b1a3675095ad576f9886f39f1374afc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17329640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:731c0ae21a974e5708c4a8006250893bca5a2ecad43babf2a0a95a60fc61d6cd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:09:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:39:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:39:19 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:39:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:39:21 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:39:21 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:39:22 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:39:22 GMT
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
	-	`sha256:f7488af8b96c79b6db13955a0302653c4e9f314d0833201984ae06c1ed697f06`  
		Last Modified: Mon, 14 Aug 2023 17:39:41 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9600da6e7e51b9083b29f3c7de592fa45e7765ca5ffe8d2abf7cc99c50578fe`  
		Last Modified: Mon, 14 Aug 2023 17:39:43 GMT  
		Size: 13.6 MB (13630728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.3-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:3b3d4b80e160105a760ad62b32c497245d69676e6053c2a7b61bc5c6fc178fd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.0 MB (17984968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a63d05bc7601e47460ff86bc91380fd9407c0b4886b80836ac3aadb436f68e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:14:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:41:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:41:39 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:41:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:41:43 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:41:43 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:41:44 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:41:44 GMT
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
	-	`sha256:308478977890baa82477ee70a3065fb9da2080efcc95facf1a87ac021b06a8e9`  
		Last Modified: Mon, 14 Aug 2023 17:42:17 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fe1cbba37a3c1c2f6ba50e59e5c238c8d83ffca820ef709108b9e3253af757`  
		Last Modified: Mon, 14 Aug 2023 17:42:19 GMT  
		Size: 14.4 MB (14408320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.3-builder`

```console
$ docker pull caddy@sha256:04b95e5e28e3ef875ec9b650d19f8ec81f92949c4b3dece2a75fcfb1b3c69473
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; s390x

### `caddy:2.7.3-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:289b1f78db36a7524bbae6562b80b29fe5585984effd44a3e22146fcbf4ab824
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108301221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98ac734398939dbe1f4c664f493d34b5353c438189c6b58b3e6e4d92186a8f80`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:12:05 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:12:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:12:40 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 23:14:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 23:14:36 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 23:14:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:14:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 23:14:37 GMT
WORKDIR /go
# Wed, 09 Aug 2023 03:38:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:49:20 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:49:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:49:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:49:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8564ce36feee688566265012773f1c8c7c046ceefe86ca763eb702682f4e6e75`  
		Last Modified: Tue, 08 Aug 2023 23:15:06 GMT  
		Size: 284.9 KB (284876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b139603b026cc15bf570c9cf012fc165cb74821883c7c7c534fe6ed189b5a2`  
		Last Modified: Tue, 08 Aug 2023 23:16:29 GMT  
		Size: 98.7 MB (98671161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b2f37c2778ffd2e158ad31438d6802c214dfa5d79e06dc9af2d8320828e148`  
		Last Modified: Tue, 08 Aug 2023 23:16:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f22c305527b162efa854ac3e1963e59e7fb8f2c71838222c56462b9809481ed`  
		Last Modified: Wed, 09 Aug 2023 03:39:10 GMT  
		Size: 5.0 MB (4951147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5520daf22ad222fbe3c81bbd6afa0c912b3817f0f432a35a939f9870a8512af`  
		Last Modified: Mon, 14 Aug 2023 17:49:51 GMT  
		Size: 1.2 MB (1248666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f8fe3942ebea0d37a8324080324eb0bca35e859273e7bac44381e31a0fa714`  
		Last Modified: Mon, 14 Aug 2023 17:49:51 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.3-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:dcbac62a4e9d8d10345a7f20ac37a814b45633ed4b050a14fa20aef08590597a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107386270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0adee903aaec70e29acbd506823b19cc477dc7788e545d1b88316b9ec0e9c154`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:39:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 01:39:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 01:40:29 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 01:42:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 01:42:12 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 01:42:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 01:42:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 01:42:13 GMT
WORKDIR /go
# Tue, 08 Aug 2023 01:51:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:57:24 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:57:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:57:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:57:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47bd95d78f565e902bafd0264a979eb4f6f71e22c0464011bf9db6feb0579e6`  
		Last Modified: Tue, 08 Aug 2023 01:48:34 GMT  
		Size: 284.1 KB (284073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a674106498848b269b5cb69fb938d3dc97247d02cb1aa3927b7a7469724e950`  
		Last Modified: Tue, 08 Aug 2023 01:49:43 GMT  
		Size: 98.5 MB (98454659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1902a68db0b07b05ab7d2f3e48ca8f1d22951b498f6ff9027bdc91a5e7e830`  
		Last Modified: Tue, 08 Aug 2023 01:49:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9caf1886c556e441f6f89cd1cb00e1b950d9d8fcad8812a988fbb59caf0b0ba5`  
		Last Modified: Tue, 08 Aug 2023 01:52:22 GMT  
		Size: 4.5 MB (4501403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c28b1afe92de619aa5de35a2f610dc68af6b39c6cd300ef8426738a739366a2`  
		Last Modified: Mon, 14 Aug 2023 17:58:00 GMT  
		Size: 1.2 MB (1246092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6fe75fd67d7668d6aeca167419514f45cb72ec61bd61a9fc32e25b5c928dba6`  
		Last Modified: Mon, 14 Aug 2023 17:58:00 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.3-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:9ad7390f7aa878bd4d6750dab9611c7397630fc15a7f80304eea3d3f64dcfe4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.0 MB (105987240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c79cdcd45a4a61e8fe257b7917335ede1523a72d1c2ef2eb9115783a5379f5ea`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:10:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:10:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:10:53 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 23:11:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 23:11:59 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 23:11:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:12:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 23:12:00 GMT
WORKDIR /go
# Wed, 09 Aug 2023 10:10:28 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:39:25 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:39:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:39:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:39:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54e960e981301b0098c80d2e61d694333b5ab480a007a3a8d0fa629662d377`  
		Last Modified: Tue, 08 Aug 2023 23:14:21 GMT  
		Size: 286.3 KB (286298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20ccffba14f84f51f896ae916a3dd045a0b0d08dc27d53f7d6a9dc5687c3501`  
		Last Modified: Tue, 08 Aug 2023 23:15:23 GMT  
		Size: 96.1 MB (96117263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d452dd4d3acc29d43b0be67bcc0c121814601787c7fd45e8260687d2cc8983`  
		Last Modified: Tue, 08 Aug 2023 23:15:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d371a704ab9a071c89db966e268fe56aad2288363a849d10eb032d47cd10848b`  
		Last Modified: Wed, 09 Aug 2023 10:10:48 GMT  
		Size: 5.1 MB (5053901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5e38cf28101c20845f7f103114793f73691285da6ac006db5cb28c20bc8000`  
		Last Modified: Mon, 14 Aug 2023 17:39:55 GMT  
		Size: 1.2 MB (1198449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d1b8334b836b303a87ddda4bfba4af764950afa40c2c263cca11ed8b53a8c6`  
		Last Modified: Mon, 14 Aug 2023 17:39:54 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.3-builder` - linux; s390x

```console
$ docker pull caddy@sha256:4c76dac9b235685647bce5e644408f9537fd2a98243936db0666252a4ec24739
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110727449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84fe6eea8994d5e82ec6e85ed4c441f0a89b9cb461829805dd3eeb9d892d49a9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:41 GMT
RUN apk add --no-cache ca-certificates
# Mon, 07 Aug 2023 20:19:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Aug 2023 20:21:06 GMT
ENV GOLANG_VERSION=1.20.7
# Mon, 07 Aug 2023 20:23:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 07 Aug 2023 20:23:05 GMT
ENV GOPATH=/go
# Mon, 07 Aug 2023 20:23:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Aug 2023 20:23:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 07 Aug 2023 20:23:06 GMT
WORKDIR /go
# Tue, 08 Aug 2023 05:25:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:41:51 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:41:52 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:41:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:41:52 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:41:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:41:54 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:41:54 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec90be18226e5c99d10161aed1a143f4134093c55b4d6979bbdbbe4b0683eb11`  
		Last Modified: Mon, 07 Aug 2023 20:30:59 GMT  
		Size: 285.1 KB (285089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c751f85e4ba6e9bbada0b11691d914b2ec2c689bb0dca6b9cbe994488d0e3e`  
		Last Modified: Mon, 07 Aug 2023 20:31:56 GMT  
		Size: 100.9 MB (100865267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2d202223222826c8580d85b8d7dd6baa8ed1cad84ba5cf47dab23eaeeae7e9`  
		Last Modified: Mon, 07 Aug 2023 20:31:43 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0359ada615d16e203e1d40a49b896060013c2952c2982ae73b141cc291305a4c`  
		Last Modified: Tue, 08 Aug 2023 05:25:47 GMT  
		Size: 5.1 MB (5099943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1039996d136f688a91d291dcf3dbb995607af1f245f1741d8ad0c5f73cec1b01`  
		Last Modified: Mon, 14 Aug 2023 17:42:27 GMT  
		Size: 1.3 MB (1262391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17e7bfc7e0d6b6a7f70b22841fe42427f0fb6372b17c71c8063c50d7c8e73c1`  
		Last Modified: Mon, 14 Aug 2023 17:42:27 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.3-builder-alpine`

```console
$ docker pull caddy@sha256:04b95e5e28e3ef875ec9b650d19f8ec81f92949c4b3dece2a75fcfb1b3c69473
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; s390x

### `caddy:2.7.3-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:289b1f78db36a7524bbae6562b80b29fe5585984effd44a3e22146fcbf4ab824
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108301221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98ac734398939dbe1f4c664f493d34b5353c438189c6b58b3e6e4d92186a8f80`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:12:05 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:12:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:12:40 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 23:14:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 23:14:36 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 23:14:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:14:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 23:14:37 GMT
WORKDIR /go
# Wed, 09 Aug 2023 03:38:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:49:20 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:49:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:49:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:49:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8564ce36feee688566265012773f1c8c7c046ceefe86ca763eb702682f4e6e75`  
		Last Modified: Tue, 08 Aug 2023 23:15:06 GMT  
		Size: 284.9 KB (284876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b139603b026cc15bf570c9cf012fc165cb74821883c7c7c534fe6ed189b5a2`  
		Last Modified: Tue, 08 Aug 2023 23:16:29 GMT  
		Size: 98.7 MB (98671161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b2f37c2778ffd2e158ad31438d6802c214dfa5d79e06dc9af2d8320828e148`  
		Last Modified: Tue, 08 Aug 2023 23:16:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f22c305527b162efa854ac3e1963e59e7fb8f2c71838222c56462b9809481ed`  
		Last Modified: Wed, 09 Aug 2023 03:39:10 GMT  
		Size: 5.0 MB (4951147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5520daf22ad222fbe3c81bbd6afa0c912b3817f0f432a35a939f9870a8512af`  
		Last Modified: Mon, 14 Aug 2023 17:49:51 GMT  
		Size: 1.2 MB (1248666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f8fe3942ebea0d37a8324080324eb0bca35e859273e7bac44381e31a0fa714`  
		Last Modified: Mon, 14 Aug 2023 17:49:51 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.3-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:dcbac62a4e9d8d10345a7f20ac37a814b45633ed4b050a14fa20aef08590597a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107386270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0adee903aaec70e29acbd506823b19cc477dc7788e545d1b88316b9ec0e9c154`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:39:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 01:39:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 01:40:29 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 01:42:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 01:42:12 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 01:42:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 01:42:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 01:42:13 GMT
WORKDIR /go
# Tue, 08 Aug 2023 01:51:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:57:24 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:57:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:57:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:57:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47bd95d78f565e902bafd0264a979eb4f6f71e22c0464011bf9db6feb0579e6`  
		Last Modified: Tue, 08 Aug 2023 01:48:34 GMT  
		Size: 284.1 KB (284073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a674106498848b269b5cb69fb938d3dc97247d02cb1aa3927b7a7469724e950`  
		Last Modified: Tue, 08 Aug 2023 01:49:43 GMT  
		Size: 98.5 MB (98454659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1902a68db0b07b05ab7d2f3e48ca8f1d22951b498f6ff9027bdc91a5e7e830`  
		Last Modified: Tue, 08 Aug 2023 01:49:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9caf1886c556e441f6f89cd1cb00e1b950d9d8fcad8812a988fbb59caf0b0ba5`  
		Last Modified: Tue, 08 Aug 2023 01:52:22 GMT  
		Size: 4.5 MB (4501403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c28b1afe92de619aa5de35a2f610dc68af6b39c6cd300ef8426738a739366a2`  
		Last Modified: Mon, 14 Aug 2023 17:58:00 GMT  
		Size: 1.2 MB (1246092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6fe75fd67d7668d6aeca167419514f45cb72ec61bd61a9fc32e25b5c928dba6`  
		Last Modified: Mon, 14 Aug 2023 17:58:00 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.3-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:9ad7390f7aa878bd4d6750dab9611c7397630fc15a7f80304eea3d3f64dcfe4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.0 MB (105987240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c79cdcd45a4a61e8fe257b7917335ede1523a72d1c2ef2eb9115783a5379f5ea`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:10:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:10:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:10:53 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 23:11:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 23:11:59 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 23:11:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:12:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 23:12:00 GMT
WORKDIR /go
# Wed, 09 Aug 2023 10:10:28 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:39:25 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:39:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:39:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:39:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54e960e981301b0098c80d2e61d694333b5ab480a007a3a8d0fa629662d377`  
		Last Modified: Tue, 08 Aug 2023 23:14:21 GMT  
		Size: 286.3 KB (286298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20ccffba14f84f51f896ae916a3dd045a0b0d08dc27d53f7d6a9dc5687c3501`  
		Last Modified: Tue, 08 Aug 2023 23:15:23 GMT  
		Size: 96.1 MB (96117263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d452dd4d3acc29d43b0be67bcc0c121814601787c7fd45e8260687d2cc8983`  
		Last Modified: Tue, 08 Aug 2023 23:15:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d371a704ab9a071c89db966e268fe56aad2288363a849d10eb032d47cd10848b`  
		Last Modified: Wed, 09 Aug 2023 10:10:48 GMT  
		Size: 5.1 MB (5053901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5e38cf28101c20845f7f103114793f73691285da6ac006db5cb28c20bc8000`  
		Last Modified: Mon, 14 Aug 2023 17:39:55 GMT  
		Size: 1.2 MB (1198449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d1b8334b836b303a87ddda4bfba4af764950afa40c2c263cca11ed8b53a8c6`  
		Last Modified: Mon, 14 Aug 2023 17:39:54 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.7.3-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:4c76dac9b235685647bce5e644408f9537fd2a98243936db0666252a4ec24739
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110727449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84fe6eea8994d5e82ec6e85ed4c441f0a89b9cb461829805dd3eeb9d892d49a9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:41 GMT
RUN apk add --no-cache ca-certificates
# Mon, 07 Aug 2023 20:19:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Aug 2023 20:21:06 GMT
ENV GOLANG_VERSION=1.20.7
# Mon, 07 Aug 2023 20:23:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 07 Aug 2023 20:23:05 GMT
ENV GOPATH=/go
# Mon, 07 Aug 2023 20:23:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Aug 2023 20:23:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 07 Aug 2023 20:23:06 GMT
WORKDIR /go
# Tue, 08 Aug 2023 05:25:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:41:51 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:41:52 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:41:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:41:52 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:41:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:41:54 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:41:54 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec90be18226e5c99d10161aed1a143f4134093c55b4d6979bbdbbe4b0683eb11`  
		Last Modified: Mon, 07 Aug 2023 20:30:59 GMT  
		Size: 285.1 KB (285089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c751f85e4ba6e9bbada0b11691d914b2ec2c689bb0dca6b9cbe994488d0e3e`  
		Last Modified: Mon, 07 Aug 2023 20:31:56 GMT  
		Size: 100.9 MB (100865267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2d202223222826c8580d85b8d7dd6baa8ed1cad84ba5cf47dab23eaeeae7e9`  
		Last Modified: Mon, 07 Aug 2023 20:31:43 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0359ada615d16e203e1d40a49b896060013c2952c2982ae73b141cc291305a4c`  
		Last Modified: Tue, 08 Aug 2023 05:25:47 GMT  
		Size: 5.1 MB (5099943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1039996d136f688a91d291dcf3dbb995607af1f245f1741d8ad0c5f73cec1b01`  
		Last Modified: Mon, 14 Aug 2023 17:42:27 GMT  
		Size: 1.3 MB (1262391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17e7bfc7e0d6b6a7f70b22841fe42427f0fb6372b17c71c8063c50d7c8e73c1`  
		Last Modified: Mon, 14 Aug 2023 17:42:27 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.7.3-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `caddy:2.7.3-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `caddy:2.7.3-windowsservercore`

```console
$ docker pull caddy@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `caddy:2.7.3-windowsservercore-1809`

```console
$ docker pull caddy@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `caddy:2.7.3-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `caddy:alpine`

```console
$ docker pull caddy@sha256:00e7c43c571e7036a06830652d919a83c140041d6f98f0ee30c2764f01b8fd6d
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

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:dc698bd1b82521df87ea42fbf48c98d10133ec962497ac80527b65769ceb6a9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17690701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3775ac20cca67f4d547f26f5984a989b9407b0c4129fd6cd86dbb3359249acd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:38:27 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:49:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:49:14 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:49:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:49:16 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:49:16 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:49:18 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:49:18 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:49:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172ef460a93549b8a3e73f6a515bccad93512788d1e8f095e7230ba41967c25a`  
		Last Modified: Wed, 09 Aug 2023 03:38:53 GMT  
		Size: 347.7 KB (347686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7aae78767a581df85fd1a51ccd646619aec320896ca016ef0f05a41b16bcbfe`  
		Last Modified: Mon, 14 Aug 2023 17:49:36 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5244db1c019e66038874df2b8b92c74437f6d355802bfccada90c9d8bd8d29`  
		Last Modified: Mon, 14 Aug 2023 17:49:38 GMT  
		Size: 14.2 MB (14190701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:e9cb1245e1c134e25a0ec0803e5132ba9ba92d0a4ad85db3f73bd2c3188cf70e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17414619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df6e2a1f4c707dc77276814a27ac22a7b5de268780603d8e08324130e1fc563`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:51:41 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:57:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:57:17 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:57:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:57:20 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:57:20 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:57:21 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:57:21 GMT
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
	-	`sha256:46e1b3e18d5e992f1805072b2d52405d575830bdce21726ef99dea99e31d8277`  
		Last Modified: Mon, 14 Aug 2023 17:57:42 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2b7485982d191f9dc0498d5b940d14df575f36ca66876b92d3ca09ff9386b2`  
		Last Modified: Mon, 14 Aug 2023 17:57:48 GMT  
		Size: 14.2 MB (14163172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:db04154ce5f7a7f4d058567375880cdc6b1a3675095ad576f9886f39f1374afc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17329640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:731c0ae21a974e5708c4a8006250893bca5a2ecad43babf2a0a95a60fc61d6cd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:09:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:39:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:39:19 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:39:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:39:21 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:39:21 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:39:22 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:39:22 GMT
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
	-	`sha256:f7488af8b96c79b6db13955a0302653c4e9f314d0833201984ae06c1ed697f06`  
		Last Modified: Mon, 14 Aug 2023 17:39:41 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9600da6e7e51b9083b29f3c7de592fa45e7765ca5ffe8d2abf7cc99c50578fe`  
		Last Modified: Mon, 14 Aug 2023 17:39:43 GMT  
		Size: 13.6 MB (13630728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

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

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:3b3d4b80e160105a760ad62b32c497245d69676e6053c2a7b61bc5c6fc178fd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.0 MB (17984968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a63d05bc7601e47460ff86bc91380fd9407c0b4886b80836ac3aadb436f68e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:14:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:41:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:41:39 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:41:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:41:43 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:41:43 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:41:44 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:41:44 GMT
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
	-	`sha256:308478977890baa82477ee70a3065fb9da2080efcc95facf1a87ac021b06a8e9`  
		Last Modified: Mon, 14 Aug 2023 17:42:17 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fe1cbba37a3c1c2f6ba50e59e5c238c8d83ffca820ef709108b9e3253af757`  
		Last Modified: Mon, 14 Aug 2023 17:42:19 GMT  
		Size: 14.4 MB (14408320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:b93978cf962da183e6d11a754d51de5f033da2708c588c9ba27cd0ce2c3b582c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4737; amd64
	-	windows version 10.0.20348.1906; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:7abb7723020bab7b367d33786efcfca5d4a4f884ec306308d4a5513f14cdc20c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110901544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e24e6bda832eff522a3ea76a20f3e8055f2ecefa2f16c9f5485ad066bebf9a14`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:36:47 GMT
RUN apk add --no-cache ca-certificates
# Wed, 09 Aug 2023 04:41:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Aug 2023 04:41:57 GMT
ENV GOLANG_VERSION=1.20.7
# Wed, 09 Aug 2023 04:43:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 09 Aug 2023 04:43:29 GMT
ENV GOPATH=/go
# Wed, 09 Aug 2023 04:43:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Aug 2023 04:43:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 09 Aug 2023 04:43:30 GMT
WORKDIR /go
# Wed, 09 Aug 2023 10:26:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 09 Aug 2023 10:26:17 GMT
ENV XCADDY_VERSION=v0.3.4
# Wed, 09 Aug 2023 10:26:17 GMT
ENV CADDY_VERSION=v2.7.2
# Wed, 09 Aug 2023 10:26:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Aug 2023 10:26:17 GMT
ENV XCADDY_SETCAP=1
# Wed, 09 Aug 2023 10:26:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68ab15d90eb70c23e8b13c3935b194fc1b638f8c0fee6506a109dcee082c20d6e07890320a876b13eb23b5a7a0617daa28fe8af24dcb0dcb3eca9ea74dc76713' ;; 		armhf)   binArch='armv6'; checksum='2853413e63ac29f296b1c44696022febc8b29c4b37fb20442b635903a0b79d523ca00896dfce3e40f5894dd297b345ac007af0ddffccaada843c7de61d334134' ;; 		armv7)   binArch='armv7'; checksum='c59e93ba270705b2312f6a70552f2a345cec91cc3504233785cb46fa4b644a47e520bb29dfbf519f814bb13d0bbea213976fd7b059883eab2b091913f9ed393f' ;; 		aarch64) binArch='arm64'; checksum='df4c58e97931ca58b7a38d245948912b817e952a2961ff583744039ca68a584a303f7cbfdb33392c84d8f76f5b30f206d9f84a04f547043a3d1fa5282b0fd544' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2795d5b7546bd10ff3cd21a393597281e42e1043164536e01e18fb56047ba5b396493a086bb2d90e8ede9a54b5208e947ecaacccca4a8550704fb3f8a17dd771' ;; 		s390x)   binArch='s390x'; checksum='2ed85231aac36e3af873e3fdf4f6b6378b55dcc17743d24b28b3b48d6622fde73aae58eed124082478a0b841c338d64caa0b0be302545a79092a97cf205f1b29' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 09 Aug 2023 10:26:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 09 Aug 2023 10:26:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d48a809fc2256f8aa0aeee47998488d64409855adba00a7cb3007ab9f3286e`  
		Last Modified: Wed, 09 Aug 2023 03:37:02 GMT  
		Size: 284.7 KB (284693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e790db5857269a95a948a96f0e3304c851351e588262d58504700b2e73fb7fe`  
		Last Modified: Wed, 09 Aug 2023 04:47:32 GMT  
		Size: 101.0 MB (100954810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727f4e1a48a681e22437b6c14b04a4e287386f50f1be21ef490a1e28fd276a91`  
		Last Modified: Wed, 09 Aug 2023 04:47:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a272b880a0f8927853947bb9b16e005e2824b1685a89cc015f4e4694c441ed0e`  
		Last Modified: Wed, 09 Aug 2023 10:26:35 GMT  
		Size: 5.0 MB (4958652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e328d3f19ca0bf59908eb26cf5d7b5f94d2aa3e53eb5426f11ddaceca7d024`  
		Last Modified: Wed, 09 Aug 2023 10:26:35 GMT  
		Size: 1.3 MB (1301217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3115a3b8c7625246591f7ffa414a109f6c26f09066d0a9b9c0aba053e2a13c02`  
		Last Modified: Wed, 09 Aug 2023 10:26:35 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:289b1f78db36a7524bbae6562b80b29fe5585984effd44a3e22146fcbf4ab824
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108301221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98ac734398939dbe1f4c664f493d34b5353c438189c6b58b3e6e4d92186a8f80`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:12:05 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:12:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:12:40 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 23:14:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 23:14:36 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 23:14:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:14:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 23:14:37 GMT
WORKDIR /go
# Wed, 09 Aug 2023 03:38:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:49:20 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:49:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:49:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:49:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8564ce36feee688566265012773f1c8c7c046ceefe86ca763eb702682f4e6e75`  
		Last Modified: Tue, 08 Aug 2023 23:15:06 GMT  
		Size: 284.9 KB (284876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b139603b026cc15bf570c9cf012fc165cb74821883c7c7c534fe6ed189b5a2`  
		Last Modified: Tue, 08 Aug 2023 23:16:29 GMT  
		Size: 98.7 MB (98671161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b2f37c2778ffd2e158ad31438d6802c214dfa5d79e06dc9af2d8320828e148`  
		Last Modified: Tue, 08 Aug 2023 23:16:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f22c305527b162efa854ac3e1963e59e7fb8f2c71838222c56462b9809481ed`  
		Last Modified: Wed, 09 Aug 2023 03:39:10 GMT  
		Size: 5.0 MB (4951147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5520daf22ad222fbe3c81bbd6afa0c912b3817f0f432a35a939f9870a8512af`  
		Last Modified: Mon, 14 Aug 2023 17:49:51 GMT  
		Size: 1.2 MB (1248666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f8fe3942ebea0d37a8324080324eb0bca35e859273e7bac44381e31a0fa714`  
		Last Modified: Mon, 14 Aug 2023 17:49:51 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:dcbac62a4e9d8d10345a7f20ac37a814b45633ed4b050a14fa20aef08590597a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107386270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0adee903aaec70e29acbd506823b19cc477dc7788e545d1b88316b9ec0e9c154`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:39:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 01:39:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 01:40:29 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 01:42:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 01:42:12 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 01:42:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 01:42:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 01:42:13 GMT
WORKDIR /go
# Tue, 08 Aug 2023 01:51:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:57:24 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:57:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:57:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:57:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47bd95d78f565e902bafd0264a979eb4f6f71e22c0464011bf9db6feb0579e6`  
		Last Modified: Tue, 08 Aug 2023 01:48:34 GMT  
		Size: 284.1 KB (284073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a674106498848b269b5cb69fb938d3dc97247d02cb1aa3927b7a7469724e950`  
		Last Modified: Tue, 08 Aug 2023 01:49:43 GMT  
		Size: 98.5 MB (98454659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1902a68db0b07b05ab7d2f3e48ca8f1d22951b498f6ff9027bdc91a5e7e830`  
		Last Modified: Tue, 08 Aug 2023 01:49:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9caf1886c556e441f6f89cd1cb00e1b950d9d8fcad8812a988fbb59caf0b0ba5`  
		Last Modified: Tue, 08 Aug 2023 01:52:22 GMT  
		Size: 4.5 MB (4501403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c28b1afe92de619aa5de35a2f610dc68af6b39c6cd300ef8426738a739366a2`  
		Last Modified: Mon, 14 Aug 2023 17:58:00 GMT  
		Size: 1.2 MB (1246092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6fe75fd67d7668d6aeca167419514f45cb72ec61bd61a9fc32e25b5c928dba6`  
		Last Modified: Mon, 14 Aug 2023 17:58:00 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:9ad7390f7aa878bd4d6750dab9611c7397630fc15a7f80304eea3d3f64dcfe4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.0 MB (105987240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c79cdcd45a4a61e8fe257b7917335ede1523a72d1c2ef2eb9115783a5379f5ea`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:10:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:10:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:10:53 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 23:11:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 23:11:59 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 23:11:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:12:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 23:12:00 GMT
WORKDIR /go
# Wed, 09 Aug 2023 10:10:28 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:39:25 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:39:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:39:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:39:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54e960e981301b0098c80d2e61d694333b5ab480a007a3a8d0fa629662d377`  
		Last Modified: Tue, 08 Aug 2023 23:14:21 GMT  
		Size: 286.3 KB (286298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20ccffba14f84f51f896ae916a3dd045a0b0d08dc27d53f7d6a9dc5687c3501`  
		Last Modified: Tue, 08 Aug 2023 23:15:23 GMT  
		Size: 96.1 MB (96117263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d452dd4d3acc29d43b0be67bcc0c121814601787c7fd45e8260687d2cc8983`  
		Last Modified: Tue, 08 Aug 2023 23:15:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d371a704ab9a071c89db966e268fe56aad2288363a849d10eb032d47cd10848b`  
		Last Modified: Wed, 09 Aug 2023 10:10:48 GMT  
		Size: 5.1 MB (5053901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5e38cf28101c20845f7f103114793f73691285da6ac006db5cb28c20bc8000`  
		Last Modified: Mon, 14 Aug 2023 17:39:55 GMT  
		Size: 1.2 MB (1198449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d1b8334b836b303a87ddda4bfba4af764950afa40c2c263cca11ed8b53a8c6`  
		Last Modified: Mon, 14 Aug 2023 17:39:54 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:e3543706f8faff15a067252f4e5760bb4cb3e12ff81b7a932052bc013ecc4151
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106660406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37b7339021535bddbd7f4a89deae282741ae3163c68d69d7d5d035167f7d440`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:25:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 00:25:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 00:26:56 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 00:29:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 00:29:34 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 00:29:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 00:29:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 00:29:36 GMT
WORKDIR /go
# Tue, 08 Aug 2023 00:44:40 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 08 Aug 2023 00:44:41 GMT
ENV XCADDY_VERSION=v0.3.4
# Tue, 08 Aug 2023 00:44:42 GMT
ENV CADDY_VERSION=v2.7.2
# Tue, 08 Aug 2023 00:44:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 08 Aug 2023 00:44:43 GMT
ENV XCADDY_SETCAP=1
# Tue, 08 Aug 2023 00:44:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68ab15d90eb70c23e8b13c3935b194fc1b638f8c0fee6506a109dcee082c20d6e07890320a876b13eb23b5a7a0617daa28fe8af24dcb0dcb3eca9ea74dc76713' ;; 		armhf)   binArch='armv6'; checksum='2853413e63ac29f296b1c44696022febc8b29c4b37fb20442b635903a0b79d523ca00896dfce3e40f5894dd297b345ac007af0ddffccaada843c7de61d334134' ;; 		armv7)   binArch='armv7'; checksum='c59e93ba270705b2312f6a70552f2a345cec91cc3504233785cb46fa4b644a47e520bb29dfbf519f814bb13d0bbea213976fd7b059883eab2b091913f9ed393f' ;; 		aarch64) binArch='arm64'; checksum='df4c58e97931ca58b7a38d245948912b817e952a2961ff583744039ca68a584a303f7cbfdb33392c84d8f76f5b30f206d9f84a04f547043a3d1fa5282b0fd544' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2795d5b7546bd10ff3cd21a393597281e42e1043164536e01e18fb56047ba5b396493a086bb2d90e8ede9a54b5208e947ecaacccca4a8550704fb3f8a17dd771' ;; 		s390x)   binArch='s390x'; checksum='2ed85231aac36e3af873e3fdf4f6b6378b55dcc17743d24b28b3b48d6622fde73aae58eed124082478a0b841c338d64caa0b0be302545a79092a97cf205f1b29' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 08 Aug 2023 00:44:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 08 Aug 2023 00:44:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c966ad2cdd35689da92e7c8fd39bd37cd6080c484e6ccaf00672c154cd4f6c2a`  
		Last Modified: Tue, 08 Aug 2023 00:39:35 GMT  
		Size: 286.7 KB (286662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7816c9df7e6881fdd62dfcc6d743edcc2c3ca9220542437a2e5fdcfa0e4548`  
		Last Modified: Tue, 08 Aug 2023 00:41:09 GMT  
		Size: 96.6 MB (96591770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d34a514a03c5af8a03dfe8c4fbfd50b2ec61591d24080f8be8bf722904f541`  
		Last Modified: Tue, 08 Aug 2023 00:40:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802af1410e20c34900a811878ca2fa2e5dc79daeb92a53b94588831011ad81fc`  
		Last Modified: Tue, 08 Aug 2023 00:45:40 GMT  
		Size: 5.2 MB (5249966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5fe808e6f175a659981d31b9687526a651f4d40bce158c2baa204fcfcf2820`  
		Last Modified: Tue, 08 Aug 2023 00:45:39 GMT  
		Size: 1.2 MB (1185194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681275e7741131c55614b72469583c04861fb9344cde71f5dc2d00b75af4737b`  
		Last Modified: Tue, 08 Aug 2023 00:45:39 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:4c76dac9b235685647bce5e644408f9537fd2a98243936db0666252a4ec24739
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110727449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84fe6eea8994d5e82ec6e85ed4c441f0a89b9cb461829805dd3eeb9d892d49a9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:41 GMT
RUN apk add --no-cache ca-certificates
# Mon, 07 Aug 2023 20:19:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Aug 2023 20:21:06 GMT
ENV GOLANG_VERSION=1.20.7
# Mon, 07 Aug 2023 20:23:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 07 Aug 2023 20:23:05 GMT
ENV GOPATH=/go
# Mon, 07 Aug 2023 20:23:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Aug 2023 20:23:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 07 Aug 2023 20:23:06 GMT
WORKDIR /go
# Tue, 08 Aug 2023 05:25:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:41:51 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:41:52 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:41:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:41:52 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:41:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:41:54 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:41:54 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec90be18226e5c99d10161aed1a143f4134093c55b4d6979bbdbbe4b0683eb11`  
		Last Modified: Mon, 07 Aug 2023 20:30:59 GMT  
		Size: 285.1 KB (285089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c751f85e4ba6e9bbada0b11691d914b2ec2c689bb0dca6b9cbe994488d0e3e`  
		Last Modified: Mon, 07 Aug 2023 20:31:56 GMT  
		Size: 100.9 MB (100865267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2d202223222826c8580d85b8d7dd6baa8ed1cad84ba5cf47dab23eaeeae7e9`  
		Last Modified: Mon, 07 Aug 2023 20:31:43 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0359ada615d16e203e1d40a49b896060013c2952c2982ae73b141cc291305a4c`  
		Last Modified: Tue, 08 Aug 2023 05:25:47 GMT  
		Size: 5.1 MB (5099943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1039996d136f688a91d291dcf3dbb995607af1f245f1741d8ad0c5f73cec1b01`  
		Last Modified: Mon, 14 Aug 2023 17:42:27 GMT  
		Size: 1.3 MB (1262391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17e7bfc7e0d6b6a7f70b22841fe42427f0fb6372b17c71c8063c50d7c8e73c1`  
		Last Modified: Mon, 14 Aug 2023 17:42:27 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:a6ebd264677820f38a44fb346c24e5b3cc1406cf5f975a99a089e14f2cfeb623
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2132345169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec0a81535ff140c0b08b259f2eb43a2face74a8aaeed3cc1ac39ef9b4e90c3f6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:39:54 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:39:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:41:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:41:12 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:42:07 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:53:35 GMT
ENV GOLANG_VERSION=1.20.7
# Thu, 10 Aug 2023 00:56:38 GMT
RUN $url = 'https://dl.google.com/go/go1.20.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '736dc6c7fcab1c96b682c8c93e38d7e371e62a17d34cb2c37d451a1147f66af9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:56:40 GMT
WORKDIR C:\go
# Thu, 10 Aug 2023 03:04:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 03:04:56 GMT
ENV XCADDY_VERSION=v0.3.4
# Thu, 10 Aug 2023 03:04:57 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:04:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Aug 2023 03:06:01 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('542b4c083852d41081186c79757b66ff3c26248f72ed461dbc038b51687d0a8a8ce8eee69e3b5a1d43360c48b3405b611b940fa378debe98aaa0b3c5aebfa218')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 10 Aug 2023 03:06:02 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594083c5c2094c95b4e52723d54c14e0d70881f4f176720c3170012275accc3b`  
		Last Modified: Thu, 10 Aug 2023 01:02:54 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e2c2a5b75ced3a3a50be088c4a6c2d7df926b1fe6515b2d0c021312e3642f4`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d28688050deeec928289543beadf5c75bb2a8246576cb7c066e23818016217`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e5fbc50e7e0fefb7c9e349038ecb00ed5c000bcab8c4d82b1e1000c4273c01`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0544e07bd9df923e11e09c7dc042da614f2f14589eb6fa79005ebbbf2731e97d`  
		Last Modified: Thu, 10 Aug 2023 01:02:57 GMT  
		Size: 25.6 MB (25560980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555a82506c4fcec2bd90ae77756e5b03788e30c89f1a3820aa0b6a7ae6ad58ae`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bcfb422b104764156fc5ba099b5e3ae9fa9f760fd2db1c21acd8969b3d73de`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 220.8 KB (220796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c6aa0a5a1689ed800c4ef72c1b9febf207840fd2c6abfe4bb460e2e2bfb0b0`  
		Last Modified: Thu, 10 Aug 2023 01:05:03 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53d3379322a67b2413189cc2b779d22cb4093124343c8bb17fdf720b7b49fda`  
		Last Modified: Thu, 10 Aug 2023 01:05:25 GMT  
		Size: 108.9 MB (108911716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b60ccf92610ddbc47a05664785c95215a123e8930afbf6e3e2cefc80e693fd2`  
		Last Modified: Thu, 10 Aug 2023 01:05:04 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2c7d6253e62d61e5e0d2ad331a96cff5175f6c608b2ab4657825b3e3b4b4d0`  
		Last Modified: Thu, 10 Aug 2023 03:08:03 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c54227291fad3a25beb98d755de6f26fee6576e1b807e42c0bb70aa45793b3`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d107b434fabbe0d8d3916744b92501e6f5f8dabf7621ce44432d53d3853b4b8`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b0bcd286241a360f34f20c3842b90b6f53c31abe4d60fcb8f1148e8ba191a3`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5677a754ea49eeeb0b5ed56da2ac0d43c11e3c935c36adc2cc71b95dc7b99c0f`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.7 MB (1679125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4626f9b6f575add3a8f4ac9248f4342e9cb80f9abf696deff5a7bd9aff57fbf1`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:44aba8da329d3ea3489327b5c94e41477f815f943659f4464a2c859ad400dcfd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1933815424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d095c2914283b4b75e4dbb95eb3e7f5ff6db80079dc6981bf1c5fa8355036c99`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:36:23 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:36:24 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:36:25 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:36:26 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:36:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:37:00 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:37:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:50:52 GMT
ENV GOLANG_VERSION=1.20.7
# Thu, 10 Aug 2023 00:53:17 GMT
RUN $url = 'https://dl.google.com/go/go1.20.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '736dc6c7fcab1c96b682c8c93e38d7e371e62a17d34cb2c37d451a1147f66af9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:53:18 GMT
WORKDIR C:\go
# Thu, 10 Aug 2023 03:06:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 03:06:10 GMT
ENV XCADDY_VERSION=v0.3.4
# Thu, 10 Aug 2023 03:06:11 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:06:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Aug 2023 03:06:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('542b4c083852d41081186c79757b66ff3c26248f72ed461dbc038b51687d0a8a8ce8eee69e3b5a1d43360c48b3405b611b940fa378debe98aaa0b3c5aebfa218')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 10 Aug 2023 03:06:35 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877256a6389e5e2563da79ad5bd201e7ee136abf14ff7cb0d4efbf3b24e5f127`  
		Last Modified: Thu, 10 Aug 2023 01:02:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a39df29b3c0b2f7e691c47273110db4a46e5c8e299f6bb95f77a9c61f79872`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8574d63bce1547e3177d0b76237a782a9b016d4880375dcd1a7b6a1c5dee3dc`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ef34b3c96316bcdd92e24c8c4eebdc3a35f245c013ef87edfae0dde091a305`  
		Last Modified: Thu, 10 Aug 2023 01:02:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a481babc5b629f694446a96dba8d77c020257c98334c605aff94162b9a917279`  
		Last Modified: Thu, 10 Aug 2023 01:02:23 GMT  
		Size: 25.6 MB (25554169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281178ea1c103ff07ea7e4fb647eb0dbe4f865742da6ef9944e04f37974fc27c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b5d34adf2aacfe87580143f3e17c635dc8dbd4068377b79b35d665f49bbad9`  
		Last Modified: Thu, 10 Aug 2023 01:02:16 GMT  
		Size: 275.9 KB (275946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02a2e79b5a05c2145c733eefb2add45d1ebefb7a16b93c321f5883c8ced6f1a`  
		Last Modified: Thu, 10 Aug 2023 01:04:30 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd9991b8cfbc481c153abf1625143209f4c4fd40d9443a5a19f4e3613336ad2`  
		Last Modified: Thu, 10 Aug 2023 01:04:53 GMT  
		Size: 108.9 MB (108927695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dc6778f41c3c7d50b8e71668e22880153d6c6794f24c4661fc3d6aa089d0a5`  
		Last Modified: Thu, 10 Aug 2023 01:04:30 GMT  
		Size: 1.5 KB (1547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c5985f015e143065716f5aabf0ecaed537103c5ec07e6c57360204a7787d02`  
		Last Modified: Thu, 10 Aug 2023 03:08:23 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd9cf527e30318df5bccd0be2c9a9716dc073b1f84c1d2c5cadc85adcf2af02`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604bc0fdaac29b943186656363f9267b86b2744da35d6b519a428d494d0a6bd3`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b527a45b48b4328e0ea94e3e2d3f239ed4f960d30ea0b9272cd902aec85c8b`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9ae10f93498ae3f8bbfef69dd561e41337584fb8dcc09fe82ed4971f9787be`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.7 MB (1675642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6218363385083ee3dbece9e5e2fd5c9086be201ca76bd6818b46bb6e591688eb`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:f921c48f48fcc6d6b234fd185f35b3762f339365402630553bfcca85a8376dbb
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
$ docker pull caddy@sha256:7abb7723020bab7b367d33786efcfca5d4a4f884ec306308d4a5513f14cdc20c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110901544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e24e6bda832eff522a3ea76a20f3e8055f2ecefa2f16c9f5485ad066bebf9a14`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:36:47 GMT
RUN apk add --no-cache ca-certificates
# Wed, 09 Aug 2023 04:41:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Aug 2023 04:41:57 GMT
ENV GOLANG_VERSION=1.20.7
# Wed, 09 Aug 2023 04:43:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 09 Aug 2023 04:43:29 GMT
ENV GOPATH=/go
# Wed, 09 Aug 2023 04:43:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Aug 2023 04:43:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 09 Aug 2023 04:43:30 GMT
WORKDIR /go
# Wed, 09 Aug 2023 10:26:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Wed, 09 Aug 2023 10:26:17 GMT
ENV XCADDY_VERSION=v0.3.4
# Wed, 09 Aug 2023 10:26:17 GMT
ENV CADDY_VERSION=v2.7.2
# Wed, 09 Aug 2023 10:26:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 09 Aug 2023 10:26:17 GMT
ENV XCADDY_SETCAP=1
# Wed, 09 Aug 2023 10:26:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68ab15d90eb70c23e8b13c3935b194fc1b638f8c0fee6506a109dcee082c20d6e07890320a876b13eb23b5a7a0617daa28fe8af24dcb0dcb3eca9ea74dc76713' ;; 		armhf)   binArch='armv6'; checksum='2853413e63ac29f296b1c44696022febc8b29c4b37fb20442b635903a0b79d523ca00896dfce3e40f5894dd297b345ac007af0ddffccaada843c7de61d334134' ;; 		armv7)   binArch='armv7'; checksum='c59e93ba270705b2312f6a70552f2a345cec91cc3504233785cb46fa4b644a47e520bb29dfbf519f814bb13d0bbea213976fd7b059883eab2b091913f9ed393f' ;; 		aarch64) binArch='arm64'; checksum='df4c58e97931ca58b7a38d245948912b817e952a2961ff583744039ca68a584a303f7cbfdb33392c84d8f76f5b30f206d9f84a04f547043a3d1fa5282b0fd544' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2795d5b7546bd10ff3cd21a393597281e42e1043164536e01e18fb56047ba5b396493a086bb2d90e8ede9a54b5208e947ecaacccca4a8550704fb3f8a17dd771' ;; 		s390x)   binArch='s390x'; checksum='2ed85231aac36e3af873e3fdf4f6b6378b55dcc17743d24b28b3b48d6622fde73aae58eed124082478a0b841c338d64caa0b0be302545a79092a97cf205f1b29' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 09 Aug 2023 10:26:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 09 Aug 2023 10:26:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d48a809fc2256f8aa0aeee47998488d64409855adba00a7cb3007ab9f3286e`  
		Last Modified: Wed, 09 Aug 2023 03:37:02 GMT  
		Size: 284.7 KB (284693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e790db5857269a95a948a96f0e3304c851351e588262d58504700b2e73fb7fe`  
		Last Modified: Wed, 09 Aug 2023 04:47:32 GMT  
		Size: 101.0 MB (100954810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727f4e1a48a681e22437b6c14b04a4e287386f50f1be21ef490a1e28fd276a91`  
		Last Modified: Wed, 09 Aug 2023 04:47:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a272b880a0f8927853947bb9b16e005e2824b1685a89cc015f4e4694c441ed0e`  
		Last Modified: Wed, 09 Aug 2023 10:26:35 GMT  
		Size: 5.0 MB (4958652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e328d3f19ca0bf59908eb26cf5d7b5f94d2aa3e53eb5426f11ddaceca7d024`  
		Last Modified: Wed, 09 Aug 2023 10:26:35 GMT  
		Size: 1.3 MB (1301217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3115a3b8c7625246591f7ffa414a109f6c26f09066d0a9b9c0aba053e2a13c02`  
		Last Modified: Wed, 09 Aug 2023 10:26:35 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:289b1f78db36a7524bbae6562b80b29fe5585984effd44a3e22146fcbf4ab824
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108301221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98ac734398939dbe1f4c664f493d34b5353c438189c6b58b3e6e4d92186a8f80`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:12:05 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:12:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:12:40 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 23:14:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 23:14:36 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 23:14:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:14:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 23:14:37 GMT
WORKDIR /go
# Wed, 09 Aug 2023 03:38:36 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:49:20 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:49:20 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:49:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:49:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:49:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8564ce36feee688566265012773f1c8c7c046ceefe86ca763eb702682f4e6e75`  
		Last Modified: Tue, 08 Aug 2023 23:15:06 GMT  
		Size: 284.9 KB (284876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b139603b026cc15bf570c9cf012fc165cb74821883c7c7c534fe6ed189b5a2`  
		Last Modified: Tue, 08 Aug 2023 23:16:29 GMT  
		Size: 98.7 MB (98671161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b2f37c2778ffd2e158ad31438d6802c214dfa5d79e06dc9af2d8320828e148`  
		Last Modified: Tue, 08 Aug 2023 23:16:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f22c305527b162efa854ac3e1963e59e7fb8f2c71838222c56462b9809481ed`  
		Last Modified: Wed, 09 Aug 2023 03:39:10 GMT  
		Size: 5.0 MB (4951147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5520daf22ad222fbe3c81bbd6afa0c912b3817f0f432a35a939f9870a8512af`  
		Last Modified: Mon, 14 Aug 2023 17:49:51 GMT  
		Size: 1.2 MB (1248666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f8fe3942ebea0d37a8324080324eb0bca35e859273e7bac44381e31a0fa714`  
		Last Modified: Mon, 14 Aug 2023 17:49:51 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:dcbac62a4e9d8d10345a7f20ac37a814b45633ed4b050a14fa20aef08590597a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107386270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0adee903aaec70e29acbd506823b19cc477dc7788e545d1b88316b9ec0e9c154`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:39:47 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 01:39:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 01:40:29 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 01:42:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 01:42:12 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 01:42:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 01:42:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 01:42:13 GMT
WORKDIR /go
# Tue, 08 Aug 2023 01:51:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:57:24 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:57:24 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:57:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:57:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:57:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47bd95d78f565e902bafd0264a979eb4f6f71e22c0464011bf9db6feb0579e6`  
		Last Modified: Tue, 08 Aug 2023 01:48:34 GMT  
		Size: 284.1 KB (284073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a674106498848b269b5cb69fb938d3dc97247d02cb1aa3927b7a7469724e950`  
		Last Modified: Tue, 08 Aug 2023 01:49:43 GMT  
		Size: 98.5 MB (98454659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1902a68db0b07b05ab7d2f3e48ca8f1d22951b498f6ff9027bdc91a5e7e830`  
		Last Modified: Tue, 08 Aug 2023 01:49:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9caf1886c556e441f6f89cd1cb00e1b950d9d8fcad8812a988fbb59caf0b0ba5`  
		Last Modified: Tue, 08 Aug 2023 01:52:22 GMT  
		Size: 4.5 MB (4501403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c28b1afe92de619aa5de35a2f610dc68af6b39c6cd300ef8426738a739366a2`  
		Last Modified: Mon, 14 Aug 2023 17:58:00 GMT  
		Size: 1.2 MB (1246092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6fe75fd67d7668d6aeca167419514f45cb72ec61bd61a9fc32e25b5c928dba6`  
		Last Modified: Mon, 14 Aug 2023 17:58:00 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:9ad7390f7aa878bd4d6750dab9611c7397630fc15a7f80304eea3d3f64dcfe4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.0 MB (105987240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c79cdcd45a4a61e8fe257b7917335ede1523a72d1c2ef2eb9115783a5379f5ea`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:10:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 23:10:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:10:53 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 23:11:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 23:11:59 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 23:11:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 23:12:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 23:12:00 GMT
WORKDIR /go
# Wed, 09 Aug 2023 10:10:28 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:39:25 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:39:25 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:39:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:39:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:39:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54e960e981301b0098c80d2e61d694333b5ab480a007a3a8d0fa629662d377`  
		Last Modified: Tue, 08 Aug 2023 23:14:21 GMT  
		Size: 286.3 KB (286298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20ccffba14f84f51f896ae916a3dd045a0b0d08dc27d53f7d6a9dc5687c3501`  
		Last Modified: Tue, 08 Aug 2023 23:15:23 GMT  
		Size: 96.1 MB (96117263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d452dd4d3acc29d43b0be67bcc0c121814601787c7fd45e8260687d2cc8983`  
		Last Modified: Tue, 08 Aug 2023 23:15:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d371a704ab9a071c89db966e268fe56aad2288363a849d10eb032d47cd10848b`  
		Last Modified: Wed, 09 Aug 2023 10:10:48 GMT  
		Size: 5.1 MB (5053901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5e38cf28101c20845f7f103114793f73691285da6ac006db5cb28c20bc8000`  
		Last Modified: Mon, 14 Aug 2023 17:39:55 GMT  
		Size: 1.2 MB (1198449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d1b8334b836b303a87ddda4bfba4af764950afa40c2c263cca11ed8b53a8c6`  
		Last Modified: Mon, 14 Aug 2023 17:39:54 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:e3543706f8faff15a067252f4e5760bb4cb3e12ff81b7a932052bc013ecc4151
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106660406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37b7339021535bddbd7f4a89deae282741ae3163c68d69d7d5d035167f7d440`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:25:24 GMT
RUN apk add --no-cache ca-certificates
# Tue, 08 Aug 2023 00:25:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 00:26:56 GMT
ENV GOLANG_VERSION=1.20.7
# Tue, 08 Aug 2023 00:29:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 08 Aug 2023 00:29:34 GMT
ENV GOPATH=/go
# Tue, 08 Aug 2023 00:29:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 00:29:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 08 Aug 2023 00:29:36 GMT
WORKDIR /go
# Tue, 08 Aug 2023 00:44:40 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 08 Aug 2023 00:44:41 GMT
ENV XCADDY_VERSION=v0.3.4
# Tue, 08 Aug 2023 00:44:42 GMT
ENV CADDY_VERSION=v2.7.2
# Tue, 08 Aug 2023 00:44:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 08 Aug 2023 00:44:43 GMT
ENV XCADDY_SETCAP=1
# Tue, 08 Aug 2023 00:44:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68ab15d90eb70c23e8b13c3935b194fc1b638f8c0fee6506a109dcee082c20d6e07890320a876b13eb23b5a7a0617daa28fe8af24dcb0dcb3eca9ea74dc76713' ;; 		armhf)   binArch='armv6'; checksum='2853413e63ac29f296b1c44696022febc8b29c4b37fb20442b635903a0b79d523ca00896dfce3e40f5894dd297b345ac007af0ddffccaada843c7de61d334134' ;; 		armv7)   binArch='armv7'; checksum='c59e93ba270705b2312f6a70552f2a345cec91cc3504233785cb46fa4b644a47e520bb29dfbf519f814bb13d0bbea213976fd7b059883eab2b091913f9ed393f' ;; 		aarch64) binArch='arm64'; checksum='df4c58e97931ca58b7a38d245948912b817e952a2961ff583744039ca68a584a303f7cbfdb33392c84d8f76f5b30f206d9f84a04f547043a3d1fa5282b0fd544' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='2795d5b7546bd10ff3cd21a393597281e42e1043164536e01e18fb56047ba5b396493a086bb2d90e8ede9a54b5208e947ecaacccca4a8550704fb3f8a17dd771' ;; 		s390x)   binArch='s390x'; checksum='2ed85231aac36e3af873e3fdf4f6b6378b55dcc17743d24b28b3b48d6622fde73aae58eed124082478a0b841c338d64caa0b0be302545a79092a97cf205f1b29' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 08 Aug 2023 00:44:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 08 Aug 2023 00:44:49 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c966ad2cdd35689da92e7c8fd39bd37cd6080c484e6ccaf00672c154cd4f6c2a`  
		Last Modified: Tue, 08 Aug 2023 00:39:35 GMT  
		Size: 286.7 KB (286662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7816c9df7e6881fdd62dfcc6d743edcc2c3ca9220542437a2e5fdcfa0e4548`  
		Last Modified: Tue, 08 Aug 2023 00:41:09 GMT  
		Size: 96.6 MB (96591770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d34a514a03c5af8a03dfe8c4fbfd50b2ec61591d24080f8be8bf722904f541`  
		Last Modified: Tue, 08 Aug 2023 00:40:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802af1410e20c34900a811878ca2fa2e5dc79daeb92a53b94588831011ad81fc`  
		Last Modified: Tue, 08 Aug 2023 00:45:40 GMT  
		Size: 5.2 MB (5249966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5fe808e6f175a659981d31b9687526a651f4d40bce158c2baa204fcfcf2820`  
		Last Modified: Tue, 08 Aug 2023 00:45:39 GMT  
		Size: 1.2 MB (1185194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681275e7741131c55614b72469583c04861fb9344cde71f5dc2d00b75af4737b`  
		Last Modified: Tue, 08 Aug 2023 00:45:39 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:4c76dac9b235685647bce5e644408f9537fd2a98243936db0666252a4ec24739
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110727449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84fe6eea8994d5e82ec6e85ed4c441f0a89b9cb461829805dd3eeb9d892d49a9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:19:41 GMT
RUN apk add --no-cache ca-certificates
# Mon, 07 Aug 2023 20:19:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Aug 2023 20:21:06 GMT
ENV GOLANG_VERSION=1.20.7
# Mon, 07 Aug 2023 20:23:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		'riscv64') 			export GOARCH='riscv64' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.20.7.src.tar.gz'; 		sha256='2c5ee9c9ec1e733b0dbbc2bdfed3f62306e51d8172bf38f4f4e542b27520f597'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 07 Aug 2023 20:23:05 GMT
ENV GOPATH=/go
# Mon, 07 Aug 2023 20:23:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Aug 2023 20:23:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 07 Aug 2023 20:23:06 GMT
WORKDIR /go
# Tue, 08 Aug 2023 05:25:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Mon, 14 Aug 2023 17:41:51 GMT
ENV XCADDY_VERSION=v0.3.5
# Mon, 14 Aug 2023 17:41:52 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:41:52 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 14 Aug 2023 17:41:52 GMT
ENV XCADDY_SETCAP=1
# Mon, 14 Aug 2023 17:41:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='9e87261a4ca4144bf25105e0cb3b3eb0fb0b8564fe4fa5c126e25a926baea2d16868cb4e88cafc419dc69db3e692894bc7ebcb25434c0bbb74362c2f3a696db5' ;; 		armhf)   binArch='armv6'; checksum='e327445263f3c4ceacae92f88417ef9d2f559bd01ea53230c38529295f2c29da45a0f9c436a71dafc85009a4ead7acdde832971479fccde7839228f0fc2153f1' ;; 		armv7)   binArch='armv7'; checksum='c46e12f1750ea1c99a80cf0ab2115541957f2791257176df2dbf2b25869c552b3108ff7c9d6854081dcf843548e6ec3b1e5451944bd7b6b9527dfe63f849f01b' ;; 		aarch64) binArch='arm64'; checksum='a4b1caf438326e0dcb58830701993d514b11fd86b4880c9c013c230031dfa68efa339be186662f586ce848d5a2841a2e6513f41ada9a05c04a297433df3f2a52' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b9c79ec1ddd1f7606d7f1263cf4ebad8c03154e78e301db27cb1554723b1f12ae886dd4be682a9decd3dbc189d6e90c51879ae160696db00e0d32dced2df8991' ;; 		s390x)   binArch='s390x'; checksum='658f3d85e751e3e43906e55b9f915c35c1e87c6cdeb606263147804520fe4cf3afdf295882c7bab2e9c932a7c12d1759275fa1c0b611d5b770c940e9ec13ec43' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.5/xcaddy_0.3.5_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 14 Aug 2023 17:41:54 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 14 Aug 2023 17:41:54 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8bed2eae372fe236061920d89ae1ce89695a12df84989113bcc7ce4bd9774456`  
		Last Modified: Mon, 07 Aug 2023 19:42:39 GMT  
		Size: 3.2 MB (3214195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec90be18226e5c99d10161aed1a143f4134093c55b4d6979bbdbbe4b0683eb11`  
		Last Modified: Mon, 07 Aug 2023 20:30:59 GMT  
		Size: 285.1 KB (285089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c751f85e4ba6e9bbada0b11691d914b2ec2c689bb0dca6b9cbe994488d0e3e`  
		Last Modified: Mon, 07 Aug 2023 20:31:56 GMT  
		Size: 100.9 MB (100865267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2d202223222826c8580d85b8d7dd6baa8ed1cad84ba5cf47dab23eaeeae7e9`  
		Last Modified: Mon, 07 Aug 2023 20:31:43 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0359ada615d16e203e1d40a49b896060013c2952c2982ae73b141cc291305a4c`  
		Last Modified: Tue, 08 Aug 2023 05:25:47 GMT  
		Size: 5.1 MB (5099943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1039996d136f688a91d291dcf3dbb995607af1f245f1741d8ad0c5f73cec1b01`  
		Last Modified: Mon, 14 Aug 2023 17:42:27 GMT  
		Size: 1.3 MB (1262391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17e7bfc7e0d6b6a7f70b22841fe42427f0fb6372b17c71c8063c50d7c8e73c1`  
		Last Modified: Mon, 14 Aug 2023 17:42:27 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:e47c546e0564931b55495f764fdfb59d8d81d4e51ff9a221952688b1dcf6d462
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:a6ebd264677820f38a44fb346c24e5b3cc1406cf5f975a99a089e14f2cfeb623
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2132345169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec0a81535ff140c0b08b259f2eb43a2face74a8aaeed3cc1ac39ef9b4e90c3f6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:39:54 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:39:55 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:39:56 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:41:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:41:12 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:42:07 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:53:35 GMT
ENV GOLANG_VERSION=1.20.7
# Thu, 10 Aug 2023 00:56:38 GMT
RUN $url = 'https://dl.google.com/go/go1.20.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '736dc6c7fcab1c96b682c8c93e38d7e371e62a17d34cb2c37d451a1147f66af9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:56:40 GMT
WORKDIR C:\go
# Thu, 10 Aug 2023 03:04:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 03:04:56 GMT
ENV XCADDY_VERSION=v0.3.4
# Thu, 10 Aug 2023 03:04:57 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:04:57 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Aug 2023 03:06:01 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('542b4c083852d41081186c79757b66ff3c26248f72ed461dbc038b51687d0a8a8ce8eee69e3b5a1d43360c48b3405b611b940fa378debe98aaa0b3c5aebfa218')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 10 Aug 2023 03:06:02 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594083c5c2094c95b4e52723d54c14e0d70881f4f176720c3170012275accc3b`  
		Last Modified: Thu, 10 Aug 2023 01:02:54 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e2c2a5b75ced3a3a50be088c4a6c2d7df926b1fe6515b2d0c021312e3642f4`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d28688050deeec928289543beadf5c75bb2a8246576cb7c066e23818016217`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e5fbc50e7e0fefb7c9e349038ecb00ed5c000bcab8c4d82b1e1000c4273c01`  
		Last Modified: Thu, 10 Aug 2023 01:02:52 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0544e07bd9df923e11e09c7dc042da614f2f14589eb6fa79005ebbbf2731e97d`  
		Last Modified: Thu, 10 Aug 2023 01:02:57 GMT  
		Size: 25.6 MB (25560980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555a82506c4fcec2bd90ae77756e5b03788e30c89f1a3820aa0b6a7ae6ad58ae`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bcfb422b104764156fc5ba099b5e3ae9fa9f760fd2db1c21acd8969b3d73de`  
		Last Modified: Thu, 10 Aug 2023 01:02:50 GMT  
		Size: 220.8 KB (220796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c6aa0a5a1689ed800c4ef72c1b9febf207840fd2c6abfe4bb460e2e2bfb0b0`  
		Last Modified: Thu, 10 Aug 2023 01:05:03 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53d3379322a67b2413189cc2b779d22cb4093124343c8bb17fdf720b7b49fda`  
		Last Modified: Thu, 10 Aug 2023 01:05:25 GMT  
		Size: 108.9 MB (108911716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b60ccf92610ddbc47a05664785c95215a123e8930afbf6e3e2cefc80e693fd2`  
		Last Modified: Thu, 10 Aug 2023 01:05:04 GMT  
		Size: 1.5 KB (1468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2c7d6253e62d61e5e0d2ad331a96cff5175f6c608b2ab4657825b3e3b4b4d0`  
		Last Modified: Thu, 10 Aug 2023 03:08:03 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c54227291fad3a25beb98d755de6f26fee6576e1b807e42c0bb70aa45793b3`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d107b434fabbe0d8d3916744b92501e6f5f8dabf7621ce44432d53d3853b4b8`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b0bcd286241a360f34f20c3842b90b6f53c31abe4d60fcb8f1148e8ba191a3`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5677a754ea49eeeb0b5ed56da2ac0d43c11e3c935c36adc2cc71b95dc7b99c0f`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.7 MB (1679125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4626f9b6f575add3a8f4ac9248f4342e9cb80f9abf696deff5a7bd9aff57fbf1`  
		Last Modified: Thu, 10 Aug 2023 03:08:01 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:b21f945f75a0af5f372c03cead52a84f725ba635c6f414ff9bcdfd81c64008c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1906; amd64

### `caddy:builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:44aba8da329d3ea3489327b5c94e41477f815f943659f4464a2c859ad400dcfd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1933815424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d095c2914283b4b75e4dbb95eb3e7f5ff6db80079dc6981bf1c5fa8355036c99`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:36:23 GMT
ENV GIT_VERSION=2.23.0
# Thu, 10 Aug 2023 00:36:24 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 10 Aug 2023 00:36:25 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 10 Aug 2023 00:36:26 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 10 Aug 2023 00:36:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:37:00 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:37:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 10 Aug 2023 00:50:52 GMT
ENV GOLANG_VERSION=1.20.7
# Thu, 10 Aug 2023 00:53:17 GMT
RUN $url = 'https://dl.google.com/go/go1.20.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '736dc6c7fcab1c96b682c8c93e38d7e371e62a17d34cb2c37d451a1147f66af9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 10 Aug 2023 00:53:18 GMT
WORKDIR C:\go
# Thu, 10 Aug 2023 03:06:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 03:06:10 GMT
ENV XCADDY_VERSION=v0.3.4
# Thu, 10 Aug 2023 03:06:11 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:06:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Aug 2023 03:06:34 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.4/xcaddy_0.3.4_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('542b4c083852d41081186c79757b66ff3c26248f72ed461dbc038b51687d0a8a8ce8eee69e3b5a1d43360c48b3405b611b940fa378debe98aaa0b3c5aebfa218')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 10 Aug 2023 03:06:35 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877256a6389e5e2563da79ad5bd201e7ee136abf14ff7cb0d4efbf3b24e5f127`  
		Last Modified: Thu, 10 Aug 2023 01:02:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a39df29b3c0b2f7e691c47273110db4a46e5c8e299f6bb95f77a9c61f79872`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8574d63bce1547e3177d0b76237a782a9b016d4880375dcd1a7b6a1c5dee3dc`  
		Last Modified: Thu, 10 Aug 2023 01:02:18 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ef34b3c96316bcdd92e24c8c4eebdc3a35f245c013ef87edfae0dde091a305`  
		Last Modified: Thu, 10 Aug 2023 01:02:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a481babc5b629f694446a96dba8d77c020257c98334c605aff94162b9a917279`  
		Last Modified: Thu, 10 Aug 2023 01:02:23 GMT  
		Size: 25.6 MB (25554169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281178ea1c103ff07ea7e4fb647eb0dbe4f865742da6ef9944e04f37974fc27c`  
		Last Modified: Thu, 10 Aug 2023 01:02:15 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b5d34adf2aacfe87580143f3e17c635dc8dbd4068377b79b35d665f49bbad9`  
		Last Modified: Thu, 10 Aug 2023 01:02:16 GMT  
		Size: 275.9 KB (275946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02a2e79b5a05c2145c733eefb2add45d1ebefb7a16b93c321f5883c8ced6f1a`  
		Last Modified: Thu, 10 Aug 2023 01:04:30 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd9991b8cfbc481c153abf1625143209f4c4fd40d9443a5a19f4e3613336ad2`  
		Last Modified: Thu, 10 Aug 2023 01:04:53 GMT  
		Size: 108.9 MB (108927695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dc6778f41c3c7d50b8e71668e22880153d6c6794f24c4661fc3d6aa089d0a5`  
		Last Modified: Thu, 10 Aug 2023 01:04:30 GMT  
		Size: 1.5 KB (1547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c5985f015e143065716f5aabf0ecaed537103c5ec07e6c57360204a7787d02`  
		Last Modified: Thu, 10 Aug 2023 03:08:23 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd9cf527e30318df5bccd0be2c9a9716dc073b1f84c1d2c5cadc85adcf2af02`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604bc0fdaac29b943186656363f9267b86b2744da35d6b519a428d494d0a6bd3`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b527a45b48b4328e0ea94e3e2d3f239ed4f960d30ea0b9272cd902aec85c8b`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9ae10f93498ae3f8bbfef69dd561e41337584fb8dcc09fe82ed4971f9787be`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.7 MB (1675642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6218363385083ee3dbece9e5e2fd5c9086be201ca76bd6818b46bb6e591688eb`  
		Last Modified: Thu, 10 Aug 2023 03:08:21 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:6c60e52f0acf862774d17f362aadc4895667d42b24ca6e74ee1e7f09a1363424
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4737; amd64
	-	windows version 10.0.20348.1906; amd64

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
$ docker pull caddy@sha256:dc698bd1b82521df87ea42fbf48c98d10133ec962497ac80527b65769ceb6a9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17690701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3775ac20cca67f4d547f26f5984a989b9407b0c4129fd6cd86dbb3359249acd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:38:27 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:49:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:49:14 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:49:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:49:16 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:49:16 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:49:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:49:17 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:49:18 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:49:18 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:49:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172ef460a93549b8a3e73f6a515bccad93512788d1e8f095e7230ba41967c25a`  
		Last Modified: Wed, 09 Aug 2023 03:38:53 GMT  
		Size: 347.7 KB (347686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7aae78767a581df85fd1a51ccd646619aec320896ca016ef0f05a41b16bcbfe`  
		Last Modified: Mon, 14 Aug 2023 17:49:36 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5244db1c019e66038874df2b8b92c74437f6d355802bfccada90c9d8bd8d29`  
		Last Modified: Mon, 14 Aug 2023 17:49:38 GMT  
		Size: 14.2 MB (14190701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:e9cb1245e1c134e25a0ec0803e5132ba9ba92d0a4ad85db3f73bd2c3188cf70e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17414619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df6e2a1f4c707dc77276814a27ac22a7b5de268780603d8e08324130e1fc563`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 01:51:41 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:57:17 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:57:17 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:57:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:57:20 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:57:20 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:57:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:57:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:57:21 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:57:21 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:57:21 GMT
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
	-	`sha256:46e1b3e18d5e992f1805072b2d52405d575830bdce21726ef99dea99e31d8277`  
		Last Modified: Mon, 14 Aug 2023 17:57:42 GMT  
		Size: 7.5 KB (7505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2b7485982d191f9dc0498d5b940d14df575f36ca66876b92d3ca09ff9386b2`  
		Last Modified: Mon, 14 Aug 2023 17:57:48 GMT  
		Size: 14.2 MB (14163172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:db04154ce5f7a7f4d058567375880cdc6b1a3675095ad576f9886f39f1374afc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17329640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:731c0ae21a974e5708c4a8006250893bca5a2ecad43babf2a0a95a60fc61d6cd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:09:12 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:39:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:39:19 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:39:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:39:21 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:39:21 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:39:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:39:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:39:22 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:39:22 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:39:22 GMT
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
	-	`sha256:f7488af8b96c79b6db13955a0302653c4e9f314d0833201984ae06c1ed697f06`  
		Last Modified: Mon, 14 Aug 2023 17:39:41 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9600da6e7e51b9083b29f3c7de592fa45e7765ca5ffe8d2abf7cc99c50578fe`  
		Last Modified: Mon, 14 Aug 2023 17:39:43 GMT  
		Size: 13.6 MB (13630728 bytes)  
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
$ docker pull caddy@sha256:3b3d4b80e160105a760ad62b32c497245d69676e6053c2a7b61bc5c6fc178fd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.0 MB (17984968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a63d05bc7601e47460ff86bc91380fd9407c0b4886b80836ac3aadb436f68e1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:41:54 GMT
ADD file:b57ea5bba3c986df3471f3ea27443a9a4b19d40c46f9fbca8bb6077b399725aa in / 
# Mon, 07 Aug 2023 19:41:55 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:14:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 17:41:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Mon, 14 Aug 2023 17:41:39 GMT
ENV CADDY_VERSION=v2.7.3
# Mon, 14 Aug 2023 17:41:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ae7a367be45f5cdaa9e5fd082e225dd84f291a6fb1fe2fefa05b9958461e0967d02de23c9147c8e8ebdc4c91b352e887c1c95b06a64fde6be69a5a32fc459d5e' ;; 		armhf)   binArch='armv6'; checksum='d6744a5e835b08208f5bfcd17525ace7b77420bca575126831f0c27100bc2b5f1ce5dcc08585e90bc8e45261d1bacd2ee37d0b1ac7bd57525e953f2a383f2820' ;; 		armv7)   binArch='armv7'; checksum='eed7a8e99dd0802b195986e077a0607536680fc22d735bde2a2773becdd2ab1063754940264dc0f1c1ca81d8d8647e0924a16aead067f1c73c5c372de9320e5c' ;; 		aarch64) binArch='arm64'; checksum='258429b3e7fe821c132f4d455a69c2d230a3f90d18bfebdbf7e9676099e7c6dc1a12af7e0b526b8f6b044cb10fe2aab12e449e529e5ed316b7e5b8433e1b353a' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='af49e94af887ef9090ff664877fdb462f33a129f6565504d7cc4b6e3c2995dd4b1b831338809b2450edfea292defa05711beb7cae35331995117258650e17de1' ;; 		s390x)   binArch='s390x'; checksum='81a2bd1e27bf1793c1979009973b468bfc4d05486888ad0376f0e425ef28812e3149f1f7f60dc924d914af6e8ee7ac90c7e1a9c8dd20c2c370f7063c3fa5049a' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.3/caddy_2.7.3_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 14 Aug 2023 17:41:43 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 14 Aug 2023 17:41:43 GMT
ENV XDG_DATA_HOME=/data
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.version=v2.7.3
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 14 Aug 2023 17:41:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 14 Aug 2023 17:41:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 80
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 443
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 443/udp
# Mon, 14 Aug 2023 17:41:44 GMT
EXPOSE 2019
# Mon, 14 Aug 2023 17:41:44 GMT
WORKDIR /srv
# Mon, 14 Aug 2023 17:41:44 GMT
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
	-	`sha256:308478977890baa82477ee70a3065fb9da2080efcc95facf1a87ac021b06a8e9`  
		Last Modified: Mon, 14 Aug 2023 17:42:17 GMT  
		Size: 7.5 KB (7503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fe1cbba37a3c1c2f6ba50e59e5c238c8d83ffca820ef709108b9e3253af757`  
		Last Modified: Mon, 14 Aug 2023 17:42:19 GMT  
		Size: 14.4 MB (14408320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:1b4a86d284b971594d7e30ef09451be59ba84514b612c87b6406e2dfb8e9e23f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2011958834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ae5f48eae2f949ec09ad9f70ff2c2626318e07111bea5b6622116482ac991b0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 02:59:41 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Aug 2023 02:59:41 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:00:57 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('69d2d73c2514ab5ce4f6a60489c79ce4da0e1d4302c85ab584d0a7a7fd0d034bfe5a5caab78c96ac3383ddd7d2e12c3c41fb47c4716909d2a78d448b0289ccec')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Aug 2023 03:00:58 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Aug 2023 03:00:59 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Aug 2023 03:01:00 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Thu, 10 Aug 2023 03:01:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Aug 2023 03:01:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Aug 2023 03:01:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Aug 2023 03:01:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Aug 2023 03:01:03 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Aug 2023 03:01:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Aug 2023 03:01:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Aug 2023 03:01:06 GMT
EXPOSE 80
# Thu, 10 Aug 2023 03:01:06 GMT
EXPOSE 443
# Thu, 10 Aug 2023 03:01:07 GMT
EXPOSE 443/udp
# Thu, 10 Aug 2023 03:01:08 GMT
EXPOSE 2019
# Thu, 10 Aug 2023 03:03:10 GMT
RUN caddy version
# Thu, 10 Aug 2023 03:03:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907ddb8e2b3b8f440ec855971bf77d521900d3faecd1816d7146d89f1c78f408`  
		Last Modified: Thu, 10 Aug 2023 03:07:15 GMT  
		Size: 469.4 KB (469388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d430330f12b22fcc17a5d114d51ba3bb8e62a55f87b67f939d18651c226f927`  
		Last Modified: Thu, 10 Aug 2023 03:07:15 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd493f43c2fb25a7c8540ea353a098f784a6e8d5fe4e9d070e4a1de796cde96c`  
		Last Modified: Thu, 10 Aug 2023 03:07:18 GMT  
		Size: 15.2 MB (15241515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95b32f0fb8252db266318cca24c13f5eea8b8b3c19405b92f1a8b9199e39c5d`  
		Last Modified: Thu, 10 Aug 2023 03:07:14 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7dbc1767506f0f3f5b4d3a9671f97a723014ae1e38cf8056f6257db7917a88`  
		Last Modified: Thu, 10 Aug 2023 03:07:13 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7905b1f85b201367c5a62618ddc55da9a60cbb3da1da40ab60a88c125a5956`  
		Last Modified: Thu, 10 Aug 2023 03:07:13 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce34081b153cf49ce89b2ff4fc81f54a648cefc5d2dbb0f60048b94ba10f43b`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9622cc1048f5f7259d3263b67dd386c5d70ae4cf0a358c33deb3df8cdb316efd`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b1ca0970bf360a0627a1deae2985b658f54b41758f12f4e5448ed1aee3bc82`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503770a8fe554599aa8e6413082b7cb24d7f1faa328deaf28b34ddb2a294972b`  
		Last Modified: Thu, 10 Aug 2023 03:07:11 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea5eee99969c433a1c2f4d0f7fdc838185350144b9d3f20888c2a53cc6f3563`  
		Last Modified: Thu, 10 Aug 2023 03:07:11 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675093fb34c31fff953a92ee1831f09679783e7d3e1d9ff40a962f346d1dc581`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fd64685610dd5572f21efe3fae8cb13537c9deb6693caf4097bf9ec3b4dabe`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540e52aaf0b1acca0c4a9fbb2a60e5ce4bca2c119fbb3bbd86658186b23e3202`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29819bc504b56dacdb0df898ee58e26d8097802c0a5578cd14d4e3ed0655bde7`  
		Last Modified: Thu, 10 Aug 2023 03:07:09 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2157a412d53cd6d3174744de6c1cf5cb0dd03274fe9b36f749525867e4b9bd2`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cfbf0b65ccf78eb536c8a23f0b92fa148268c1fa4a39c1b19c7d9310e53b8d`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7faedca764204aa914e83a3721476c9a6a7f8177d057021e5a1debb81a436808`  
		Last Modified: Thu, 10 Aug 2023 03:07:09 GMT  
		Size: 268.6 KB (268640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86622825a44d72176deccdf0a5e4c9127ebf8f2591211cbdae585e9977363e8`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:144bc31c96841830b174ed1ff2da09ba18881208aae2efd16b3c850953f762f6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1813356270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02028c6ef8441cbf5181f34f78b4740b60dffff030772882302c9ca39f9a6096`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 03:03:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Aug 2023 03:03:52 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:04:21 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('69d2d73c2514ab5ce4f6a60489c79ce4da0e1d4302c85ab584d0a7a7fd0d034bfe5a5caab78c96ac3383ddd7d2e12c3c41fb47c4716909d2a78d448b0289ccec')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Aug 2023 03:04:21 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Aug 2023 03:04:22 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Aug 2023 03:04:23 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Thu, 10 Aug 2023 03:04:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Aug 2023 03:04:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Aug 2023 03:04:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Aug 2023 03:04:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Aug 2023 03:04:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Aug 2023 03:04:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Aug 2023 03:04:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Aug 2023 03:04:29 GMT
EXPOSE 80
# Thu, 10 Aug 2023 03:04:30 GMT
EXPOSE 443
# Thu, 10 Aug 2023 03:04:31 GMT
EXPOSE 443/udp
# Thu, 10 Aug 2023 03:04:32 GMT
EXPOSE 2019
# Thu, 10 Aug 2023 03:04:47 GMT
RUN caddy version
# Thu, 10 Aug 2023 03:04:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee168d3c6067847c3aef71a2a0dfdc70984b0bb6164086b49da7bd27de3ff3e4`  
		Last Modified: Thu, 10 Aug 2023 03:07:41 GMT  
		Size: 462.1 KB (462122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0efe6e8d5895981c45dc711aa05390379a6f7e5ceea618991435f40db1736c5`  
		Last Modified: Thu, 10 Aug 2023 03:07:40 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c66dfda490f2720f8d21e51546bae9f4e21a4b3b76b29f45e18435544c66a7c`  
		Last Modified: Thu, 10 Aug 2023 03:07:44 GMT  
		Size: 15.2 MB (15227189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67327c2fc33a0a30f2e409ada51c37d6663c07a498c7663987be61f888f7a8`  
		Last Modified: Thu, 10 Aug 2023 03:07:40 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c73910f4e5bd8630e3f4a5c23d004a9f6eff60c9f50af18e4b1d9b5f9ac0aa4`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d17a44e8dc24bdc71a9866c99b7022ca1a00e04acc6bf00dbf794c0550bb79d`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851a0578d2d21e2b22a64fe518454ef0283a718573db4e60e3b4a0121bd4081a`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ab80276792afc4370db678044627f33dabc32a9a987d736686239ed1d85a5b`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dcfba0d938817014a224fd3369379868ad4bd05a910cf582eb5e88ca8630ce`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd3ed16ce737bd3530ec90c77867e59892ce05deebca1a42256c570b86ddf1a`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb186d102ae807e026f9de311625fe281b24e140d91adaa2c46298a163035182`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267fad2b6b29094e45425d6b1d39b3f0a295ee7bbce5489aab9e77a659c7ef09`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608cb1e8b46f127167ebb53ec28593783baa810d0ec8e54a929e2907cea85352`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dadf995868b2bcb1e42a4b48f3df0ccd9a979672da04a75dad7970b567bb793`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4209fa97cbb4a651cae617cf81de393ea0652645a1f00b607c18dfa26834c475`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e65f2bc3967a653972ae76ef447ff72659e620a98280fe5230591a0e7c29cd`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9d8975e744e0f5b82190fc02ef017a7f4e7ffa1dda69f5be10f43ffa554d9e`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef526b9884253387824d19beee5d18eee6650c38429c56acd30286c1ea94da03`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 280.0 KB (280042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0266d9103b52d7b0129a0aa08ddab9c5bdfca0694ed3368c0b9c887941c524a`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:ee77e6dfe66fce930f6e92b862071843a872dfc67ee4b8ad9c0e843a0c4103fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4737; amd64
	-	windows version 10.0.20348.1906; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:1b4a86d284b971594d7e30ef09451be59ba84514b612c87b6406e2dfb8e9e23f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2011958834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ae5f48eae2f949ec09ad9f70ff2c2626318e07111bea5b6622116482ac991b0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 02:59:41 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Aug 2023 02:59:41 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:00:57 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('69d2d73c2514ab5ce4f6a60489c79ce4da0e1d4302c85ab584d0a7a7fd0d034bfe5a5caab78c96ac3383ddd7d2e12c3c41fb47c4716909d2a78d448b0289ccec')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Aug 2023 03:00:58 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Aug 2023 03:00:59 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Aug 2023 03:01:00 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Thu, 10 Aug 2023 03:01:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Aug 2023 03:01:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Aug 2023 03:01:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Aug 2023 03:01:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Aug 2023 03:01:03 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Aug 2023 03:01:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Aug 2023 03:01:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Aug 2023 03:01:06 GMT
EXPOSE 80
# Thu, 10 Aug 2023 03:01:06 GMT
EXPOSE 443
# Thu, 10 Aug 2023 03:01:07 GMT
EXPOSE 443/udp
# Thu, 10 Aug 2023 03:01:08 GMT
EXPOSE 2019
# Thu, 10 Aug 2023 03:03:10 GMT
RUN caddy version
# Thu, 10 Aug 2023 03:03:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907ddb8e2b3b8f440ec855971bf77d521900d3faecd1816d7146d89f1c78f408`  
		Last Modified: Thu, 10 Aug 2023 03:07:15 GMT  
		Size: 469.4 KB (469388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d430330f12b22fcc17a5d114d51ba3bb8e62a55f87b67f939d18651c226f927`  
		Last Modified: Thu, 10 Aug 2023 03:07:15 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd493f43c2fb25a7c8540ea353a098f784a6e8d5fe4e9d070e4a1de796cde96c`  
		Last Modified: Thu, 10 Aug 2023 03:07:18 GMT  
		Size: 15.2 MB (15241515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95b32f0fb8252db266318cca24c13f5eea8b8b3c19405b92f1a8b9199e39c5d`  
		Last Modified: Thu, 10 Aug 2023 03:07:14 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7dbc1767506f0f3f5b4d3a9671f97a723014ae1e38cf8056f6257db7917a88`  
		Last Modified: Thu, 10 Aug 2023 03:07:13 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7905b1f85b201367c5a62618ddc55da9a60cbb3da1da40ab60a88c125a5956`  
		Last Modified: Thu, 10 Aug 2023 03:07:13 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce34081b153cf49ce89b2ff4fc81f54a648cefc5d2dbb0f60048b94ba10f43b`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9622cc1048f5f7259d3263b67dd386c5d70ae4cf0a358c33deb3df8cdb316efd`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b1ca0970bf360a0627a1deae2985b658f54b41758f12f4e5448ed1aee3bc82`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503770a8fe554599aa8e6413082b7cb24d7f1faa328deaf28b34ddb2a294972b`  
		Last Modified: Thu, 10 Aug 2023 03:07:11 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea5eee99969c433a1c2f4d0f7fdc838185350144b9d3f20888c2a53cc6f3563`  
		Last Modified: Thu, 10 Aug 2023 03:07:11 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675093fb34c31fff953a92ee1831f09679783e7d3e1d9ff40a962f346d1dc581`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fd64685610dd5572f21efe3fae8cb13537c9deb6693caf4097bf9ec3b4dabe`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540e52aaf0b1acca0c4a9fbb2a60e5ce4bca2c119fbb3bbd86658186b23e3202`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29819bc504b56dacdb0df898ee58e26d8097802c0a5578cd14d4e3ed0655bde7`  
		Last Modified: Thu, 10 Aug 2023 03:07:09 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2157a412d53cd6d3174744de6c1cf5cb0dd03274fe9b36f749525867e4b9bd2`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cfbf0b65ccf78eb536c8a23f0b92fa148268c1fa4a39c1b19c7d9310e53b8d`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7faedca764204aa914e83a3721476c9a6a7f8177d057021e5a1debb81a436808`  
		Last Modified: Thu, 10 Aug 2023 03:07:09 GMT  
		Size: 268.6 KB (268640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86622825a44d72176deccdf0a5e4c9127ebf8f2591211cbdae585e9977363e8`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:144bc31c96841830b174ed1ff2da09ba18881208aae2efd16b3c850953f762f6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1813356270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02028c6ef8441cbf5181f34f78b4740b60dffff030772882302c9ca39f9a6096`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 03:03:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Aug 2023 03:03:52 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:04:21 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('69d2d73c2514ab5ce4f6a60489c79ce4da0e1d4302c85ab584d0a7a7fd0d034bfe5a5caab78c96ac3383ddd7d2e12c3c41fb47c4716909d2a78d448b0289ccec')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Aug 2023 03:04:21 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Aug 2023 03:04:22 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Aug 2023 03:04:23 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Thu, 10 Aug 2023 03:04:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Aug 2023 03:04:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Aug 2023 03:04:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Aug 2023 03:04:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Aug 2023 03:04:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Aug 2023 03:04:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Aug 2023 03:04:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Aug 2023 03:04:29 GMT
EXPOSE 80
# Thu, 10 Aug 2023 03:04:30 GMT
EXPOSE 443
# Thu, 10 Aug 2023 03:04:31 GMT
EXPOSE 443/udp
# Thu, 10 Aug 2023 03:04:32 GMT
EXPOSE 2019
# Thu, 10 Aug 2023 03:04:47 GMT
RUN caddy version
# Thu, 10 Aug 2023 03:04:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee168d3c6067847c3aef71a2a0dfdc70984b0bb6164086b49da7bd27de3ff3e4`  
		Last Modified: Thu, 10 Aug 2023 03:07:41 GMT  
		Size: 462.1 KB (462122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0efe6e8d5895981c45dc711aa05390379a6f7e5ceea618991435f40db1736c5`  
		Last Modified: Thu, 10 Aug 2023 03:07:40 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c66dfda490f2720f8d21e51546bae9f4e21a4b3b76b29f45e18435544c66a7c`  
		Last Modified: Thu, 10 Aug 2023 03:07:44 GMT  
		Size: 15.2 MB (15227189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67327c2fc33a0a30f2e409ada51c37d6663c07a498c7663987be61f888f7a8`  
		Last Modified: Thu, 10 Aug 2023 03:07:40 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c73910f4e5bd8630e3f4a5c23d004a9f6eff60c9f50af18e4b1d9b5f9ac0aa4`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d17a44e8dc24bdc71a9866c99b7022ca1a00e04acc6bf00dbf794c0550bb79d`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851a0578d2d21e2b22a64fe518454ef0283a718573db4e60e3b4a0121bd4081a`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ab80276792afc4370db678044627f33dabc32a9a987d736686239ed1d85a5b`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dcfba0d938817014a224fd3369379868ad4bd05a910cf582eb5e88ca8630ce`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd3ed16ce737bd3530ec90c77867e59892ce05deebca1a42256c570b86ddf1a`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb186d102ae807e026f9de311625fe281b24e140d91adaa2c46298a163035182`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267fad2b6b29094e45425d6b1d39b3f0a295ee7bbce5489aab9e77a659c7ef09`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608cb1e8b46f127167ebb53ec28593783baa810d0ec8e54a929e2907cea85352`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dadf995868b2bcb1e42a4b48f3df0ccd9a979672da04a75dad7970b567bb793`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4209fa97cbb4a651cae617cf81de393ea0652645a1f00b607c18dfa26834c475`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e65f2bc3967a653972ae76ef447ff72659e620a98280fe5230591a0e7c29cd`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9d8975e744e0f5b82190fc02ef017a7f4e7ffa1dda69f5be10f43ffa554d9e`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef526b9884253387824d19beee5d18eee6650c38429c56acd30286c1ea94da03`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 280.0 KB (280042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0266d9103b52d7b0129a0aa08ddab9c5bdfca0694ed3368c0b9c887941c524a`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:40d5f0aa53bb62f81ccb8625ca40ae2b0057b977b8432daa5d3a76079b9737e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull caddy@sha256:1b4a86d284b971594d7e30ef09451be59ba84514b612c87b6406e2dfb8e9e23f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2011958834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ae5f48eae2f949ec09ad9f70ff2c2626318e07111bea5b6622116482ac991b0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 02:59:41 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Aug 2023 02:59:41 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:00:57 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('69d2d73c2514ab5ce4f6a60489c79ce4da0e1d4302c85ab584d0a7a7fd0d034bfe5a5caab78c96ac3383ddd7d2e12c3c41fb47c4716909d2a78d448b0289ccec')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Aug 2023 03:00:58 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Aug 2023 03:00:59 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Aug 2023 03:01:00 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Thu, 10 Aug 2023 03:01:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Aug 2023 03:01:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Aug 2023 03:01:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Aug 2023 03:01:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Aug 2023 03:01:03 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Aug 2023 03:01:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Aug 2023 03:01:05 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Aug 2023 03:01:06 GMT
EXPOSE 80
# Thu, 10 Aug 2023 03:01:06 GMT
EXPOSE 443
# Thu, 10 Aug 2023 03:01:07 GMT
EXPOSE 443/udp
# Thu, 10 Aug 2023 03:01:08 GMT
EXPOSE 2019
# Thu, 10 Aug 2023 03:03:10 GMT
RUN caddy version
# Thu, 10 Aug 2023 03:03:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907ddb8e2b3b8f440ec855971bf77d521900d3faecd1816d7146d89f1c78f408`  
		Last Modified: Thu, 10 Aug 2023 03:07:15 GMT  
		Size: 469.4 KB (469388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d430330f12b22fcc17a5d114d51ba3bb8e62a55f87b67f939d18651c226f927`  
		Last Modified: Thu, 10 Aug 2023 03:07:15 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd493f43c2fb25a7c8540ea353a098f784a6e8d5fe4e9d070e4a1de796cde96c`  
		Last Modified: Thu, 10 Aug 2023 03:07:18 GMT  
		Size: 15.2 MB (15241515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95b32f0fb8252db266318cca24c13f5eea8b8b3c19405b92f1a8b9199e39c5d`  
		Last Modified: Thu, 10 Aug 2023 03:07:14 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7dbc1767506f0f3f5b4d3a9671f97a723014ae1e38cf8056f6257db7917a88`  
		Last Modified: Thu, 10 Aug 2023 03:07:13 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7905b1f85b201367c5a62618ddc55da9a60cbb3da1da40ab60a88c125a5956`  
		Last Modified: Thu, 10 Aug 2023 03:07:13 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce34081b153cf49ce89b2ff4fc81f54a648cefc5d2dbb0f60048b94ba10f43b`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9622cc1048f5f7259d3263b67dd386c5d70ae4cf0a358c33deb3df8cdb316efd`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b1ca0970bf360a0627a1deae2985b658f54b41758f12f4e5448ed1aee3bc82`  
		Last Modified: Thu, 10 Aug 2023 03:07:12 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503770a8fe554599aa8e6413082b7cb24d7f1faa328deaf28b34ddb2a294972b`  
		Last Modified: Thu, 10 Aug 2023 03:07:11 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea5eee99969c433a1c2f4d0f7fdc838185350144b9d3f20888c2a53cc6f3563`  
		Last Modified: Thu, 10 Aug 2023 03:07:11 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675093fb34c31fff953a92ee1831f09679783e7d3e1d9ff40a962f346d1dc581`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fd64685610dd5572f21efe3fae8cb13537c9deb6693caf4097bf9ec3b4dabe`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540e52aaf0b1acca0c4a9fbb2a60e5ce4bca2c119fbb3bbd86658186b23e3202`  
		Last Modified: Thu, 10 Aug 2023 03:07:10 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29819bc504b56dacdb0df898ee58e26d8097802c0a5578cd14d4e3ed0655bde7`  
		Last Modified: Thu, 10 Aug 2023 03:07:09 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2157a412d53cd6d3174744de6c1cf5cb0dd03274fe9b36f749525867e4b9bd2`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cfbf0b65ccf78eb536c8a23f0b92fa148268c1fa4a39c1b19c7d9310e53b8d`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7faedca764204aa914e83a3721476c9a6a7f8177d057021e5a1debb81a436808`  
		Last Modified: Thu, 10 Aug 2023 03:07:09 GMT  
		Size: 268.6 KB (268640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86622825a44d72176deccdf0a5e4c9127ebf8f2591211cbdae585e9977363e8`  
		Last Modified: Thu, 10 Aug 2023 03:07:08 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:32d0082c4ae3fdb4c834f812d8c65442f02e9ea2e037e23a5fa80b0399bbf314
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1906; amd64

### `caddy:windowsservercore-ltsc2022` - windows version 10.0.20348.1906; amd64

```console
$ docker pull caddy@sha256:144bc31c96841830b174ed1ff2da09ba18881208aae2efd16b3c850953f762f6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1813356270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02028c6ef8441cbf5181f34f78b4740b60dffff030772882302c9ca39f9a6096`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 03:03:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/5910351159c2995a9a1c911d7879de6ff598d905/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Aug 2023 03:03:52 GMT
ENV CADDY_VERSION=v2.7.2
# Thu, 10 Aug 2023 03:04:21 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.2/caddy_2.7.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('69d2d73c2514ab5ce4f6a60489c79ce4da0e1d4302c85ab584d0a7a7fd0d034bfe5a5caab78c96ac3383ddd7d2e12c3c41fb47c4716909d2a78d448b0289ccec')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Aug 2023 03:04:21 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Aug 2023 03:04:22 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Aug 2023 03:04:23 GMT
LABEL org.opencontainers.image.version=v2.7.2
# Thu, 10 Aug 2023 03:04:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Aug 2023 03:04:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Aug 2023 03:04:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Aug 2023 03:04:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Aug 2023 03:04:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Aug 2023 03:04:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Aug 2023 03:04:28 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Aug 2023 03:04:29 GMT
EXPOSE 80
# Thu, 10 Aug 2023 03:04:30 GMT
EXPOSE 443
# Thu, 10 Aug 2023 03:04:31 GMT
EXPOSE 443/udp
# Thu, 10 Aug 2023 03:04:32 GMT
EXPOSE 2019
# Thu, 10 Aug 2023 03:04:47 GMT
RUN caddy version
# Thu, 10 Aug 2023 03:04:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee168d3c6067847c3aef71a2a0dfdc70984b0bb6164086b49da7bd27de3ff3e4`  
		Last Modified: Thu, 10 Aug 2023 03:07:41 GMT  
		Size: 462.1 KB (462122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0efe6e8d5895981c45dc711aa05390379a6f7e5ceea618991435f40db1736c5`  
		Last Modified: Thu, 10 Aug 2023 03:07:40 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c66dfda490f2720f8d21e51546bae9f4e21a4b3b76b29f45e18435544c66a7c`  
		Last Modified: Thu, 10 Aug 2023 03:07:44 GMT  
		Size: 15.2 MB (15227189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de67327c2fc33a0a30f2e409ada51c37d6663c07a498c7663987be61f888f7a8`  
		Last Modified: Thu, 10 Aug 2023 03:07:40 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c73910f4e5bd8630e3f4a5c23d004a9f6eff60c9f50af18e4b1d9b5f9ac0aa4`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d17a44e8dc24bdc71a9866c99b7022ca1a00e04acc6bf00dbf794c0550bb79d`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851a0578d2d21e2b22a64fe518454ef0283a718573db4e60e3b4a0121bd4081a`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ab80276792afc4370db678044627f33dabc32a9a987d736686239ed1d85a5b`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dcfba0d938817014a224fd3369379868ad4bd05a910cf582eb5e88ca8630ce`  
		Last Modified: Thu, 10 Aug 2023 03:07:38 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd3ed16ce737bd3530ec90c77867e59892ce05deebca1a42256c570b86ddf1a`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb186d102ae807e026f9de311625fe281b24e140d91adaa2c46298a163035182`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267fad2b6b29094e45425d6b1d39b3f0a295ee7bbce5489aab9e77a659c7ef09`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608cb1e8b46f127167ebb53ec28593783baa810d0ec8e54a929e2907cea85352`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dadf995868b2bcb1e42a4b48f3df0ccd9a979672da04a75dad7970b567bb793`  
		Last Modified: Thu, 10 Aug 2023 03:07:36 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4209fa97cbb4a651cae617cf81de393ea0652645a1f00b607c18dfa26834c475`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e65f2bc3967a653972ae76ef447ff72659e620a98280fe5230591a0e7c29cd`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9d8975e744e0f5b82190fc02ef017a7f4e7ffa1dda69f5be10f43ffa554d9e`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef526b9884253387824d19beee5d18eee6650c38429c56acd30286c1ea94da03`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 280.0 KB (280042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0266d9103b52d7b0129a0aa08ddab9c5bdfca0694ed3368c0b9c887941c524a`  
		Last Modified: Thu, 10 Aug 2023 03:07:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
