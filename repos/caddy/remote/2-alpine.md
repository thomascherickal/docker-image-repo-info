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
