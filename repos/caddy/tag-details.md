<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `caddy`

-	[`caddy:2`](#caddy2)
-	[`caddy:2.1.1`](#caddy211)
-	[`caddy:2.1.1-alpine`](#caddy211-alpine)
-	[`caddy:2.1.1-builder`](#caddy211-builder)
-	[`caddy:2.1.1-windowsservercore`](#caddy211-windowsservercore)
-	[`caddy:2.1.1-windowsservercore-1809`](#caddy211-windowsservercore-1809)
-	[`caddy:2.1.1-windowsservercore-ltsc2016`](#caddy211-windowsservercore-ltsc2016)
-	[`caddy:2-alpine`](#caddy2-alpine)
-	[`caddy:2-builder`](#caddy2-builder)
-	[`caddy:2-windowsservercore`](#caddy2-windowsservercore)
-	[`caddy:2-windowsservercore-1809`](#caddy2-windowsservercore-1809)
-	[`caddy:2-windowsservercore-ltsc2016`](#caddy2-windowsservercore-ltsc2016)
-	[`caddy:alpine`](#caddyalpine)
-	[`caddy:builder`](#caddybuilder)
-	[`caddy:latest`](#caddylatest)
-	[`caddy:windowsservercore`](#caddywindowsservercore)
-	[`caddy:windowsservercore-1809`](#caddywindowsservercore-1809)
-	[`caddy:windowsservercore-ltsc2016`](#caddywindowsservercore-ltsc2016)

## `caddy:2`

```console
$ docker pull caddy@sha256:9ee709b080aacb1a5cae6c4cb654d950f1ded75d7a2277a792860bb28134158e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1282; amd64
	-	windows version 10.0.14393.3750; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:4ebb2f65ffef1445e2bcf137fc482fb212994bdb13b1868d750676725e7cf443
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16498000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a737824e95f5dac6216b82956d982715f24a48b766894844b1a6a607c2375027`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:21:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 21:21:16 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 21:21:18 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 20:19:29 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:19:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 20:19:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 20:19:33 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 20:19:33 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 20:19:33 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 20:19:33 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 20:19:34 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 20:19:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 20:19:34 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 20:19:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 20:19:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 20:19:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 20:19:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 20:19:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 20:19:35 GMT
EXPOSE 80
# Mon, 29 Jun 2020 20:19:35 GMT
EXPOSE 443
# Mon, 29 Jun 2020 20:19:35 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 20:19:36 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 20:19:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed237faf7b90187b720d5e863fb021a1ca678304744dad14ff8ad6434e4e1da`  
		Last Modified: Mon, 15 Jun 2020 21:22:02 GMT  
		Size: 300.0 KB (299981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e49a2f7ba4b80caa31bb2874b39f9c4bbb447708f3a0e07ff43892744e63a4`  
		Last Modified: Mon, 15 Jun 2020 21:22:02 GMT  
		Size: 5.8 KB (5767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc737685e2c14b5fdd7d0988d75baaf51de1353bc59127eebf7be1b496a02f9`  
		Last Modified: Mon, 29 Jun 2020 20:20:10 GMT  
		Size: 13.4 MB (13394558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba35373e6dd60c32e3ee0c3336ea77052d4cf981bed1cfd7a8f6b1e2fdf6f1cd`  
		Last Modified: Mon, 29 Jun 2020 20:20:07 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:cf35a85f26269ab62adfe126d4669c6951ec6bb9ff26fe21cfd494aff1d2d3d4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.6 MB (15646628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55d1456582127518b50a7cca33e619677857b0dee80fe88ff99e35ef84d53468`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:52:06 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 20:52:07 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 20:52:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 19:49:31 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:49:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 19:49:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 19:49:45 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 19:49:46 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 19:49:46 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 19:49:47 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 19:49:47 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 19:49:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 19:49:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 19:49:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 19:49:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 19:49:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 19:49:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 19:49:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 19:49:52 GMT
EXPOSE 80
# Mon, 29 Jun 2020 19:49:53 GMT
EXPOSE 443
# Mon, 29 Jun 2020 19:49:53 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 19:49:54 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 19:49:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2a5a47b7ff29cc165cee9824ba874fa6cb56d737ce18f841fc3ed5e937cb75`  
		Last Modified: Mon, 15 Jun 2020 20:54:38 GMT  
		Size: 300.1 KB (300144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3243ce9c25dc28a597c553cc7f0d4816c4b75789e4ebc37225ac58d5bd078995`  
		Last Modified: Mon, 15 Jun 2020 20:54:38 GMT  
		Size: 5.8 KB (5842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e9f25f4ff5c7a540a28a538f1a268137ec941f2be720b1bb5a284f588131f9`  
		Last Modified: Mon, 29 Jun 2020 19:52:00 GMT  
		Size: 12.7 MB (12737203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363d05163dedef9589519a417c89106201dbedc9dfe6b122a9eaa60ab2885a1f`  
		Last Modified: Mon, 29 Jun 2020 19:51:56 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:d370dd37d66b0814addc5114c3b4be7e42c00bfa90501c6497c8765a4036fa40
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15427533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7d7e451c4983b297ee7dbcda3b2334193679fcf011df665e95933aa8c27a260`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:59:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 21:00:00 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 21:00:03 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 19:57:29 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:57:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 19:57:42 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 19:57:43 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 19:57:44 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 19:57:44 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 19:57:45 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 19:57:46 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 19:57:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 19:57:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 19:57:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 19:57:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 19:57:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 19:57:50 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 19:57:50 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 19:57:51 GMT
EXPOSE 80
# Mon, 29 Jun 2020 19:57:52 GMT
EXPOSE 443
# Mon, 29 Jun 2020 19:57:52 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 19:57:53 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 19:57:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2aa34f01f2f9112772fdaebe7083b7dcdb4313768e0d6533a3e5b99597c98d`  
		Last Modified: Mon, 15 Jun 2020 21:02:12 GMT  
		Size: 299.2 KB (299237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b107a7bf1560d80dcded532795715f77765cf1a3d9464665d42acab82d366e`  
		Last Modified: Mon, 15 Jun 2020 21:02:12 GMT  
		Size: 5.8 KB (5845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a9aae216c1bc5bb511c635b06620b9537a354f011671c718d62e1f0cdd1e55`  
		Last Modified: Mon, 29 Jun 2020 19:59:29 GMT  
		Size: 12.7 MB (12715535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e31bd59a84cad62fcf351b80ea45db935206ee2a53dc6c6755a05a3a56b350a`  
		Last Modified: Mon, 29 Jun 2020 19:59:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7bae42d1c40f55e4406c24be4cbf0980dd87ab27d4e0cff6a5dddbea55aabca2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15324730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5794c058f0b994dcd4698e866d7db6dafc76f0cb9be4a1262eb893314a6176a9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:42:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 20:42:33 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 20:42:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 19:40:19 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:40:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 19:40:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 19:40:27 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 19:40:28 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 19:40:28 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 19:40:29 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 19:40:29 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 19:40:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 19:40:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 19:40:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 19:40:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 19:40:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 19:40:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 19:40:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 19:40:35 GMT
EXPOSE 80
# Mon, 29 Jun 2020 19:40:36 GMT
EXPOSE 443
# Mon, 29 Jun 2020 19:40:37 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 19:40:38 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 19:40:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f33282aee1a51127f669c7222e26bd0d5107b28d68819a6ead7f68076a73dc`  
		Last Modified: Mon, 15 Jun 2020 20:44:05 GMT  
		Size: 300.4 KB (300393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b85f4621f67650b74dc2db70b30f9593bc6695d3e91ff3899b3ee7c34cffc04`  
		Last Modified: Mon, 15 Jun 2020 20:44:04 GMT  
		Size: 5.8 KB (5846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f2cff8627bb2fbb4a0a0b9f9b57936ec53447aa2d2de70f1b7a5381acede31`  
		Last Modified: Mon, 29 Jun 2020 19:41:45 GMT  
		Size: 12.3 MB (12310372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934573df7ec7ebf99ab90bd97aa562d53dc3334ebdad1cc27970c48352809d2b`  
		Last Modified: Mon, 29 Jun 2020 19:41:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:382970b5cca83435fda7ec524c4e55f6f3eac245fa3ba70d1436b430995a9ef8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15188949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98bd39661b7c63c2701d172a8d747148274c11c8866b67a0a95036c34d95c8c8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:19:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 21:19:13 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 21:19:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 20:17:08 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:17:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 20:17:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 20:17:29 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 20:17:31 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 20:17:34 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 20:17:38 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 20:17:41 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 20:17:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 20:17:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 20:17:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 20:17:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 20:18:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 20:18:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 20:18:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 20:18:10 GMT
EXPOSE 80
# Mon, 29 Jun 2020 20:18:13 GMT
EXPOSE 443
# Mon, 29 Jun 2020 20:18:16 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 20:18:20 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 20:18:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b28df4c8a155654ad705e08f459bd177acc1005644ce2173ac62e954d6d4d2`  
		Last Modified: Mon, 15 Jun 2020 21:24:35 GMT  
		Size: 302.4 KB (302369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2288431c86a795754eb4d3a678e778c534a14e9243aea01a7cf9feff8d8e4e`  
		Last Modified: Mon, 15 Jun 2020 21:24:35 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d7ec5c119ab9881df3cbd4ba6b7b5c760c3b2ba149852fd430ff4cb8381c9a`  
		Last Modified: Mon, 29 Jun 2020 20:21:56 GMT  
		Size: 12.1 MB (12075379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788a23ed056849a1dc58fd563a9f8e0827e3f16678c61af3495f2a751cdf718d`  
		Last Modified: Mon, 29 Jun 2020 20:21:53 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:31dbbca225902439b42fd9e804440b767a810c638671193051eb0e47dd8af357
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (16040684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:589941f612353f33545544e2621a4a8fc31e28b78dd33543b2a7b3b5a5f7d09d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:43:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 20:43:15 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 20:43:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 19:41:26 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:41:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 19:41:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 19:41:30 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 19:41:30 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 19:41:30 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 19:41:30 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 19:41:31 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 19:41:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 19:41:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 19:41:31 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 19:41:31 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 19:41:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 19:41:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 19:41:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 19:41:32 GMT
EXPOSE 80
# Mon, 29 Jun 2020 19:41:32 GMT
EXPOSE 443
# Mon, 29 Jun 2020 19:41:33 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 19:41:33 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 19:41:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc47bdcaea173dfb029a09265c41846030477dc696b22fed52acad2b2078bb7`  
		Last Modified: Mon, 15 Jun 2020 20:44:21 GMT  
		Size: 300.5 KB (300524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf084f3ceb3b3b1196400fa251cc45e01de7ece41b7605bb40ae5178d849b47d`  
		Last Modified: Mon, 15 Jun 2020 20:44:26 GMT  
		Size: 5.8 KB (5841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236e43429060d4faebd33793542b4580546354f9e942339b380a69c0d1ebc94a`  
		Last Modified: Mon, 29 Jun 2020 19:42:20 GMT  
		Size: 13.2 MB (13167975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c83d9fdfe57ad6eda493263027564db3f25c9b58a45c2afaf3738e6ccb6e452`  
		Last Modified: Mon, 29 Jun 2020 19:42:19 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:e8b1865dd51a79cddf1ce786b52156e81cbaf67046a24bd475a8115ab960445c
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2312693391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ddbcd3c45a5583a6c9b91d6672b879ac5fd94c25a88540d6ca81b52c37931de`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Tue, 09 Jun 2020 22:33:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:02:29 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:03:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 29 Jun 2020 20:14:27 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:14:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('360bade38fea4d0e87bf00f2dc0c7e7b4434bb020af49d189b2c424246710bf6a3074e486ef2c3d6994473bcd62393302a1a704c215b4e323eeaecbfa359a533')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 29 Jun 2020 20:15:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 29 Jun 2020 20:15:02 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 29 Jun 2020 20:15:03 GMT
VOLUME [c:/config]
# Mon, 29 Jun 2020 20:15:04 GMT
VOLUME [c:/data]
# Mon, 29 Jun 2020 20:15:05 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 20:15:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 20:15:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 20:15:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 20:15:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 20:15:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 20:15:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 20:15:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 20:15:11 GMT
EXPOSE 80
# Mon, 29 Jun 2020 20:15:12 GMT
EXPOSE 443
# Mon, 29 Jun 2020 20:15:13 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 20:15:29 GMT
RUN caddy version
# Mon, 29 Jun 2020 20:15:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f841c6a0c622cd36b5b2688011a224ac3e8e96273758f4a2804f2f3f099f267d`  
		Last Modified: Tue, 09 Jun 2020 23:17:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e676deb3766189ea2b008f69205017c9ee31a77f9c7001fb5a07fb2e2d4fbb0`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba576338ed5242ba3fb838ce5fa930abb61e22fc422ba46b260dbca773cb9`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 4.8 MB (4772911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723eab0814ebbb502654a889ac99b52f2f7cb218a7164887ad0c9a1a5634d191`  
		Last Modified: Mon, 29 Jun 2020 20:18:31 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d3ac5a82f61292731263eecfe0635a4e0b486dd7f7f843a5cf9c1962fb54f1`  
		Last Modified: Mon, 29 Jun 2020 20:18:34 GMT  
		Size: 13.7 MB (13685965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18990846d9f6b2e03b43f0c42307982b5d13426a8d003425ce98e88c1ee61e9e`  
		Last Modified: Mon, 29 Jun 2020 20:18:30 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd85b14725d34f8e3d6505a3730098d0d983c7bfc436fab9f0025e28ea413c9`  
		Last Modified: Mon, 29 Jun 2020 20:18:30 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c83ec7d2b6fe2d3beb4121b8691686945da20d9398144840e2699dd7352378`  
		Last Modified: Mon, 29 Jun 2020 20:18:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7205b75fee4bcd79e0441081d0c18f4f16c9e3faddfbe44e9a2017d9c98e12`  
		Last Modified: Mon, 29 Jun 2020 20:18:29 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2d684094d65ac89815f73d6bb42fcc037bb91d14788f39d7c874f923010f78`  
		Last Modified: Mon, 29 Jun 2020 20:18:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d345ee36ca73380ffc59a00a9f9645c4be0f97bd3450083d5105bfb2456e5379`  
		Last Modified: Mon, 29 Jun 2020 20:18:27 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1399cf9fea037f4b40be192761883219e66d7fac0e8a7e53707b63894fd9a0a`  
		Last Modified: Mon, 29 Jun 2020 20:18:27 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abd79214efe888d78b44116335a0015f91de32819741eba80d9523b930ea548`  
		Last Modified: Mon, 29 Jun 2020 20:18:26 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1ac2c904ffff4f7f0d926f3fedbd61527aaf55aa38e88cde26c9d568962975`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108a4ea5a1055078abaa7e068c8d881cf36e81204a33175caff409d43aa0c9ce`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6c57249f136d38f7aa1045a8956c4f5f4c3f50d93bfb010221f45219da7dd5`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dec9ff0349ee91649d28733494db17d02470cf6a73f8268d7f3e717bb52f90`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c09a8d6df681bb92ae4ee08eb66e50aa8636527ebad60c50ee3917dd252a97`  
		Last Modified: Mon, 29 Jun 2020 20:18:22 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3888338b94e4b7f8a0a2eeb0c1724e90d743bddbbda11b28ed6a436cc0acc571`  
		Last Modified: Mon, 29 Jun 2020 20:18:22 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6ef034637a0be1fc8331c80eceeaba597da0bda3d9bb9769fde9678f401e9d`  
		Last Modified: Mon, 29 Jun 2020 20:18:22 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e84984fd0f42956c1dc9d31717a9fada1dfdf8e2cb00ce952e2655bf25249ce`  
		Last Modified: Mon, 29 Jun 2020 20:18:23 GMT  
		Size: 298.4 KB (298450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b4fdef44f059a30624268d4a303dc4436aada1655b41b5380dcdf6a1b925a7`  
		Last Modified: Mon, 29 Jun 2020 20:18:23 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:c9cc0726f345f76e464e535e972374668d02c30c224057e4f82e4186ae942ba6
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758382605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:150ecdbd7cbd511f1549e36fab065abcf44446cf7fcd58e45ceef61df883bf2b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:04:40 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:06:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 29 Jun 2020 20:15:40 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:17:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('360bade38fea4d0e87bf00f2dc0c7e7b4434bb020af49d189b2c424246710bf6a3074e486ef2c3d6994473bcd62393302a1a704c215b4e323eeaecbfa359a533')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 29 Jun 2020 20:17:05 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 29 Jun 2020 20:17:06 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 29 Jun 2020 20:17:07 GMT
VOLUME [c:/config]
# Mon, 29 Jun 2020 20:17:08 GMT
VOLUME [c:/data]
# Mon, 29 Jun 2020 20:17:09 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 20:17:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 20:17:11 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 20:17:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 20:17:12 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 20:17:13 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 20:17:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 20:17:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 20:17:16 GMT
EXPOSE 80
# Mon, 29 Jun 2020 20:17:17 GMT
EXPOSE 443
# Mon, 29 Jun 2020 20:17:18 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 20:17:58 GMT
RUN caddy version
# Mon, 29 Jun 2020 20:17:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22985925139cd6a6e83b6eb5286a8a6e1053a5c6ddd9762f34deea2aa6bcaacc`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43c028d6768e901bc64b3edb7e2e5f72050d3ed78ea4e7337fe85725d250c15`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 5.4 MB (5404509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae58d77a8d67f842374c3e60732465a9aaddfd9ce2b054b39aac0b7f2a420d0f`  
		Last Modified: Mon, 29 Jun 2020 20:18:56 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f76df30f6b9698ddedad69790139a9d2cf4fc871763691861f8aab018ac8ed`  
		Last Modified: Mon, 29 Jun 2020 20:19:01 GMT  
		Size: 18.7 MB (18718943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf3b4f088973e051021b74d9b9f795a9f2c8c71f7ae83e83f0cd6e95343f562`  
		Last Modified: Mon, 29 Jun 2020 20:18:56 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef3ce431d20a03b531eadce4cbe5680aca6c4ee4e24d70578687c89963b41d1`  
		Last Modified: Mon, 29 Jun 2020 20:18:55 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091019db4f4b75fe37b7b7ce991db4c4b02422388f836be3c4eb7c51159208b3`  
		Last Modified: Mon, 29 Jun 2020 20:18:54 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e080558fbf5cadbed8b34080d8bad08b45fff65ab533d87a24639d3ba6fd837f`  
		Last Modified: Mon, 29 Jun 2020 20:18:54 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc66481244327f616ca39ffe8c4b596d1aa9b7d778aa717e75b0b8f4a4c06350`  
		Last Modified: Mon, 29 Jun 2020 20:18:54 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f6e5557d697d57716bbf495fc701cef5b9073dbe5646f64fbbb0b8207fc07a`  
		Last Modified: Mon, 29 Jun 2020 20:18:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e238dae9de9d36d2c73796aa4c2a29645bbd5239ab47082579ccdc42e76244d8`  
		Last Modified: Mon, 29 Jun 2020 20:18:53 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbccba413742cc92bb8c53edd613f0be0250226ae8465165c5bc4e25a0c79a0`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911208ad8ab28008b96820a6251bee291bb5840e23ec782b1bbafdfe8019e08c`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2440198b129a0383b522e8b349ec26d2b66b1b33c422df3c3933be7c6591f661`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa72d9c6b7293c4d60c48fc5729c6f3a7eaa2f8276c8cba94bbb20edab126354`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a35778894255e6ba11c0d42ca54c80e69279c8777b609c7366208de7e0ac4c`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b99c2dfe7b1a527300bd8de8147e159f8ecdbab796e7a71c7dd3e2df8cf216`  
		Last Modified: Mon, 29 Jun 2020 20:18:48 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9969646e605208d0301ec4741756dd6257ac0991ed01bfde817b513b8e7a9e19`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2919689d5a48dd6e4ef39397ffed789e7ff54451a9abaadbc274574a363256e`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfa5d572d4b3ac461e8246a58be6e84431cc733d430cb532e99e83af335ded3`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 239.7 KB (239740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90df7192caf1a86dbf2f53b57375af83ea514b4128fc8040808368b6ae7fd815`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1`

**does not exist** (yet?)

## `caddy:2.1.1-alpine`

**does not exist** (yet?)

## `caddy:2.1.1-builder`

**does not exist** (yet?)

## `caddy:2.1.1-windowsservercore`

**does not exist** (yet?)

## `caddy:2.1.1-windowsservercore-1809`

**does not exist** (yet?)

## `caddy:2.1.1-windowsservercore-ltsc2016`

**does not exist** (yet?)

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:76f1223d447df304172b1f8a6d22f70d2e43afd276ca0e107513e958d8629ded
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:4ebb2f65ffef1445e2bcf137fc482fb212994bdb13b1868d750676725e7cf443
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16498000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a737824e95f5dac6216b82956d982715f24a48b766894844b1a6a607c2375027`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:21:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 21:21:16 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 21:21:18 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 20:19:29 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:19:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 20:19:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 20:19:33 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 20:19:33 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 20:19:33 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 20:19:33 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 20:19:34 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 20:19:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 20:19:34 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 20:19:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 20:19:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 20:19:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 20:19:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 20:19:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 20:19:35 GMT
EXPOSE 80
# Mon, 29 Jun 2020 20:19:35 GMT
EXPOSE 443
# Mon, 29 Jun 2020 20:19:35 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 20:19:36 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 20:19:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed237faf7b90187b720d5e863fb021a1ca678304744dad14ff8ad6434e4e1da`  
		Last Modified: Mon, 15 Jun 2020 21:22:02 GMT  
		Size: 300.0 KB (299981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e49a2f7ba4b80caa31bb2874b39f9c4bbb447708f3a0e07ff43892744e63a4`  
		Last Modified: Mon, 15 Jun 2020 21:22:02 GMT  
		Size: 5.8 KB (5767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc737685e2c14b5fdd7d0988d75baaf51de1353bc59127eebf7be1b496a02f9`  
		Last Modified: Mon, 29 Jun 2020 20:20:10 GMT  
		Size: 13.4 MB (13394558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba35373e6dd60c32e3ee0c3336ea77052d4cf981bed1cfd7a8f6b1e2fdf6f1cd`  
		Last Modified: Mon, 29 Jun 2020 20:20:07 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:cf35a85f26269ab62adfe126d4669c6951ec6bb9ff26fe21cfd494aff1d2d3d4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.6 MB (15646628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55d1456582127518b50a7cca33e619677857b0dee80fe88ff99e35ef84d53468`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:52:06 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 20:52:07 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 20:52:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 19:49:31 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:49:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 19:49:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 19:49:45 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 19:49:46 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 19:49:46 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 19:49:47 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 19:49:47 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 19:49:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 19:49:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 19:49:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 19:49:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 19:49:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 19:49:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 19:49:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 19:49:52 GMT
EXPOSE 80
# Mon, 29 Jun 2020 19:49:53 GMT
EXPOSE 443
# Mon, 29 Jun 2020 19:49:53 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 19:49:54 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 19:49:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2a5a47b7ff29cc165cee9824ba874fa6cb56d737ce18f841fc3ed5e937cb75`  
		Last Modified: Mon, 15 Jun 2020 20:54:38 GMT  
		Size: 300.1 KB (300144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3243ce9c25dc28a597c553cc7f0d4816c4b75789e4ebc37225ac58d5bd078995`  
		Last Modified: Mon, 15 Jun 2020 20:54:38 GMT  
		Size: 5.8 KB (5842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e9f25f4ff5c7a540a28a538f1a268137ec941f2be720b1bb5a284f588131f9`  
		Last Modified: Mon, 29 Jun 2020 19:52:00 GMT  
		Size: 12.7 MB (12737203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363d05163dedef9589519a417c89106201dbedc9dfe6b122a9eaa60ab2885a1f`  
		Last Modified: Mon, 29 Jun 2020 19:51:56 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:d370dd37d66b0814addc5114c3b4be7e42c00bfa90501c6497c8765a4036fa40
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15427533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7d7e451c4983b297ee7dbcda3b2334193679fcf011df665e95933aa8c27a260`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:59:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 21:00:00 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 21:00:03 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 19:57:29 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:57:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 19:57:42 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 19:57:43 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 19:57:44 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 19:57:44 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 19:57:45 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 19:57:46 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 19:57:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 19:57:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 19:57:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 19:57:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 19:57:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 19:57:50 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 19:57:50 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 19:57:51 GMT
EXPOSE 80
# Mon, 29 Jun 2020 19:57:52 GMT
EXPOSE 443
# Mon, 29 Jun 2020 19:57:52 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 19:57:53 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 19:57:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2aa34f01f2f9112772fdaebe7083b7dcdb4313768e0d6533a3e5b99597c98d`  
		Last Modified: Mon, 15 Jun 2020 21:02:12 GMT  
		Size: 299.2 KB (299237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b107a7bf1560d80dcded532795715f77765cf1a3d9464665d42acab82d366e`  
		Last Modified: Mon, 15 Jun 2020 21:02:12 GMT  
		Size: 5.8 KB (5845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a9aae216c1bc5bb511c635b06620b9537a354f011671c718d62e1f0cdd1e55`  
		Last Modified: Mon, 29 Jun 2020 19:59:29 GMT  
		Size: 12.7 MB (12715535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e31bd59a84cad62fcf351b80ea45db935206ee2a53dc6c6755a05a3a56b350a`  
		Last Modified: Mon, 29 Jun 2020 19:59:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7bae42d1c40f55e4406c24be4cbf0980dd87ab27d4e0cff6a5dddbea55aabca2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15324730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5794c058f0b994dcd4698e866d7db6dafc76f0cb9be4a1262eb893314a6176a9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:42:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 20:42:33 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 20:42:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 19:40:19 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:40:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 19:40:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 19:40:27 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 19:40:28 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 19:40:28 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 19:40:29 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 19:40:29 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 19:40:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 19:40:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 19:40:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 19:40:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 19:40:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 19:40:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 19:40:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 19:40:35 GMT
EXPOSE 80
# Mon, 29 Jun 2020 19:40:36 GMT
EXPOSE 443
# Mon, 29 Jun 2020 19:40:37 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 19:40:38 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 19:40:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f33282aee1a51127f669c7222e26bd0d5107b28d68819a6ead7f68076a73dc`  
		Last Modified: Mon, 15 Jun 2020 20:44:05 GMT  
		Size: 300.4 KB (300393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b85f4621f67650b74dc2db70b30f9593bc6695d3e91ff3899b3ee7c34cffc04`  
		Last Modified: Mon, 15 Jun 2020 20:44:04 GMT  
		Size: 5.8 KB (5846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f2cff8627bb2fbb4a0a0b9f9b57936ec53447aa2d2de70f1b7a5381acede31`  
		Last Modified: Mon, 29 Jun 2020 19:41:45 GMT  
		Size: 12.3 MB (12310372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934573df7ec7ebf99ab90bd97aa562d53dc3334ebdad1cc27970c48352809d2b`  
		Last Modified: Mon, 29 Jun 2020 19:41:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:382970b5cca83435fda7ec524c4e55f6f3eac245fa3ba70d1436b430995a9ef8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15188949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98bd39661b7c63c2701d172a8d747148274c11c8866b67a0a95036c34d95c8c8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:19:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 21:19:13 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 21:19:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 20:17:08 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:17:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 20:17:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 20:17:29 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 20:17:31 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 20:17:34 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 20:17:38 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 20:17:41 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 20:17:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 20:17:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 20:17:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 20:17:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 20:18:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 20:18:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 20:18:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 20:18:10 GMT
EXPOSE 80
# Mon, 29 Jun 2020 20:18:13 GMT
EXPOSE 443
# Mon, 29 Jun 2020 20:18:16 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 20:18:20 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 20:18:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b28df4c8a155654ad705e08f459bd177acc1005644ce2173ac62e954d6d4d2`  
		Last Modified: Mon, 15 Jun 2020 21:24:35 GMT  
		Size: 302.4 KB (302369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2288431c86a795754eb4d3a678e778c534a14e9243aea01a7cf9feff8d8e4e`  
		Last Modified: Mon, 15 Jun 2020 21:24:35 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d7ec5c119ab9881df3cbd4ba6b7b5c760c3b2ba149852fd430ff4cb8381c9a`  
		Last Modified: Mon, 29 Jun 2020 20:21:56 GMT  
		Size: 12.1 MB (12075379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788a23ed056849a1dc58fd563a9f8e0827e3f16678c61af3495f2a751cdf718d`  
		Last Modified: Mon, 29 Jun 2020 20:21:53 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:31dbbca225902439b42fd9e804440b767a810c638671193051eb0e47dd8af357
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (16040684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:589941f612353f33545544e2621a4a8fc31e28b78dd33543b2a7b3b5a5f7d09d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:43:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 20:43:15 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 20:43:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 19:41:26 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:41:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 19:41:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 19:41:30 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 19:41:30 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 19:41:30 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 19:41:30 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 19:41:31 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 19:41:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 19:41:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 19:41:31 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 19:41:31 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 19:41:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 19:41:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 19:41:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 19:41:32 GMT
EXPOSE 80
# Mon, 29 Jun 2020 19:41:32 GMT
EXPOSE 443
# Mon, 29 Jun 2020 19:41:33 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 19:41:33 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 19:41:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc47bdcaea173dfb029a09265c41846030477dc696b22fed52acad2b2078bb7`  
		Last Modified: Mon, 15 Jun 2020 20:44:21 GMT  
		Size: 300.5 KB (300524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf084f3ceb3b3b1196400fa251cc45e01de7ece41b7605bb40ae5178d849b47d`  
		Last Modified: Mon, 15 Jun 2020 20:44:26 GMT  
		Size: 5.8 KB (5841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236e43429060d4faebd33793542b4580546354f9e942339b380a69c0d1ebc94a`  
		Last Modified: Mon, 29 Jun 2020 19:42:20 GMT  
		Size: 13.2 MB (13167975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c83d9fdfe57ad6eda493263027564db3f25c9b58a45c2afaf3738e6ccb6e452`  
		Last Modified: Mon, 29 Jun 2020 19:42:19 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:e455aded5df9a8ebb35447ab864c1426f80ee6f807c66d1e61ffeb00bea1889e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:174f4aac00feefebff6adf98c35b9d83f92e8b1b83e2fda9316d7747a7cd0f15
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.0 MB (333987526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41fdef47036e115062adce80689ad61ccb2b9cd17b0893c0a02eec8b638b8d43`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:30:20 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:32:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:32:35 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:32:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:32:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:32:36 GMT
WORKDIR /go
# Mon, 15 Jun 2020 21:21:27 GMT
WORKDIR /src
# Mon, 15 Jun 2020 21:21:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 29 Jun 2020 20:19:40 GMT
ENV CADDY_SOURCE_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:19:42 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Mon, 29 Jun 2020 20:19:42 GMT
WORKDIR /src/caddy/cmd/caddy
# Mon, 29 Jun 2020 20:19:56 GMT
RUN go get -d ./...
# Mon, 29 Jun 2020 20:19:57 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Mon, 29 Jun 2020 20:19:57 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0cccf56431698a0981b191f61dcb4ba6afa272d35deb14eaccf2cb46ed0f9d`  
		Last Modified: Tue, 02 Jun 2020 01:44:38 GMT  
		Size: 132.1 MB (132120859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbe0275821fc905c0321a44449b7ca670963f2cc0824150bea2125dee8dc7376`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8183c72c683b23caab534e2ddeef5f4a54ed1040c87f05484e0248e21bb74954`  
		Last Modified: Mon, 15 Jun 2020 21:22:10 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404f93ac2221d032b0fca7fdb3d4bc6d9156768ffc95251e0607652cfbecc8b8`  
		Last Modified: Mon, 15 Jun 2020 21:22:10 GMT  
		Size: 8.3 MB (8309926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603c90769f39a502c786ab7eee221293be6835a473c3d9aaa621afa6068b5ee8`  
		Last Modified: Mon, 29 Jun 2020 20:20:16 GMT  
		Size: 3.1 MB (3057920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a0952b6cb77878a7141da63ee7ec7a0786849b87f81eb46f22f9be090e94b6`  
		Last Modified: Mon, 29 Jun 2020 20:20:38 GMT  
		Size: 187.4 MB (187417642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8a394faab9ec441308fbf55d2e542c297e7c61a9f3ae3ad6658c8e110d187a`  
		Last Modified: Mon, 29 Jun 2020 20:20:15 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3a8152559323a4cf8eb3ef0ca03307062d34e3a5ba24bbd517d6c64f9a96b2`  
		Last Modified: Mon, 29 Jun 2020 20:20:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:9d7661f3789c9c9d95cd0afa4026a4954b638757c0d1350694b8d9e7f71c8307
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.5 MB (329510925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e2f7767b3f46ec3fcde26b3dd823bd3bc05cefd8b63107be285e238972844df`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:02:10 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 02:02:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 02:02:29 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 02:55:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 02:56:02 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 02:56:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 02:56:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 02:56:07 GMT
WORKDIR /go
# Mon, 15 Jun 2020 20:52:46 GMT
WORKDIR /src
# Mon, 15 Jun 2020 20:52:50 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 29 Jun 2020 19:50:02 GMT
ENV CADDY_SOURCE_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:50:06 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Mon, 29 Jun 2020 19:50:06 GMT
WORKDIR /src/caddy/cmd/caddy
# Mon, 29 Jun 2020 19:51:25 GMT
RUN go get -d ./...
# Mon, 29 Jun 2020 19:51:33 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Mon, 29 Jun 2020 19:51:34 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c276dc457bae632c9eadd1ac69c1a756a9a67e050b0350a475b19663722191cf`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 282.8 KB (282778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f0819b703e39c232c6d0a8ac0f76d8f3c6856629db16fd6dd7b7ae69368281`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e66763a2c2fd4a68d63d58e30f372cf4ebdc811274c6979d891e5e0cb676d73`  
		Last Modified: Tue, 02 Jun 2020 05:22:08 GMT  
		Size: 128.2 MB (128209215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7367c813a205e4503e365f0492c4c2de22baead5b600a620d362655aa9cd483`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce88b922cbeaa0f67211b29ad7ed76847d7725e329cc620ff7dcc9257fba77e3`  
		Last Modified: Mon, 15 Jun 2020 20:54:49 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720f093e5ede770f019c0c7a14a3361e9648d5b00f7a171f8feaefab719955aa`  
		Last Modified: Mon, 15 Jun 2020 20:54:50 GMT  
		Size: 7.9 MB (7928846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f025440c9236e5025567778b1c12077fb848a31569134c04c8b3cc35245700d`  
		Last Modified: Mon, 29 Jun 2020 19:52:07 GMT  
		Size: 3.1 MB (3058957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8344d190141f30e1aae92a5b7895c902dce5118a7f926ef5d5dfabb338077de8`  
		Last Modified: Mon, 29 Jun 2020 19:52:56 GMT  
		Size: 187.4 MB (187426715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db33b81f00857c93719b9256ab96b7c1d0ea8a69d3f3e32849ac07e97929cc9`  
		Last Modified: Mon, 29 Jun 2020 19:52:07 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f108514bdcdf3896865f08d980a37ab7cd19cb828c0b2221a5e5c2e5b5200c`  
		Last Modified: Mon, 29 Jun 2020 19:52:07 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a7788f8eef0de32ff4ee764adb2b1a35290eb353f19e345958f35df232d16acc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.2 MB (328162638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5546f695708008cd952d145b679402d539b3f8552695b15d4a0f8afa2e72cfee`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:10:58 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:11:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:11:01 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:34:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:34:38 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:34:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:34:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:34:44 GMT
WORKDIR /go
# Mon, 15 Jun 2020 21:00:34 GMT
WORKDIR /src
# Mon, 15 Jun 2020 21:00:37 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 29 Jun 2020 19:58:00 GMT
ENV CADDY_SOURCE_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:58:03 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Mon, 29 Jun 2020 19:58:04 GMT
WORKDIR /src/caddy/cmd/caddy
# Mon, 29 Jun 2020 19:59:01 GMT
RUN go get -d ./...
# Mon, 29 Jun 2020 19:59:07 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Mon, 29 Jun 2020 19:59:08 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512c25ce227edddad11326504a9bab47e83f8b61c090c9dc95882452984ac62`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 281.9 KB (281892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87928ee7e6c788309b46621e351321410e4dde5374869ffa75f404b19e0e0c12`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754691c4bcf20eb06087104e5fc82d340991d9bf26c21cae6979f36e3bd38ca7`  
		Last Modified: Tue, 02 Jun 2020 03:52:16 GMT  
		Size: 127.8 MB (127846663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63238be1b74c86ab98841c3959a33d79a903d58ac50518d4fa65b2ea8c6a75ba`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a1abd4bf80876cf553a554662e0cb3c5c310601b937ee7749c6f828de9dfea`  
		Last Modified: Mon, 15 Jun 2020 21:02:23 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac591f152779d4cfd93fb1e2f29dfeb27073f3559e8cb0daf8ee5c6f58310dc`  
		Last Modified: Mon, 15 Jun 2020 21:02:23 GMT  
		Size: 7.1 MB (7144878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e0594bfc9d580f4e451d7cbb01f558bfe98432dd6ee33eb4a443825ac46449`  
		Last Modified: Mon, 29 Jun 2020 19:59:36 GMT  
		Size: 3.1 MB (3058990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08a2552e8b69f86ac9b9c6958b9ee45d37e3d8c2a5d693fa7040f93fecb1af7`  
		Last Modified: Mon, 29 Jun 2020 20:00:27 GMT  
		Size: 187.4 MB (187422323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae179221c59eb112751c3f996f0ecb537813be0fafd1a4bd1cde75f43575d52`  
		Last Modified: Mon, 29 Jun 2020 19:59:35 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c2ee8d77f04705a1012498984c1060591fb20d309efdec522a25b7fd059680`  
		Last Modified: Mon, 29 Jun 2020 19:59:35 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:9b2e83c1df1c45e57f97c48bdc5d944e64b9fbafe4621f588941f8535c07a05c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.5 MB (328477149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b87b66e72fe48cf1e13cb7c0ca831fddd9b1200500629d508be6de71b386a2d4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:58:16 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 02:00:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 02:00:34 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 02:00:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 02:00:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 02:01:01 GMT
WORKDIR /go
# Mon, 15 Jun 2020 20:42:55 GMT
WORKDIR /src
# Mon, 15 Jun 2020 20:42:58 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 29 Jun 2020 19:40:47 GMT
ENV CADDY_SOURCE_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:40:51 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Mon, 29 Jun 2020 19:40:52 GMT
WORKDIR /src/caddy/cmd/caddy
# Mon, 29 Jun 2020 19:41:20 GMT
RUN go get -d ./...
# Mon, 29 Jun 2020 19:41:27 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Mon, 29 Jun 2020 19:41:28 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a10f6d585c919680bed516e83e217d8bb824ee48306a00ce36c94a2a42e127`  
		Last Modified: Tue, 02 Jun 2020 02:30:00 GMT  
		Size: 126.5 MB (126505030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fdc7971b1eac6baae4423fc0ecca822c4d0372de7bfbdb5a7451e3cdd06be30`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9d4bc6b21331beadc7877a16034ab0b38c0afcf3434fba21ae30649336cb92`  
		Last Modified: Mon, 15 Jun 2020 20:44:13 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebe763a900953fc839be7c307bee96cc4464502cd2cf875941354458648b2b4`  
		Last Modified: Mon, 15 Jun 2020 20:44:13 GMT  
		Size: 8.5 MB (8499921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd27d4d70da701eebdcb2e122f3ba1e8e37426112e12ab1fbbe2e8ee0d6dccd4`  
		Last Modified: Mon, 29 Jun 2020 19:41:52 GMT  
		Size: 3.1 MB (3058980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92f41d7e82ced6444f24c9196af37bc1b89cfcda5a0d73d5a1c46ba7e77282f`  
		Last Modified: Mon, 29 Jun 2020 19:42:30 GMT  
		Size: 187.4 MB (187421128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81ac8d9d1615f457d108d726bb296ebea749e3492e4a639d965461dff718955`  
		Last Modified: Mon, 29 Jun 2020 19:41:51 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e1562a3a569241d3ea907191c7197ea60d84f24a3ed5438c09cfbdea6c4972`  
		Last Modified: Mon, 29 Jun 2020 19:41:51 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:08127eef54ee0f4a65aac670acb12694f8aedc66bfb5f7c5a1117b0932e55b46
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.8 MB (327766267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f38654e854c4d326b17dbe210820d8fec5ce3ed9a388e22bd06ce27693b11eb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:30:00 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:32:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:32:22 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:32:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:32:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:32:46 GMT
WORKDIR /go
# Mon, 15 Jun 2020 21:20:48 GMT
WORKDIR /src
# Mon, 15 Jun 2020 21:20:57 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 29 Jun 2020 20:18:34 GMT
ENV CADDY_SOURCE_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:18:47 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Mon, 29 Jun 2020 20:18:51 GMT
WORKDIR /src/caddy/cmd/caddy
# Mon, 29 Jun 2020 20:21:19 GMT
RUN go get -d ./...
# Mon, 29 Jun 2020 20:21:29 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Mon, 29 Jun 2020 20:21:32 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa9f54e0b14ecd0984863bb950f61bd4bf436b6072e38800e7f963358557067`  
		Last Modified: Tue, 02 Jun 2020 01:48:47 GMT  
		Size: 125.3 MB (125263901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a41edd0480b633d5ed3f00eef305e8a7526c48f1fdde5ef350565830d40609`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca1ca7c0085d0ffb2b0cb1bdabb73af28921fe105ac26bae09acee083eb4c72`  
		Last Modified: Mon, 15 Jun 2020 21:24:51 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55082f384c6dea8e172df520164ab7feeca61be6b9d38ab64bb2265b7f197b1`  
		Last Modified: Mon, 15 Jun 2020 21:24:49 GMT  
		Size: 8.9 MB (8919998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef68f42bbb77bbb1f77ff75b7844f6871222865c01822b3479c9bfacd19afbfe`  
		Last Modified: Mon, 29 Jun 2020 20:22:09 GMT  
		Size: 3.1 MB (3056722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f055e9f88932992a7302c04e8502ad82457b4cca90a5f8da7c67c1a1ce686e5a`  
		Last Modified: Mon, 29 Jun 2020 20:22:36 GMT  
		Size: 187.4 MB (187434281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75cd750be57c01f0ccc6d84c16b2ee317cd5364f7933ff71de5f6d023f04adbd`  
		Last Modified: Mon, 29 Jun 2020 20:22:08 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ccc0213dea3f99dffb64414d611d494f9b129eee3aebcb59ea0e81be9df9f37`  
		Last Modified: Mon, 29 Jun 2020 20:22:07 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:0169dfe70d71f5cf9c35f9947ee054112da43b3baeb7d53fadbb477d901424a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.5 MB (333495213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:270b81fea5e00d9fc31bda2961e13708de4ae9569b09c9a2f89751d01d513703`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:53:16 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:54:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:54:38 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:54:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:54:38 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:54:39 GMT
WORKDIR /go
# Mon, 15 Jun 2020 20:43:26 GMT
WORKDIR /src
# Mon, 15 Jun 2020 20:43:28 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 29 Jun 2020 19:41:38 GMT
ENV CADDY_SOURCE_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:41:39 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Mon, 29 Jun 2020 19:41:40 GMT
WORKDIR /src/caddy/cmd/caddy
# Mon, 29 Jun 2020 19:41:59 GMT
RUN go get -d ./...
# Mon, 29 Jun 2020 19:42:07 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Mon, 29 Jun 2020 19:42:07 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc125fe27a23a8501491445468375e7ea9db946b45cbd911a05a65cfb7c3334`  
		Last Modified: Tue, 02 Jun 2020 02:01:21 GMT  
		Size: 131.8 MB (131814783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7129c3822665192c1533e7d5ab270717e256b1b9844d6fd116852b00a29058e9`  
		Last Modified: Tue, 02 Jun 2020 02:01:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d8d7ec191535d778fe97d9e282050d4140fab1236212ea77816ba1db178bae`  
		Last Modified: Mon, 15 Jun 2020 20:44:32 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a8d11ad8b6daae49f4e16f31468f03664af47d81d6792e5da6fb1eff11ee52`  
		Last Modified: Mon, 15 Jun 2020 20:44:32 GMT  
		Size: 8.4 MB (8352257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8663396503bae3461037b0068a6ef6c9ed511cc92f9e98e9284b59ade05a8b93`  
		Last Modified: Mon, 29 Jun 2020 19:42:26 GMT  
		Size: 3.1 MB (3058958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d136cb87215514845773f75dd169a4cab8b7c8dadbac4a8690a9cb9b92190d`  
		Last Modified: Mon, 29 Jun 2020 19:42:43 GMT  
		Size: 187.4 MB (187418751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb6fcd609f2e3e86d693af70201cbc44718bccd00e80f5d3053a5f642832900`  
		Last Modified: Mon, 29 Jun 2020 19:42:56 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e562fb9f71cf78663817e0f877a55ef56211183920d2840976d4ee2883d29dd`  
		Last Modified: Mon, 29 Jun 2020 19:42:25 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:197b83d529db3ebae4b13cb9079006ad0016f9964e1f1cad639679a2c214af7e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64
	-	windows version 10.0.14393.3750; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:e8b1865dd51a79cddf1ce786b52156e81cbaf67046a24bd475a8115ab960445c
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2312693391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ddbcd3c45a5583a6c9b91d6672b879ac5fd94c25a88540d6ca81b52c37931de`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Tue, 09 Jun 2020 22:33:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:02:29 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:03:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 29 Jun 2020 20:14:27 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:14:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('360bade38fea4d0e87bf00f2dc0c7e7b4434bb020af49d189b2c424246710bf6a3074e486ef2c3d6994473bcd62393302a1a704c215b4e323eeaecbfa359a533')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 29 Jun 2020 20:15:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 29 Jun 2020 20:15:02 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 29 Jun 2020 20:15:03 GMT
VOLUME [c:/config]
# Mon, 29 Jun 2020 20:15:04 GMT
VOLUME [c:/data]
# Mon, 29 Jun 2020 20:15:05 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 20:15:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 20:15:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 20:15:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 20:15:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 20:15:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 20:15:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 20:15:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 20:15:11 GMT
EXPOSE 80
# Mon, 29 Jun 2020 20:15:12 GMT
EXPOSE 443
# Mon, 29 Jun 2020 20:15:13 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 20:15:29 GMT
RUN caddy version
# Mon, 29 Jun 2020 20:15:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f841c6a0c622cd36b5b2688011a224ac3e8e96273758f4a2804f2f3f099f267d`  
		Last Modified: Tue, 09 Jun 2020 23:17:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e676deb3766189ea2b008f69205017c9ee31a77f9c7001fb5a07fb2e2d4fbb0`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba576338ed5242ba3fb838ce5fa930abb61e22fc422ba46b260dbca773cb9`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 4.8 MB (4772911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723eab0814ebbb502654a889ac99b52f2f7cb218a7164887ad0c9a1a5634d191`  
		Last Modified: Mon, 29 Jun 2020 20:18:31 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d3ac5a82f61292731263eecfe0635a4e0b486dd7f7f843a5cf9c1962fb54f1`  
		Last Modified: Mon, 29 Jun 2020 20:18:34 GMT  
		Size: 13.7 MB (13685965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18990846d9f6b2e03b43f0c42307982b5d13426a8d003425ce98e88c1ee61e9e`  
		Last Modified: Mon, 29 Jun 2020 20:18:30 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd85b14725d34f8e3d6505a3730098d0d983c7bfc436fab9f0025e28ea413c9`  
		Last Modified: Mon, 29 Jun 2020 20:18:30 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c83ec7d2b6fe2d3beb4121b8691686945da20d9398144840e2699dd7352378`  
		Last Modified: Mon, 29 Jun 2020 20:18:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7205b75fee4bcd79e0441081d0c18f4f16c9e3faddfbe44e9a2017d9c98e12`  
		Last Modified: Mon, 29 Jun 2020 20:18:29 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2d684094d65ac89815f73d6bb42fcc037bb91d14788f39d7c874f923010f78`  
		Last Modified: Mon, 29 Jun 2020 20:18:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d345ee36ca73380ffc59a00a9f9645c4be0f97bd3450083d5105bfb2456e5379`  
		Last Modified: Mon, 29 Jun 2020 20:18:27 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1399cf9fea037f4b40be192761883219e66d7fac0e8a7e53707b63894fd9a0a`  
		Last Modified: Mon, 29 Jun 2020 20:18:27 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abd79214efe888d78b44116335a0015f91de32819741eba80d9523b930ea548`  
		Last Modified: Mon, 29 Jun 2020 20:18:26 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1ac2c904ffff4f7f0d926f3fedbd61527aaf55aa38e88cde26c9d568962975`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108a4ea5a1055078abaa7e068c8d881cf36e81204a33175caff409d43aa0c9ce`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6c57249f136d38f7aa1045a8956c4f5f4c3f50d93bfb010221f45219da7dd5`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dec9ff0349ee91649d28733494db17d02470cf6a73f8268d7f3e717bb52f90`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c09a8d6df681bb92ae4ee08eb66e50aa8636527ebad60c50ee3917dd252a97`  
		Last Modified: Mon, 29 Jun 2020 20:18:22 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3888338b94e4b7f8a0a2eeb0c1724e90d743bddbbda11b28ed6a436cc0acc571`  
		Last Modified: Mon, 29 Jun 2020 20:18:22 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6ef034637a0be1fc8331c80eceeaba597da0bda3d9bb9769fde9678f401e9d`  
		Last Modified: Mon, 29 Jun 2020 20:18:22 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e84984fd0f42956c1dc9d31717a9fada1dfdf8e2cb00ce952e2655bf25249ce`  
		Last Modified: Mon, 29 Jun 2020 20:18:23 GMT  
		Size: 298.4 KB (298450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b4fdef44f059a30624268d4a303dc4436aada1655b41b5380dcdf6a1b925a7`  
		Last Modified: Mon, 29 Jun 2020 20:18:23 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:c9cc0726f345f76e464e535e972374668d02c30c224057e4f82e4186ae942ba6
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758382605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:150ecdbd7cbd511f1549e36fab065abcf44446cf7fcd58e45ceef61df883bf2b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:04:40 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:06:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 29 Jun 2020 20:15:40 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:17:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('360bade38fea4d0e87bf00f2dc0c7e7b4434bb020af49d189b2c424246710bf6a3074e486ef2c3d6994473bcd62393302a1a704c215b4e323eeaecbfa359a533')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 29 Jun 2020 20:17:05 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 29 Jun 2020 20:17:06 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 29 Jun 2020 20:17:07 GMT
VOLUME [c:/config]
# Mon, 29 Jun 2020 20:17:08 GMT
VOLUME [c:/data]
# Mon, 29 Jun 2020 20:17:09 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 20:17:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 20:17:11 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 20:17:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 20:17:12 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 20:17:13 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 20:17:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 20:17:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 20:17:16 GMT
EXPOSE 80
# Mon, 29 Jun 2020 20:17:17 GMT
EXPOSE 443
# Mon, 29 Jun 2020 20:17:18 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 20:17:58 GMT
RUN caddy version
# Mon, 29 Jun 2020 20:17:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22985925139cd6a6e83b6eb5286a8a6e1053a5c6ddd9762f34deea2aa6bcaacc`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43c028d6768e901bc64b3edb7e2e5f72050d3ed78ea4e7337fe85725d250c15`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 5.4 MB (5404509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae58d77a8d67f842374c3e60732465a9aaddfd9ce2b054b39aac0b7f2a420d0f`  
		Last Modified: Mon, 29 Jun 2020 20:18:56 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f76df30f6b9698ddedad69790139a9d2cf4fc871763691861f8aab018ac8ed`  
		Last Modified: Mon, 29 Jun 2020 20:19:01 GMT  
		Size: 18.7 MB (18718943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf3b4f088973e051021b74d9b9f795a9f2c8c71f7ae83e83f0cd6e95343f562`  
		Last Modified: Mon, 29 Jun 2020 20:18:56 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef3ce431d20a03b531eadce4cbe5680aca6c4ee4e24d70578687c89963b41d1`  
		Last Modified: Mon, 29 Jun 2020 20:18:55 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091019db4f4b75fe37b7b7ce991db4c4b02422388f836be3c4eb7c51159208b3`  
		Last Modified: Mon, 29 Jun 2020 20:18:54 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e080558fbf5cadbed8b34080d8bad08b45fff65ab533d87a24639d3ba6fd837f`  
		Last Modified: Mon, 29 Jun 2020 20:18:54 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc66481244327f616ca39ffe8c4b596d1aa9b7d778aa717e75b0b8f4a4c06350`  
		Last Modified: Mon, 29 Jun 2020 20:18:54 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f6e5557d697d57716bbf495fc701cef5b9073dbe5646f64fbbb0b8207fc07a`  
		Last Modified: Mon, 29 Jun 2020 20:18:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e238dae9de9d36d2c73796aa4c2a29645bbd5239ab47082579ccdc42e76244d8`  
		Last Modified: Mon, 29 Jun 2020 20:18:53 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbccba413742cc92bb8c53edd613f0be0250226ae8465165c5bc4e25a0c79a0`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911208ad8ab28008b96820a6251bee291bb5840e23ec782b1bbafdfe8019e08c`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2440198b129a0383b522e8b349ec26d2b66b1b33c422df3c3933be7c6591f661`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa72d9c6b7293c4d60c48fc5729c6f3a7eaa2f8276c8cba94bbb20edab126354`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a35778894255e6ba11c0d42ca54c80e69279c8777b609c7366208de7e0ac4c`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b99c2dfe7b1a527300bd8de8147e159f8ecdbab796e7a71c7dd3e2df8cf216`  
		Last Modified: Mon, 29 Jun 2020 20:18:48 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9969646e605208d0301ec4741756dd6257ac0991ed01bfde817b513b8e7a9e19`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2919689d5a48dd6e4ef39397ffed789e7ff54451a9abaadbc274574a363256e`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfa5d572d4b3ac461e8246a58be6e84431cc733d430cb532e99e83af335ded3`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 239.7 KB (239740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90df7192caf1a86dbf2f53b57375af83ea514b4128fc8040808368b6ae7fd815`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:42b2115a0f6b0c698531f3b41f61a85096377ad6f2bc9c7a967b5f7efaecf78b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:e8b1865dd51a79cddf1ce786b52156e81cbaf67046a24bd475a8115ab960445c
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2312693391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ddbcd3c45a5583a6c9b91d6672b879ac5fd94c25a88540d6ca81b52c37931de`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Tue, 09 Jun 2020 22:33:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:02:29 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:03:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 29 Jun 2020 20:14:27 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:14:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('360bade38fea4d0e87bf00f2dc0c7e7b4434bb020af49d189b2c424246710bf6a3074e486ef2c3d6994473bcd62393302a1a704c215b4e323eeaecbfa359a533')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 29 Jun 2020 20:15:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 29 Jun 2020 20:15:02 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 29 Jun 2020 20:15:03 GMT
VOLUME [c:/config]
# Mon, 29 Jun 2020 20:15:04 GMT
VOLUME [c:/data]
# Mon, 29 Jun 2020 20:15:05 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 20:15:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 20:15:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 20:15:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 20:15:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 20:15:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 20:15:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 20:15:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 20:15:11 GMT
EXPOSE 80
# Mon, 29 Jun 2020 20:15:12 GMT
EXPOSE 443
# Mon, 29 Jun 2020 20:15:13 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 20:15:29 GMT
RUN caddy version
# Mon, 29 Jun 2020 20:15:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f841c6a0c622cd36b5b2688011a224ac3e8e96273758f4a2804f2f3f099f267d`  
		Last Modified: Tue, 09 Jun 2020 23:17:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e676deb3766189ea2b008f69205017c9ee31a77f9c7001fb5a07fb2e2d4fbb0`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba576338ed5242ba3fb838ce5fa930abb61e22fc422ba46b260dbca773cb9`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 4.8 MB (4772911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723eab0814ebbb502654a889ac99b52f2f7cb218a7164887ad0c9a1a5634d191`  
		Last Modified: Mon, 29 Jun 2020 20:18:31 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d3ac5a82f61292731263eecfe0635a4e0b486dd7f7f843a5cf9c1962fb54f1`  
		Last Modified: Mon, 29 Jun 2020 20:18:34 GMT  
		Size: 13.7 MB (13685965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18990846d9f6b2e03b43f0c42307982b5d13426a8d003425ce98e88c1ee61e9e`  
		Last Modified: Mon, 29 Jun 2020 20:18:30 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd85b14725d34f8e3d6505a3730098d0d983c7bfc436fab9f0025e28ea413c9`  
		Last Modified: Mon, 29 Jun 2020 20:18:30 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c83ec7d2b6fe2d3beb4121b8691686945da20d9398144840e2699dd7352378`  
		Last Modified: Mon, 29 Jun 2020 20:18:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7205b75fee4bcd79e0441081d0c18f4f16c9e3faddfbe44e9a2017d9c98e12`  
		Last Modified: Mon, 29 Jun 2020 20:18:29 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2d684094d65ac89815f73d6bb42fcc037bb91d14788f39d7c874f923010f78`  
		Last Modified: Mon, 29 Jun 2020 20:18:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d345ee36ca73380ffc59a00a9f9645c4be0f97bd3450083d5105bfb2456e5379`  
		Last Modified: Mon, 29 Jun 2020 20:18:27 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1399cf9fea037f4b40be192761883219e66d7fac0e8a7e53707b63894fd9a0a`  
		Last Modified: Mon, 29 Jun 2020 20:18:27 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abd79214efe888d78b44116335a0015f91de32819741eba80d9523b930ea548`  
		Last Modified: Mon, 29 Jun 2020 20:18:26 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1ac2c904ffff4f7f0d926f3fedbd61527aaf55aa38e88cde26c9d568962975`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108a4ea5a1055078abaa7e068c8d881cf36e81204a33175caff409d43aa0c9ce`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6c57249f136d38f7aa1045a8956c4f5f4c3f50d93bfb010221f45219da7dd5`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dec9ff0349ee91649d28733494db17d02470cf6a73f8268d7f3e717bb52f90`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c09a8d6df681bb92ae4ee08eb66e50aa8636527ebad60c50ee3917dd252a97`  
		Last Modified: Mon, 29 Jun 2020 20:18:22 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3888338b94e4b7f8a0a2eeb0c1724e90d743bddbbda11b28ed6a436cc0acc571`  
		Last Modified: Mon, 29 Jun 2020 20:18:22 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6ef034637a0be1fc8331c80eceeaba597da0bda3d9bb9769fde9678f401e9d`  
		Last Modified: Mon, 29 Jun 2020 20:18:22 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e84984fd0f42956c1dc9d31717a9fada1dfdf8e2cb00ce952e2655bf25249ce`  
		Last Modified: Mon, 29 Jun 2020 20:18:23 GMT  
		Size: 298.4 KB (298450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b4fdef44f059a30624268d4a303dc4436aada1655b41b5380dcdf6a1b925a7`  
		Last Modified: Mon, 29 Jun 2020 20:18:23 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:0f179ab33aa576db54d686130dcb5cfe8c3ce5f292f5bccc9fa16f1128bfc31f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:c9cc0726f345f76e464e535e972374668d02c30c224057e4f82e4186ae942ba6
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758382605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:150ecdbd7cbd511f1549e36fab065abcf44446cf7fcd58e45ceef61df883bf2b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:04:40 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:06:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 29 Jun 2020 20:15:40 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:17:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('360bade38fea4d0e87bf00f2dc0c7e7b4434bb020af49d189b2c424246710bf6a3074e486ef2c3d6994473bcd62393302a1a704c215b4e323eeaecbfa359a533')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 29 Jun 2020 20:17:05 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 29 Jun 2020 20:17:06 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 29 Jun 2020 20:17:07 GMT
VOLUME [c:/config]
# Mon, 29 Jun 2020 20:17:08 GMT
VOLUME [c:/data]
# Mon, 29 Jun 2020 20:17:09 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 20:17:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 20:17:11 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 20:17:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 20:17:12 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 20:17:13 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 20:17:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 20:17:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 20:17:16 GMT
EXPOSE 80
# Mon, 29 Jun 2020 20:17:17 GMT
EXPOSE 443
# Mon, 29 Jun 2020 20:17:18 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 20:17:58 GMT
RUN caddy version
# Mon, 29 Jun 2020 20:17:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22985925139cd6a6e83b6eb5286a8a6e1053a5c6ddd9762f34deea2aa6bcaacc`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43c028d6768e901bc64b3edb7e2e5f72050d3ed78ea4e7337fe85725d250c15`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 5.4 MB (5404509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae58d77a8d67f842374c3e60732465a9aaddfd9ce2b054b39aac0b7f2a420d0f`  
		Last Modified: Mon, 29 Jun 2020 20:18:56 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f76df30f6b9698ddedad69790139a9d2cf4fc871763691861f8aab018ac8ed`  
		Last Modified: Mon, 29 Jun 2020 20:19:01 GMT  
		Size: 18.7 MB (18718943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf3b4f088973e051021b74d9b9f795a9f2c8c71f7ae83e83f0cd6e95343f562`  
		Last Modified: Mon, 29 Jun 2020 20:18:56 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef3ce431d20a03b531eadce4cbe5680aca6c4ee4e24d70578687c89963b41d1`  
		Last Modified: Mon, 29 Jun 2020 20:18:55 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091019db4f4b75fe37b7b7ce991db4c4b02422388f836be3c4eb7c51159208b3`  
		Last Modified: Mon, 29 Jun 2020 20:18:54 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e080558fbf5cadbed8b34080d8bad08b45fff65ab533d87a24639d3ba6fd837f`  
		Last Modified: Mon, 29 Jun 2020 20:18:54 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc66481244327f616ca39ffe8c4b596d1aa9b7d778aa717e75b0b8f4a4c06350`  
		Last Modified: Mon, 29 Jun 2020 20:18:54 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f6e5557d697d57716bbf495fc701cef5b9073dbe5646f64fbbb0b8207fc07a`  
		Last Modified: Mon, 29 Jun 2020 20:18:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e238dae9de9d36d2c73796aa4c2a29645bbd5239ab47082579ccdc42e76244d8`  
		Last Modified: Mon, 29 Jun 2020 20:18:53 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbccba413742cc92bb8c53edd613f0be0250226ae8465165c5bc4e25a0c79a0`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911208ad8ab28008b96820a6251bee291bb5840e23ec782b1bbafdfe8019e08c`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2440198b129a0383b522e8b349ec26d2b66b1b33c422df3c3933be7c6591f661`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa72d9c6b7293c4d60c48fc5729c6f3a7eaa2f8276c8cba94bbb20edab126354`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a35778894255e6ba11c0d42ca54c80e69279c8777b609c7366208de7e0ac4c`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b99c2dfe7b1a527300bd8de8147e159f8ecdbab796e7a71c7dd3e2df8cf216`  
		Last Modified: Mon, 29 Jun 2020 20:18:48 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9969646e605208d0301ec4741756dd6257ac0991ed01bfde817b513b8e7a9e19`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2919689d5a48dd6e4ef39397ffed789e7ff54451a9abaadbc274574a363256e`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfa5d572d4b3ac461e8246a58be6e84431cc733d430cb532e99e83af335ded3`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 239.7 KB (239740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90df7192caf1a86dbf2f53b57375af83ea514b4128fc8040808368b6ae7fd815`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:76f1223d447df304172b1f8a6d22f70d2e43afd276ca0e107513e958d8629ded
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:alpine` - linux; amd64

```console
$ docker pull caddy@sha256:4ebb2f65ffef1445e2bcf137fc482fb212994bdb13b1868d750676725e7cf443
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16498000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a737824e95f5dac6216b82956d982715f24a48b766894844b1a6a607c2375027`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:21:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 21:21:16 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 21:21:18 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 20:19:29 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:19:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 20:19:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 20:19:33 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 20:19:33 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 20:19:33 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 20:19:33 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 20:19:34 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 20:19:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 20:19:34 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 20:19:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 20:19:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 20:19:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 20:19:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 20:19:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 20:19:35 GMT
EXPOSE 80
# Mon, 29 Jun 2020 20:19:35 GMT
EXPOSE 443
# Mon, 29 Jun 2020 20:19:35 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 20:19:36 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 20:19:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed237faf7b90187b720d5e863fb021a1ca678304744dad14ff8ad6434e4e1da`  
		Last Modified: Mon, 15 Jun 2020 21:22:02 GMT  
		Size: 300.0 KB (299981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e49a2f7ba4b80caa31bb2874b39f9c4bbb447708f3a0e07ff43892744e63a4`  
		Last Modified: Mon, 15 Jun 2020 21:22:02 GMT  
		Size: 5.8 KB (5767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc737685e2c14b5fdd7d0988d75baaf51de1353bc59127eebf7be1b496a02f9`  
		Last Modified: Mon, 29 Jun 2020 20:20:10 GMT  
		Size: 13.4 MB (13394558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba35373e6dd60c32e3ee0c3336ea77052d4cf981bed1cfd7a8f6b1e2fdf6f1cd`  
		Last Modified: Mon, 29 Jun 2020 20:20:07 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:cf35a85f26269ab62adfe126d4669c6951ec6bb9ff26fe21cfd494aff1d2d3d4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.6 MB (15646628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55d1456582127518b50a7cca33e619677857b0dee80fe88ff99e35ef84d53468`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:52:06 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 20:52:07 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 20:52:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 19:49:31 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:49:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 19:49:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 19:49:45 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 19:49:46 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 19:49:46 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 19:49:47 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 19:49:47 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 19:49:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 19:49:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 19:49:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 19:49:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 19:49:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 19:49:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 19:49:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 19:49:52 GMT
EXPOSE 80
# Mon, 29 Jun 2020 19:49:53 GMT
EXPOSE 443
# Mon, 29 Jun 2020 19:49:53 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 19:49:54 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 19:49:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2a5a47b7ff29cc165cee9824ba874fa6cb56d737ce18f841fc3ed5e937cb75`  
		Last Modified: Mon, 15 Jun 2020 20:54:38 GMT  
		Size: 300.1 KB (300144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3243ce9c25dc28a597c553cc7f0d4816c4b75789e4ebc37225ac58d5bd078995`  
		Last Modified: Mon, 15 Jun 2020 20:54:38 GMT  
		Size: 5.8 KB (5842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e9f25f4ff5c7a540a28a538f1a268137ec941f2be720b1bb5a284f588131f9`  
		Last Modified: Mon, 29 Jun 2020 19:52:00 GMT  
		Size: 12.7 MB (12737203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363d05163dedef9589519a417c89106201dbedc9dfe6b122a9eaa60ab2885a1f`  
		Last Modified: Mon, 29 Jun 2020 19:51:56 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:d370dd37d66b0814addc5114c3b4be7e42c00bfa90501c6497c8765a4036fa40
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15427533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7d7e451c4983b297ee7dbcda3b2334193679fcf011df665e95933aa8c27a260`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:59:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 21:00:00 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 21:00:03 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 19:57:29 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:57:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 19:57:42 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 19:57:43 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 19:57:44 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 19:57:44 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 19:57:45 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 19:57:46 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 19:57:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 19:57:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 19:57:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 19:57:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 19:57:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 19:57:50 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 19:57:50 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 19:57:51 GMT
EXPOSE 80
# Mon, 29 Jun 2020 19:57:52 GMT
EXPOSE 443
# Mon, 29 Jun 2020 19:57:52 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 19:57:53 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 19:57:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2aa34f01f2f9112772fdaebe7083b7dcdb4313768e0d6533a3e5b99597c98d`  
		Last Modified: Mon, 15 Jun 2020 21:02:12 GMT  
		Size: 299.2 KB (299237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b107a7bf1560d80dcded532795715f77765cf1a3d9464665d42acab82d366e`  
		Last Modified: Mon, 15 Jun 2020 21:02:12 GMT  
		Size: 5.8 KB (5845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a9aae216c1bc5bb511c635b06620b9537a354f011671c718d62e1f0cdd1e55`  
		Last Modified: Mon, 29 Jun 2020 19:59:29 GMT  
		Size: 12.7 MB (12715535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e31bd59a84cad62fcf351b80ea45db935206ee2a53dc6c6755a05a3a56b350a`  
		Last Modified: Mon, 29 Jun 2020 19:59:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7bae42d1c40f55e4406c24be4cbf0980dd87ab27d4e0cff6a5dddbea55aabca2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15324730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5794c058f0b994dcd4698e866d7db6dafc76f0cb9be4a1262eb893314a6176a9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:42:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 20:42:33 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 20:42:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 19:40:19 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:40:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 19:40:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 19:40:27 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 19:40:28 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 19:40:28 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 19:40:29 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 19:40:29 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 19:40:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 19:40:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 19:40:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 19:40:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 19:40:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 19:40:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 19:40:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 19:40:35 GMT
EXPOSE 80
# Mon, 29 Jun 2020 19:40:36 GMT
EXPOSE 443
# Mon, 29 Jun 2020 19:40:37 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 19:40:38 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 19:40:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f33282aee1a51127f669c7222e26bd0d5107b28d68819a6ead7f68076a73dc`  
		Last Modified: Mon, 15 Jun 2020 20:44:05 GMT  
		Size: 300.4 KB (300393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b85f4621f67650b74dc2db70b30f9593bc6695d3e91ff3899b3ee7c34cffc04`  
		Last Modified: Mon, 15 Jun 2020 20:44:04 GMT  
		Size: 5.8 KB (5846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f2cff8627bb2fbb4a0a0b9f9b57936ec53447aa2d2de70f1b7a5381acede31`  
		Last Modified: Mon, 29 Jun 2020 19:41:45 GMT  
		Size: 12.3 MB (12310372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934573df7ec7ebf99ab90bd97aa562d53dc3334ebdad1cc27970c48352809d2b`  
		Last Modified: Mon, 29 Jun 2020 19:41:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:382970b5cca83435fda7ec524c4e55f6f3eac245fa3ba70d1436b430995a9ef8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15188949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98bd39661b7c63c2701d172a8d747148274c11c8866b67a0a95036c34d95c8c8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:19:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 21:19:13 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 21:19:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 20:17:08 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:17:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 20:17:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 20:17:29 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 20:17:31 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 20:17:34 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 20:17:38 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 20:17:41 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 20:17:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 20:17:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 20:17:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 20:17:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 20:18:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 20:18:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 20:18:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 20:18:10 GMT
EXPOSE 80
# Mon, 29 Jun 2020 20:18:13 GMT
EXPOSE 443
# Mon, 29 Jun 2020 20:18:16 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 20:18:20 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 20:18:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b28df4c8a155654ad705e08f459bd177acc1005644ce2173ac62e954d6d4d2`  
		Last Modified: Mon, 15 Jun 2020 21:24:35 GMT  
		Size: 302.4 KB (302369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2288431c86a795754eb4d3a678e778c534a14e9243aea01a7cf9feff8d8e4e`  
		Last Modified: Mon, 15 Jun 2020 21:24:35 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d7ec5c119ab9881df3cbd4ba6b7b5c760c3b2ba149852fd430ff4cb8381c9a`  
		Last Modified: Mon, 29 Jun 2020 20:21:56 GMT  
		Size: 12.1 MB (12075379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788a23ed056849a1dc58fd563a9f8e0827e3f16678c61af3495f2a751cdf718d`  
		Last Modified: Mon, 29 Jun 2020 20:21:53 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:31dbbca225902439b42fd9e804440b767a810c638671193051eb0e47dd8af357
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (16040684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:589941f612353f33545544e2621a4a8fc31e28b78dd33543b2a7b3b5a5f7d09d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:43:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 20:43:15 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 20:43:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 19:41:26 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:41:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 19:41:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 19:41:30 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 19:41:30 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 19:41:30 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 19:41:30 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 19:41:31 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 19:41:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 19:41:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 19:41:31 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 19:41:31 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 19:41:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 19:41:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 19:41:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 19:41:32 GMT
EXPOSE 80
# Mon, 29 Jun 2020 19:41:32 GMT
EXPOSE 443
# Mon, 29 Jun 2020 19:41:33 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 19:41:33 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 19:41:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc47bdcaea173dfb029a09265c41846030477dc696b22fed52acad2b2078bb7`  
		Last Modified: Mon, 15 Jun 2020 20:44:21 GMT  
		Size: 300.5 KB (300524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf084f3ceb3b3b1196400fa251cc45e01de7ece41b7605bb40ae5178d849b47d`  
		Last Modified: Mon, 15 Jun 2020 20:44:26 GMT  
		Size: 5.8 KB (5841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236e43429060d4faebd33793542b4580546354f9e942339b380a69c0d1ebc94a`  
		Last Modified: Mon, 29 Jun 2020 19:42:20 GMT  
		Size: 13.2 MB (13167975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c83d9fdfe57ad6eda493263027564db3f25c9b58a45c2afaf3738e6ccb6e452`  
		Last Modified: Mon, 29 Jun 2020 19:42:19 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:e455aded5df9a8ebb35447ab864c1426f80ee6f807c66d1e61ffeb00bea1889e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:174f4aac00feefebff6adf98c35b9d83f92e8b1b83e2fda9316d7747a7cd0f15
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.0 MB (333987526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41fdef47036e115062adce80689ad61ccb2b9cd17b0893c0a02eec8b638b8d43`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:30:19 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:30:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:30:20 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:32:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:32:35 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:32:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:32:36 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:32:36 GMT
WORKDIR /go
# Mon, 15 Jun 2020 21:21:27 GMT
WORKDIR /src
# Mon, 15 Jun 2020 21:21:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 29 Jun 2020 20:19:40 GMT
ENV CADDY_SOURCE_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:19:42 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Mon, 29 Jun 2020 20:19:42 GMT
WORKDIR /src/caddy/cmd/caddy
# Mon, 29 Jun 2020 20:19:56 GMT
RUN go get -d ./...
# Mon, 29 Jun 2020 20:19:57 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Mon, 29 Jun 2020 20:19:57 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8968b2872e472e21554ca58b35a02277634f3e501cc04ab7b0d0963f60f54d`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 282.6 KB (282603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92cc7c5fd73817407fa0e4de5e1fb262a9c0f34c35c7450a2d01a7cef79c62f`  
		Last Modified: Tue, 02 Jun 2020 01:44:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0cccf56431698a0981b191f61dcb4ba6afa272d35deb14eaccf2cb46ed0f9d`  
		Last Modified: Tue, 02 Jun 2020 01:44:38 GMT  
		Size: 132.1 MB (132120859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbe0275821fc905c0321a44449b7ca670963f2cc0824150bea2125dee8dc7376`  
		Last Modified: Tue, 02 Jun 2020 01:44:13 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8183c72c683b23caab534e2ddeef5f4a54ed1040c87f05484e0248e21bb74954`  
		Last Modified: Mon, 15 Jun 2020 21:22:10 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404f93ac2221d032b0fca7fdb3d4bc6d9156768ffc95251e0607652cfbecc8b8`  
		Last Modified: Mon, 15 Jun 2020 21:22:10 GMT  
		Size: 8.3 MB (8309926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603c90769f39a502c786ab7eee221293be6835a473c3d9aaa621afa6068b5ee8`  
		Last Modified: Mon, 29 Jun 2020 20:20:16 GMT  
		Size: 3.1 MB (3057920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a0952b6cb77878a7141da63ee7ec7a0786849b87f81eb46f22f9be090e94b6`  
		Last Modified: Mon, 29 Jun 2020 20:20:38 GMT  
		Size: 187.4 MB (187417642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8a394faab9ec441308fbf55d2e542c297e7c61a9f3ae3ad6658c8e110d187a`  
		Last Modified: Mon, 29 Jun 2020 20:20:15 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3a8152559323a4cf8eb3ef0ca03307062d34e3a5ba24bbd517d6c64f9a96b2`  
		Last Modified: Mon, 29 Jun 2020 20:20:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:9d7661f3789c9c9d95cd0afa4026a4954b638757c0d1350694b8d9e7f71c8307
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.5 MB (329510925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e2f7767b3f46ec3fcde26b3dd823bd3bc05cefd8b63107be285e238972844df`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 02:02:10 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 02:02:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 02:02:29 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 02:55:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 02:56:02 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 02:56:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 02:56:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 02:56:07 GMT
WORKDIR /go
# Mon, 15 Jun 2020 20:52:46 GMT
WORKDIR /src
# Mon, 15 Jun 2020 20:52:50 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 29 Jun 2020 19:50:02 GMT
ENV CADDY_SOURCE_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:50:06 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Mon, 29 Jun 2020 19:50:06 GMT
WORKDIR /src/caddy/cmd/caddy
# Mon, 29 Jun 2020 19:51:25 GMT
RUN go get -d ./...
# Mon, 29 Jun 2020 19:51:33 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Mon, 29 Jun 2020 19:51:34 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c276dc457bae632c9eadd1ac69c1a756a9a67e050b0350a475b19663722191cf`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 282.8 KB (282778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f0819b703e39c232c6d0a8ac0f76d8f3c6856629db16fd6dd7b7ae69368281`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e66763a2c2fd4a68d63d58e30f372cf4ebdc811274c6979d891e5e0cb676d73`  
		Last Modified: Tue, 02 Jun 2020 05:22:08 GMT  
		Size: 128.2 MB (128209215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7367c813a205e4503e365f0492c4c2de22baead5b600a620d362655aa9cd483`  
		Last Modified: Tue, 02 Jun 2020 05:21:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce88b922cbeaa0f67211b29ad7ed76847d7725e329cc620ff7dcc9257fba77e3`  
		Last Modified: Mon, 15 Jun 2020 20:54:49 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720f093e5ede770f019c0c7a14a3361e9648d5b00f7a171f8feaefab719955aa`  
		Last Modified: Mon, 15 Jun 2020 20:54:50 GMT  
		Size: 7.9 MB (7928846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f025440c9236e5025567778b1c12077fb848a31569134c04c8b3cc35245700d`  
		Last Modified: Mon, 29 Jun 2020 19:52:07 GMT  
		Size: 3.1 MB (3058957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8344d190141f30e1aae92a5b7895c902dce5118a7f926ef5d5dfabb338077de8`  
		Last Modified: Mon, 29 Jun 2020 19:52:56 GMT  
		Size: 187.4 MB (187426715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db33b81f00857c93719b9256ab96b7c1d0ea8a69d3f3e32849ac07e97929cc9`  
		Last Modified: Mon, 29 Jun 2020 19:52:07 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f108514bdcdf3896865f08d980a37ab7cd19cb828c0b2221a5e5c2e5b5200c`  
		Last Modified: Mon, 29 Jun 2020 19:52:07 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a7788f8eef0de32ff4ee764adb2b1a35290eb353f19e345958f35df232d16acc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.2 MB (328162638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5546f695708008cd952d145b679402d539b3f8552695b15d4a0f8afa2e72cfee`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:10:58 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:11:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:11:01 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:34:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:34:38 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:34:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:34:43 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:34:44 GMT
WORKDIR /go
# Mon, 15 Jun 2020 21:00:34 GMT
WORKDIR /src
# Mon, 15 Jun 2020 21:00:37 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 29 Jun 2020 19:58:00 GMT
ENV CADDY_SOURCE_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:58:03 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Mon, 29 Jun 2020 19:58:04 GMT
WORKDIR /src/caddy/cmd/caddy
# Mon, 29 Jun 2020 19:59:01 GMT
RUN go get -d ./...
# Mon, 29 Jun 2020 19:59:07 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Mon, 29 Jun 2020 19:59:08 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512c25ce227edddad11326504a9bab47e83f8b61c090c9dc95882452984ac62`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 281.9 KB (281892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87928ee7e6c788309b46621e351321410e4dde5374869ffa75f404b19e0e0c12`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754691c4bcf20eb06087104e5fc82d340991d9bf26c21cae6979f36e3bd38ca7`  
		Last Modified: Tue, 02 Jun 2020 03:52:16 GMT  
		Size: 127.8 MB (127846663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63238be1b74c86ab98841c3959a33d79a903d58ac50518d4fa65b2ea8c6a75ba`  
		Last Modified: Tue, 02 Jun 2020 03:51:20 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a1abd4bf80876cf553a554662e0cb3c5c310601b937ee7749c6f828de9dfea`  
		Last Modified: Mon, 15 Jun 2020 21:02:23 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac591f152779d4cfd93fb1e2f29dfeb27073f3559e8cb0daf8ee5c6f58310dc`  
		Last Modified: Mon, 15 Jun 2020 21:02:23 GMT  
		Size: 7.1 MB (7144878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e0594bfc9d580f4e451d7cbb01f558bfe98432dd6ee33eb4a443825ac46449`  
		Last Modified: Mon, 29 Jun 2020 19:59:36 GMT  
		Size: 3.1 MB (3058990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08a2552e8b69f86ac9b9c6958b9ee45d37e3d8c2a5d693fa7040f93fecb1af7`  
		Last Modified: Mon, 29 Jun 2020 20:00:27 GMT  
		Size: 187.4 MB (187422323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae179221c59eb112751c3f996f0ecb537813be0fafd1a4bd1cde75f43575d52`  
		Last Modified: Mon, 29 Jun 2020 19:59:35 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c2ee8d77f04705a1012498984c1060591fb20d309efdec522a25b7fd059680`  
		Last Modified: Mon, 29 Jun 2020 19:59:35 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:9b2e83c1df1c45e57f97c48bdc5d944e64b9fbafe4621f588941f8535c07a05c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.5 MB (328477149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b87b66e72fe48cf1e13cb7c0ca831fddd9b1200500629d508be6de71b386a2d4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:57:21 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:58:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:58:16 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 02:00:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 02:00:34 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 02:00:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 02:00:55 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 02:01:01 GMT
WORKDIR /go
# Mon, 15 Jun 2020 20:42:55 GMT
WORKDIR /src
# Mon, 15 Jun 2020 20:42:58 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 29 Jun 2020 19:40:47 GMT
ENV CADDY_SOURCE_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:40:51 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Mon, 29 Jun 2020 19:40:52 GMT
WORKDIR /src/caddy/cmd/caddy
# Mon, 29 Jun 2020 19:41:20 GMT
RUN go get -d ./...
# Mon, 29 Jun 2020 19:41:27 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Mon, 29 Jun 2020 19:41:28 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f711af9a0d350d42a1cb00f41feb32277e11189d70d84d76fdef5065f78c47`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 283.0 KB (282997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f96fe45779b3ba9e9daededd02c233c5c76715ef1c5e88dd10c7acbea8414f`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a10f6d585c919680bed516e83e217d8bb824ee48306a00ce36c94a2a42e127`  
		Last Modified: Tue, 02 Jun 2020 02:30:00 GMT  
		Size: 126.5 MB (126505030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fdc7971b1eac6baae4423fc0ecca822c4d0372de7bfbdb5a7451e3cdd06be30`  
		Last Modified: Tue, 02 Jun 2020 02:29:25 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9d4bc6b21331beadc7877a16034ab0b38c0afcf3434fba21ae30649336cb92`  
		Last Modified: Mon, 15 Jun 2020 20:44:13 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebe763a900953fc839be7c307bee96cc4464502cd2cf875941354458648b2b4`  
		Last Modified: Mon, 15 Jun 2020 20:44:13 GMT  
		Size: 8.5 MB (8499921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd27d4d70da701eebdcb2e122f3ba1e8e37426112e12ab1fbbe2e8ee0d6dccd4`  
		Last Modified: Mon, 29 Jun 2020 19:41:52 GMT  
		Size: 3.1 MB (3058980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92f41d7e82ced6444f24c9196af37bc1b89cfcda5a0d73d5a1c46ba7e77282f`  
		Last Modified: Mon, 29 Jun 2020 19:42:30 GMT  
		Size: 187.4 MB (187421128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81ac8d9d1615f457d108d726bb296ebea749e3492e4a639d965461dff718955`  
		Last Modified: Mon, 29 Jun 2020 19:41:51 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e1562a3a569241d3ea907191c7197ea60d84f24a3ed5438c09cfbdea6c4972`  
		Last Modified: Mon, 29 Jun 2020 19:41:51 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:08127eef54ee0f4a65aac670acb12694f8aedc66bfb5f7c5a1117b0932e55b46
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.8 MB (327766267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f38654e854c4d326b17dbe210820d8fec5ce3ed9a388e22bd06ce27693b11eb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:29:37 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:29:54 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:30:00 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:32:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:32:22 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:32:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:32:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:32:46 GMT
WORKDIR /go
# Mon, 15 Jun 2020 21:20:48 GMT
WORKDIR /src
# Mon, 15 Jun 2020 21:20:57 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 29 Jun 2020 20:18:34 GMT
ENV CADDY_SOURCE_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:18:47 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Mon, 29 Jun 2020 20:18:51 GMT
WORKDIR /src/caddy/cmd/caddy
# Mon, 29 Jun 2020 20:21:19 GMT
RUN go get -d ./...
# Mon, 29 Jun 2020 20:21:29 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Mon, 29 Jun 2020 20:21:32 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d800b4e456ea05213bc7310b5d1b1706274430828a3c19a2fa8c6694733dc4`  
		Last Modified: Tue, 02 Jun 2020 01:48:21 GMT  
		Size: 285.0 KB (285034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45a7c013c1132848fd122dfb4511c34ed884573ddfd7d8ad13d9a8a6157c42`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa9f54e0b14ecd0984863bb950f61bd4bf436b6072e38800e7f963358557067`  
		Last Modified: Tue, 02 Jun 2020 01:48:47 GMT  
		Size: 125.3 MB (125263901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a41edd0480b633d5ed3f00eef305e8a7526c48f1fdde5ef350565830d40609`  
		Last Modified: Tue, 02 Jun 2020 01:48:20 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca1ca7c0085d0ffb2b0cb1bdabb73af28921fe105ac26bae09acee083eb4c72`  
		Last Modified: Mon, 15 Jun 2020 21:24:51 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55082f384c6dea8e172df520164ab7feeca61be6b9d38ab64bb2265b7f197b1`  
		Last Modified: Mon, 15 Jun 2020 21:24:49 GMT  
		Size: 8.9 MB (8919998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef68f42bbb77bbb1f77ff75b7844f6871222865c01822b3479c9bfacd19afbfe`  
		Last Modified: Mon, 29 Jun 2020 20:22:09 GMT  
		Size: 3.1 MB (3056722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f055e9f88932992a7302c04e8502ad82457b4cca90a5f8da7c67c1a1ce686e5a`  
		Last Modified: Mon, 29 Jun 2020 20:22:36 GMT  
		Size: 187.4 MB (187434281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75cd750be57c01f0ccc6d84c16b2ee317cd5364f7933ff71de5f6d023f04adbd`  
		Last Modified: Mon, 29 Jun 2020 20:22:08 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ccc0213dea3f99dffb64414d611d494f9b129eee3aebcb59ea0e81be9df9f37`  
		Last Modified: Mon, 29 Jun 2020 20:22:07 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:0169dfe70d71f5cf9c35f9947ee054112da43b3baeb7d53fadbb477d901424a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.5 MB (333495213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:270b81fea5e00d9fc31bda2961e13708de4ae9569b09c9a2f89751d01d513703`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 01:53:15 GMT
RUN apk add --no-cache 		ca-certificates
# Tue, 02 Jun 2020 01:53:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Jun 2020 01:53:16 GMT
ENV GOLANG_VERSION=1.14.4
# Tue, 02 Jun 2020 01:54:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '7011af3bbc2ac108d1b82ea8abb87b2e63f78844f0259be20cde4d42c5c40584 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Tue, 02 Jun 2020 01:54:38 GMT
ENV GOPATH=/go
# Tue, 02 Jun 2020 01:54:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Jun 2020 01:54:38 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 02 Jun 2020 01:54:39 GMT
WORKDIR /go
# Mon, 15 Jun 2020 20:43:26 GMT
WORKDIR /src
# Mon, 15 Jun 2020 20:43:28 GMT
RUN apk add --no-cache     git     ca-certificates
# Mon, 29 Jun 2020 19:41:38 GMT
ENV CADDY_SOURCE_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:41:39 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Mon, 29 Jun 2020 19:41:40 GMT
WORKDIR /src/caddy/cmd/caddy
# Mon, 29 Jun 2020 19:41:59 GMT
RUN go get -d ./...
# Mon, 29 Jun 2020 19:42:07 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Mon, 29 Jun 2020 19:42:07 GMT
WORKDIR /src/custom-caddy/cmd/caddy
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094092570892a8483a3fc940b327cccddf0cb7affb2a628ef4c98e40b4830bd`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 283.1 KB (283144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64a1c2f9ba0751e3e55cf33ddc6f0fd325bce1e6d64ef921f6258c5115b3c0`  
		Last Modified: Tue, 02 Jun 2020 02:01:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc125fe27a23a8501491445468375e7ea9db946b45cbd911a05a65cfb7c3334`  
		Last Modified: Tue, 02 Jun 2020 02:01:21 GMT  
		Size: 131.8 MB (131814783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7129c3822665192c1533e7d5ab270717e256b1b9844d6fd116852b00a29058e9`  
		Last Modified: Tue, 02 Jun 2020 02:01:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d8d7ec191535d778fe97d9e282050d4140fab1236212ea77816ba1db178bae`  
		Last Modified: Mon, 15 Jun 2020 20:44:32 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a8d11ad8b6daae49f4e16f31468f03664af47d81d6792e5da6fb1eff11ee52`  
		Last Modified: Mon, 15 Jun 2020 20:44:32 GMT  
		Size: 8.4 MB (8352257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8663396503bae3461037b0068a6ef6c9ed511cc92f9e98e9284b59ade05a8b93`  
		Last Modified: Mon, 29 Jun 2020 19:42:26 GMT  
		Size: 3.1 MB (3058958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d136cb87215514845773f75dd169a4cab8b7c8dadbac4a8690a9cb9b92190d`  
		Last Modified: Mon, 29 Jun 2020 19:42:43 GMT  
		Size: 187.4 MB (187418751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb6fcd609f2e3e86d693af70201cbc44718bccd00e80f5d3053a5f642832900`  
		Last Modified: Mon, 29 Jun 2020 19:42:56 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e562fb9f71cf78663817e0f877a55ef56211183920d2840976d4ee2883d29dd`  
		Last Modified: Mon, 29 Jun 2020 19:42:25 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:9ee709b080aacb1a5cae6c4cb654d950f1ded75d7a2277a792860bb28134158e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1282; amd64
	-	windows version 10.0.14393.3750; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:4ebb2f65ffef1445e2bcf137fc482fb212994bdb13b1868d750676725e7cf443
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16498000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a737824e95f5dac6216b82956d982715f24a48b766894844b1a6a607c2375027`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:21:16 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 21:21:16 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 21:21:18 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 20:19:29 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:19:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 20:19:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 20:19:33 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 20:19:33 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 20:19:33 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 20:19:33 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 20:19:34 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 20:19:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 20:19:34 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 20:19:34 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 20:19:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 20:19:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 20:19:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 20:19:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 20:19:35 GMT
EXPOSE 80
# Mon, 29 Jun 2020 20:19:35 GMT
EXPOSE 443
# Mon, 29 Jun 2020 20:19:35 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 20:19:36 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 20:19:36 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed237faf7b90187b720d5e863fb021a1ca678304744dad14ff8ad6434e4e1da`  
		Last Modified: Mon, 15 Jun 2020 21:22:02 GMT  
		Size: 300.0 KB (299981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e49a2f7ba4b80caa31bb2874b39f9c4bbb447708f3a0e07ff43892744e63a4`  
		Last Modified: Mon, 15 Jun 2020 21:22:02 GMT  
		Size: 5.8 KB (5767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc737685e2c14b5fdd7d0988d75baaf51de1353bc59127eebf7be1b496a02f9`  
		Last Modified: Mon, 29 Jun 2020 20:20:10 GMT  
		Size: 13.4 MB (13394558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba35373e6dd60c32e3ee0c3336ea77052d4cf981bed1cfd7a8f6b1e2fdf6f1cd`  
		Last Modified: Mon, 29 Jun 2020 20:20:07 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:cf35a85f26269ab62adfe126d4669c6951ec6bb9ff26fe21cfd494aff1d2d3d4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.6 MB (15646628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55d1456582127518b50a7cca33e619677857b0dee80fe88ff99e35ef84d53468`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:52:06 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 20:52:07 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 20:52:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 19:49:31 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:49:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 19:49:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 19:49:45 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 19:49:46 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 19:49:46 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 19:49:47 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 19:49:47 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 19:49:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 19:49:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 19:49:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 19:49:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 19:49:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 19:49:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 19:49:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 19:49:52 GMT
EXPOSE 80
# Mon, 29 Jun 2020 19:49:53 GMT
EXPOSE 443
# Mon, 29 Jun 2020 19:49:53 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 19:49:54 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 19:49:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2a5a47b7ff29cc165cee9824ba874fa6cb56d737ce18f841fc3ed5e937cb75`  
		Last Modified: Mon, 15 Jun 2020 20:54:38 GMT  
		Size: 300.1 KB (300144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3243ce9c25dc28a597c553cc7f0d4816c4b75789e4ebc37225ac58d5bd078995`  
		Last Modified: Mon, 15 Jun 2020 20:54:38 GMT  
		Size: 5.8 KB (5842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e9f25f4ff5c7a540a28a538f1a268137ec941f2be720b1bb5a284f588131f9`  
		Last Modified: Mon, 29 Jun 2020 19:52:00 GMT  
		Size: 12.7 MB (12737203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363d05163dedef9589519a417c89106201dbedc9dfe6b122a9eaa60ab2885a1f`  
		Last Modified: Mon, 29 Jun 2020 19:51:56 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:d370dd37d66b0814addc5114c3b4be7e42c00bfa90501c6497c8765a4036fa40
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15427533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7d7e451c4983b297ee7dbcda3b2334193679fcf011df665e95933aa8c27a260`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:59:59 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 21:00:00 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 21:00:03 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 19:57:29 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:57:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 19:57:42 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 19:57:43 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 19:57:44 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 19:57:44 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 19:57:45 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 19:57:46 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 19:57:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 19:57:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 19:57:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 19:57:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 19:57:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 19:57:50 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 19:57:50 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 19:57:51 GMT
EXPOSE 80
# Mon, 29 Jun 2020 19:57:52 GMT
EXPOSE 443
# Mon, 29 Jun 2020 19:57:52 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 19:57:53 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 19:57:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2aa34f01f2f9112772fdaebe7083b7dcdb4313768e0d6533a3e5b99597c98d`  
		Last Modified: Mon, 15 Jun 2020 21:02:12 GMT  
		Size: 299.2 KB (299237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b107a7bf1560d80dcded532795715f77765cf1a3d9464665d42acab82d366e`  
		Last Modified: Mon, 15 Jun 2020 21:02:12 GMT  
		Size: 5.8 KB (5845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a9aae216c1bc5bb511c635b06620b9537a354f011671c718d62e1f0cdd1e55`  
		Last Modified: Mon, 29 Jun 2020 19:59:29 GMT  
		Size: 12.7 MB (12715535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e31bd59a84cad62fcf351b80ea45db935206ee2a53dc6c6755a05a3a56b350a`  
		Last Modified: Mon, 29 Jun 2020 19:59:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7bae42d1c40f55e4406c24be4cbf0980dd87ab27d4e0cff6a5dddbea55aabca2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15324730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5794c058f0b994dcd4698e866d7db6dafc76f0cb9be4a1262eb893314a6176a9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:42:32 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 20:42:33 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 20:42:35 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 19:40:19 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:40:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 19:40:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 19:40:27 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 19:40:28 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 19:40:28 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 19:40:29 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 19:40:29 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 19:40:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 19:40:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 19:40:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 19:40:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 19:40:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 19:40:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 19:40:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 19:40:35 GMT
EXPOSE 80
# Mon, 29 Jun 2020 19:40:36 GMT
EXPOSE 443
# Mon, 29 Jun 2020 19:40:37 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 19:40:38 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 19:40:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f33282aee1a51127f669c7222e26bd0d5107b28d68819a6ead7f68076a73dc`  
		Last Modified: Mon, 15 Jun 2020 20:44:05 GMT  
		Size: 300.4 KB (300393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b85f4621f67650b74dc2db70b30f9593bc6695d3e91ff3899b3ee7c34cffc04`  
		Last Modified: Mon, 15 Jun 2020 20:44:04 GMT  
		Size: 5.8 KB (5846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f2cff8627bb2fbb4a0a0b9f9b57936ec53447aa2d2de70f1b7a5381acede31`  
		Last Modified: Mon, 29 Jun 2020 19:41:45 GMT  
		Size: 12.3 MB (12310372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934573df7ec7ebf99ab90bd97aa562d53dc3334ebdad1cc27970c48352809d2b`  
		Last Modified: Mon, 29 Jun 2020 19:41:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:382970b5cca83435fda7ec524c4e55f6f3eac245fa3ba70d1436b430995a9ef8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15188949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98bd39661b7c63c2701d172a8d747148274c11c8866b67a0a95036c34d95c8c8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 21:19:09 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 21:19:13 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 21:19:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 20:17:08 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:17:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 20:17:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 20:17:29 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 20:17:31 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 20:17:34 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 20:17:38 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 20:17:41 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 20:17:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 20:17:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 20:17:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 20:17:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 20:18:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 20:18:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 20:18:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 20:18:10 GMT
EXPOSE 80
# Mon, 29 Jun 2020 20:18:13 GMT
EXPOSE 443
# Mon, 29 Jun 2020 20:18:16 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 20:18:20 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 20:18:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b28df4c8a155654ad705e08f459bd177acc1005644ce2173ac62e954d6d4d2`  
		Last Modified: Mon, 15 Jun 2020 21:24:35 GMT  
		Size: 302.4 KB (302369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2288431c86a795754eb4d3a678e778c534a14e9243aea01a7cf9feff8d8e4e`  
		Last Modified: Mon, 15 Jun 2020 21:24:35 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d7ec5c119ab9881df3cbd4ba6b7b5c760c3b2ba149852fd430ff4cb8381c9a`  
		Last Modified: Mon, 29 Jun 2020 20:21:56 GMT  
		Size: 12.1 MB (12075379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788a23ed056849a1dc58fd563a9f8e0827e3f16678c61af3495f2a751cdf718d`  
		Last Modified: Mon, 29 Jun 2020 20:21:53 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:31dbbca225902439b42fd9e804440b767a810c638671193051eb0e47dd8af357
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (16040684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:589941f612353f33545544e2621a4a8fc31e28b78dd33543b2a7b3b5a5f7d09d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Mon, 15 Jun 2020 20:43:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 15 Jun 2020 20:43:15 GMT
ENV CADDY_DIST_COMMIT=80870b227ded910971ecace4a0c136bf0ef46342
# Mon, 15 Jun 2020 20:43:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/$CADDY_DIST_COMMIT/welcome/index.html"
# Mon, 29 Jun 2020 19:41:26 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 19:41:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='17d425b20a6906adfa57fd98181b349a2de1a0ac3331ae5cc2858bef1a4d755d7eb0ed093e1bda256d00ecca5f950267bbb892d08f016f00606c5b21b72b51ee' ;; 		armhf)   binArch='armv6'; checksum='4260a1063eaebbafbf66370c697008ffcc991fadb0bf16e0382e296b5750d2b923c6bffeaa25c263e7bd0b919c42416b91246afff2aa2df160e7f2ffa3eb22c5' ;; 		armv7)   binArch='armv7'; checksum='54a65f92bcb0813ec0942611aec2dee3cbe2a15c580d6e44abaf23b85d3cba50740a655ea22a0984087b26b6002fb08c01da0d2c0c95341981c59da4a4fc6e75' ;; 		aarch64) binArch='arm64'; checksum='c2ced633f0de9ae7ffcf7484f364d199e19a962e6224a183a293926e6fffbd24e873c83327b7be1dcd43318e62376b1462a955e393d1e2c7d264e22fc24b7dee' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='d7a3015fee2f36079729246a816fca4656b45d67d708bf7fab9bbfa5ae200e777e97f5c4962de1693699204f32bb578cf31609bc0b1e19190fe1b7caeb5b9018' ;; 		s390x)   binArch='s390x'; checksum='5f0af31c7272dccf6ad2e206510e27980e03b5ac817014d5b90eb4f476b2897c752c0fd27aecfc6cdab2d410be6dfb926cda8f2f2da0b46b8cef5285d5dbc922' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 29 Jun 2020 19:41:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 29 Jun 2020 19:41:30 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 29 Jun 2020 19:41:30 GMT
ENV XDG_DATA_HOME=/data
# Mon, 29 Jun 2020 19:41:30 GMT
VOLUME [/config]
# Mon, 29 Jun 2020 19:41:30 GMT
VOLUME [/data]
# Mon, 29 Jun 2020 19:41:31 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 19:41:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 19:41:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 19:41:31 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 19:41:31 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 19:41:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 19:41:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 19:41:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 19:41:32 GMT
EXPOSE 80
# Mon, 29 Jun 2020 19:41:32 GMT
EXPOSE 443
# Mon, 29 Jun 2020 19:41:33 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 19:41:33 GMT
WORKDIR /srv
# Mon, 29 Jun 2020 19:41:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc47bdcaea173dfb029a09265c41846030477dc696b22fed52acad2b2078bb7`  
		Last Modified: Mon, 15 Jun 2020 20:44:21 GMT  
		Size: 300.5 KB (300524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf084f3ceb3b3b1196400fa251cc45e01de7ece41b7605bb40ae5178d849b47d`  
		Last Modified: Mon, 15 Jun 2020 20:44:26 GMT  
		Size: 5.8 KB (5841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236e43429060d4faebd33793542b4580546354f9e942339b380a69c0d1ebc94a`  
		Last Modified: Mon, 29 Jun 2020 19:42:20 GMT  
		Size: 13.2 MB (13167975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c83d9fdfe57ad6eda493263027564db3f25c9b58a45c2afaf3738e6ccb6e452`  
		Last Modified: Mon, 29 Jun 2020 19:42:19 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:e8b1865dd51a79cddf1ce786b52156e81cbaf67046a24bd475a8115ab960445c
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2312693391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ddbcd3c45a5583a6c9b91d6672b879ac5fd94c25a88540d6ca81b52c37931de`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Tue, 09 Jun 2020 22:33:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:02:29 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:03:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 29 Jun 2020 20:14:27 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:14:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('360bade38fea4d0e87bf00f2dc0c7e7b4434bb020af49d189b2c424246710bf6a3074e486ef2c3d6994473bcd62393302a1a704c215b4e323eeaecbfa359a533')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 29 Jun 2020 20:15:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 29 Jun 2020 20:15:02 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 29 Jun 2020 20:15:03 GMT
VOLUME [c:/config]
# Mon, 29 Jun 2020 20:15:04 GMT
VOLUME [c:/data]
# Mon, 29 Jun 2020 20:15:05 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 20:15:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 20:15:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 20:15:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 20:15:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 20:15:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 20:15:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 20:15:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 20:15:11 GMT
EXPOSE 80
# Mon, 29 Jun 2020 20:15:12 GMT
EXPOSE 443
# Mon, 29 Jun 2020 20:15:13 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 20:15:29 GMT
RUN caddy version
# Mon, 29 Jun 2020 20:15:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f841c6a0c622cd36b5b2688011a224ac3e8e96273758f4a2804f2f3f099f267d`  
		Last Modified: Tue, 09 Jun 2020 23:17:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e676deb3766189ea2b008f69205017c9ee31a77f9c7001fb5a07fb2e2d4fbb0`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba576338ed5242ba3fb838ce5fa930abb61e22fc422ba46b260dbca773cb9`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 4.8 MB (4772911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723eab0814ebbb502654a889ac99b52f2f7cb218a7164887ad0c9a1a5634d191`  
		Last Modified: Mon, 29 Jun 2020 20:18:31 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d3ac5a82f61292731263eecfe0635a4e0b486dd7f7f843a5cf9c1962fb54f1`  
		Last Modified: Mon, 29 Jun 2020 20:18:34 GMT  
		Size: 13.7 MB (13685965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18990846d9f6b2e03b43f0c42307982b5d13426a8d003425ce98e88c1ee61e9e`  
		Last Modified: Mon, 29 Jun 2020 20:18:30 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd85b14725d34f8e3d6505a3730098d0d983c7bfc436fab9f0025e28ea413c9`  
		Last Modified: Mon, 29 Jun 2020 20:18:30 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c83ec7d2b6fe2d3beb4121b8691686945da20d9398144840e2699dd7352378`  
		Last Modified: Mon, 29 Jun 2020 20:18:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7205b75fee4bcd79e0441081d0c18f4f16c9e3faddfbe44e9a2017d9c98e12`  
		Last Modified: Mon, 29 Jun 2020 20:18:29 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2d684094d65ac89815f73d6bb42fcc037bb91d14788f39d7c874f923010f78`  
		Last Modified: Mon, 29 Jun 2020 20:18:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d345ee36ca73380ffc59a00a9f9645c4be0f97bd3450083d5105bfb2456e5379`  
		Last Modified: Mon, 29 Jun 2020 20:18:27 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1399cf9fea037f4b40be192761883219e66d7fac0e8a7e53707b63894fd9a0a`  
		Last Modified: Mon, 29 Jun 2020 20:18:27 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abd79214efe888d78b44116335a0015f91de32819741eba80d9523b930ea548`  
		Last Modified: Mon, 29 Jun 2020 20:18:26 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1ac2c904ffff4f7f0d926f3fedbd61527aaf55aa38e88cde26c9d568962975`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108a4ea5a1055078abaa7e068c8d881cf36e81204a33175caff409d43aa0c9ce`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6c57249f136d38f7aa1045a8956c4f5f4c3f50d93bfb010221f45219da7dd5`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dec9ff0349ee91649d28733494db17d02470cf6a73f8268d7f3e717bb52f90`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c09a8d6df681bb92ae4ee08eb66e50aa8636527ebad60c50ee3917dd252a97`  
		Last Modified: Mon, 29 Jun 2020 20:18:22 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3888338b94e4b7f8a0a2eeb0c1724e90d743bddbbda11b28ed6a436cc0acc571`  
		Last Modified: Mon, 29 Jun 2020 20:18:22 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6ef034637a0be1fc8331c80eceeaba597da0bda3d9bb9769fde9678f401e9d`  
		Last Modified: Mon, 29 Jun 2020 20:18:22 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e84984fd0f42956c1dc9d31717a9fada1dfdf8e2cb00ce952e2655bf25249ce`  
		Last Modified: Mon, 29 Jun 2020 20:18:23 GMT  
		Size: 298.4 KB (298450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b4fdef44f059a30624268d4a303dc4436aada1655b41b5380dcdf6a1b925a7`  
		Last Modified: Mon, 29 Jun 2020 20:18:23 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:c9cc0726f345f76e464e535e972374668d02c30c224057e4f82e4186ae942ba6
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758382605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:150ecdbd7cbd511f1549e36fab065abcf44446cf7fcd58e45ceef61df883bf2b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:04:40 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:06:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 29 Jun 2020 20:15:40 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:17:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('360bade38fea4d0e87bf00f2dc0c7e7b4434bb020af49d189b2c424246710bf6a3074e486ef2c3d6994473bcd62393302a1a704c215b4e323eeaecbfa359a533')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 29 Jun 2020 20:17:05 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 29 Jun 2020 20:17:06 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 29 Jun 2020 20:17:07 GMT
VOLUME [c:/config]
# Mon, 29 Jun 2020 20:17:08 GMT
VOLUME [c:/data]
# Mon, 29 Jun 2020 20:17:09 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 20:17:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 20:17:11 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 20:17:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 20:17:12 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 20:17:13 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 20:17:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 20:17:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 20:17:16 GMT
EXPOSE 80
# Mon, 29 Jun 2020 20:17:17 GMT
EXPOSE 443
# Mon, 29 Jun 2020 20:17:18 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 20:17:58 GMT
RUN caddy version
# Mon, 29 Jun 2020 20:17:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22985925139cd6a6e83b6eb5286a8a6e1053a5c6ddd9762f34deea2aa6bcaacc`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43c028d6768e901bc64b3edb7e2e5f72050d3ed78ea4e7337fe85725d250c15`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 5.4 MB (5404509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae58d77a8d67f842374c3e60732465a9aaddfd9ce2b054b39aac0b7f2a420d0f`  
		Last Modified: Mon, 29 Jun 2020 20:18:56 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f76df30f6b9698ddedad69790139a9d2cf4fc871763691861f8aab018ac8ed`  
		Last Modified: Mon, 29 Jun 2020 20:19:01 GMT  
		Size: 18.7 MB (18718943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf3b4f088973e051021b74d9b9f795a9f2c8c71f7ae83e83f0cd6e95343f562`  
		Last Modified: Mon, 29 Jun 2020 20:18:56 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef3ce431d20a03b531eadce4cbe5680aca6c4ee4e24d70578687c89963b41d1`  
		Last Modified: Mon, 29 Jun 2020 20:18:55 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091019db4f4b75fe37b7b7ce991db4c4b02422388f836be3c4eb7c51159208b3`  
		Last Modified: Mon, 29 Jun 2020 20:18:54 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e080558fbf5cadbed8b34080d8bad08b45fff65ab533d87a24639d3ba6fd837f`  
		Last Modified: Mon, 29 Jun 2020 20:18:54 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc66481244327f616ca39ffe8c4b596d1aa9b7d778aa717e75b0b8f4a4c06350`  
		Last Modified: Mon, 29 Jun 2020 20:18:54 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f6e5557d697d57716bbf495fc701cef5b9073dbe5646f64fbbb0b8207fc07a`  
		Last Modified: Mon, 29 Jun 2020 20:18:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e238dae9de9d36d2c73796aa4c2a29645bbd5239ab47082579ccdc42e76244d8`  
		Last Modified: Mon, 29 Jun 2020 20:18:53 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbccba413742cc92bb8c53edd613f0be0250226ae8465165c5bc4e25a0c79a0`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911208ad8ab28008b96820a6251bee291bb5840e23ec782b1bbafdfe8019e08c`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2440198b129a0383b522e8b349ec26d2b66b1b33c422df3c3933be7c6591f661`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa72d9c6b7293c4d60c48fc5729c6f3a7eaa2f8276c8cba94bbb20edab126354`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a35778894255e6ba11c0d42ca54c80e69279c8777b609c7366208de7e0ac4c`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b99c2dfe7b1a527300bd8de8147e159f8ecdbab796e7a71c7dd3e2df8cf216`  
		Last Modified: Mon, 29 Jun 2020 20:18:48 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9969646e605208d0301ec4741756dd6257ac0991ed01bfde817b513b8e7a9e19`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2919689d5a48dd6e4ef39397ffed789e7ff54451a9abaadbc274574a363256e`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfa5d572d4b3ac461e8246a58be6e84431cc733d430cb532e99e83af335ded3`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 239.7 KB (239740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90df7192caf1a86dbf2f53b57375af83ea514b4128fc8040808368b6ae7fd815`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:197b83d529db3ebae4b13cb9079006ad0016f9964e1f1cad639679a2c214af7e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64
	-	windows version 10.0.14393.3750; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:e8b1865dd51a79cddf1ce786b52156e81cbaf67046a24bd475a8115ab960445c
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2312693391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ddbcd3c45a5583a6c9b91d6672b879ac5fd94c25a88540d6ca81b52c37931de`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Tue, 09 Jun 2020 22:33:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:02:29 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:03:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 29 Jun 2020 20:14:27 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:14:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('360bade38fea4d0e87bf00f2dc0c7e7b4434bb020af49d189b2c424246710bf6a3074e486ef2c3d6994473bcd62393302a1a704c215b4e323eeaecbfa359a533')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 29 Jun 2020 20:15:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 29 Jun 2020 20:15:02 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 29 Jun 2020 20:15:03 GMT
VOLUME [c:/config]
# Mon, 29 Jun 2020 20:15:04 GMT
VOLUME [c:/data]
# Mon, 29 Jun 2020 20:15:05 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 20:15:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 20:15:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 20:15:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 20:15:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 20:15:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 20:15:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 20:15:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 20:15:11 GMT
EXPOSE 80
# Mon, 29 Jun 2020 20:15:12 GMT
EXPOSE 443
# Mon, 29 Jun 2020 20:15:13 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 20:15:29 GMT
RUN caddy version
# Mon, 29 Jun 2020 20:15:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f841c6a0c622cd36b5b2688011a224ac3e8e96273758f4a2804f2f3f099f267d`  
		Last Modified: Tue, 09 Jun 2020 23:17:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e676deb3766189ea2b008f69205017c9ee31a77f9c7001fb5a07fb2e2d4fbb0`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba576338ed5242ba3fb838ce5fa930abb61e22fc422ba46b260dbca773cb9`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 4.8 MB (4772911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723eab0814ebbb502654a889ac99b52f2f7cb218a7164887ad0c9a1a5634d191`  
		Last Modified: Mon, 29 Jun 2020 20:18:31 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d3ac5a82f61292731263eecfe0635a4e0b486dd7f7f843a5cf9c1962fb54f1`  
		Last Modified: Mon, 29 Jun 2020 20:18:34 GMT  
		Size: 13.7 MB (13685965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18990846d9f6b2e03b43f0c42307982b5d13426a8d003425ce98e88c1ee61e9e`  
		Last Modified: Mon, 29 Jun 2020 20:18:30 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd85b14725d34f8e3d6505a3730098d0d983c7bfc436fab9f0025e28ea413c9`  
		Last Modified: Mon, 29 Jun 2020 20:18:30 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c83ec7d2b6fe2d3beb4121b8691686945da20d9398144840e2699dd7352378`  
		Last Modified: Mon, 29 Jun 2020 20:18:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7205b75fee4bcd79e0441081d0c18f4f16c9e3faddfbe44e9a2017d9c98e12`  
		Last Modified: Mon, 29 Jun 2020 20:18:29 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2d684094d65ac89815f73d6bb42fcc037bb91d14788f39d7c874f923010f78`  
		Last Modified: Mon, 29 Jun 2020 20:18:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d345ee36ca73380ffc59a00a9f9645c4be0f97bd3450083d5105bfb2456e5379`  
		Last Modified: Mon, 29 Jun 2020 20:18:27 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1399cf9fea037f4b40be192761883219e66d7fac0e8a7e53707b63894fd9a0a`  
		Last Modified: Mon, 29 Jun 2020 20:18:27 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abd79214efe888d78b44116335a0015f91de32819741eba80d9523b930ea548`  
		Last Modified: Mon, 29 Jun 2020 20:18:26 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1ac2c904ffff4f7f0d926f3fedbd61527aaf55aa38e88cde26c9d568962975`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108a4ea5a1055078abaa7e068c8d881cf36e81204a33175caff409d43aa0c9ce`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6c57249f136d38f7aa1045a8956c4f5f4c3f50d93bfb010221f45219da7dd5`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dec9ff0349ee91649d28733494db17d02470cf6a73f8268d7f3e717bb52f90`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c09a8d6df681bb92ae4ee08eb66e50aa8636527ebad60c50ee3917dd252a97`  
		Last Modified: Mon, 29 Jun 2020 20:18:22 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3888338b94e4b7f8a0a2eeb0c1724e90d743bddbbda11b28ed6a436cc0acc571`  
		Last Modified: Mon, 29 Jun 2020 20:18:22 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6ef034637a0be1fc8331c80eceeaba597da0bda3d9bb9769fde9678f401e9d`  
		Last Modified: Mon, 29 Jun 2020 20:18:22 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e84984fd0f42956c1dc9d31717a9fada1dfdf8e2cb00ce952e2655bf25249ce`  
		Last Modified: Mon, 29 Jun 2020 20:18:23 GMT  
		Size: 298.4 KB (298450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b4fdef44f059a30624268d4a303dc4436aada1655b41b5380dcdf6a1b925a7`  
		Last Modified: Mon, 29 Jun 2020 20:18:23 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:c9cc0726f345f76e464e535e972374668d02c30c224057e4f82e4186ae942ba6
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758382605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:150ecdbd7cbd511f1549e36fab065abcf44446cf7fcd58e45ceef61df883bf2b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:04:40 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:06:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 29 Jun 2020 20:15:40 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:17:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('360bade38fea4d0e87bf00f2dc0c7e7b4434bb020af49d189b2c424246710bf6a3074e486ef2c3d6994473bcd62393302a1a704c215b4e323eeaecbfa359a533')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 29 Jun 2020 20:17:05 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 29 Jun 2020 20:17:06 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 29 Jun 2020 20:17:07 GMT
VOLUME [c:/config]
# Mon, 29 Jun 2020 20:17:08 GMT
VOLUME [c:/data]
# Mon, 29 Jun 2020 20:17:09 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 20:17:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 20:17:11 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 20:17:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 20:17:12 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 20:17:13 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 20:17:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 20:17:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 20:17:16 GMT
EXPOSE 80
# Mon, 29 Jun 2020 20:17:17 GMT
EXPOSE 443
# Mon, 29 Jun 2020 20:17:18 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 20:17:58 GMT
RUN caddy version
# Mon, 29 Jun 2020 20:17:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22985925139cd6a6e83b6eb5286a8a6e1053a5c6ddd9762f34deea2aa6bcaacc`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43c028d6768e901bc64b3edb7e2e5f72050d3ed78ea4e7337fe85725d250c15`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 5.4 MB (5404509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae58d77a8d67f842374c3e60732465a9aaddfd9ce2b054b39aac0b7f2a420d0f`  
		Last Modified: Mon, 29 Jun 2020 20:18:56 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f76df30f6b9698ddedad69790139a9d2cf4fc871763691861f8aab018ac8ed`  
		Last Modified: Mon, 29 Jun 2020 20:19:01 GMT  
		Size: 18.7 MB (18718943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf3b4f088973e051021b74d9b9f795a9f2c8c71f7ae83e83f0cd6e95343f562`  
		Last Modified: Mon, 29 Jun 2020 20:18:56 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef3ce431d20a03b531eadce4cbe5680aca6c4ee4e24d70578687c89963b41d1`  
		Last Modified: Mon, 29 Jun 2020 20:18:55 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091019db4f4b75fe37b7b7ce991db4c4b02422388f836be3c4eb7c51159208b3`  
		Last Modified: Mon, 29 Jun 2020 20:18:54 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e080558fbf5cadbed8b34080d8bad08b45fff65ab533d87a24639d3ba6fd837f`  
		Last Modified: Mon, 29 Jun 2020 20:18:54 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc66481244327f616ca39ffe8c4b596d1aa9b7d778aa717e75b0b8f4a4c06350`  
		Last Modified: Mon, 29 Jun 2020 20:18:54 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f6e5557d697d57716bbf495fc701cef5b9073dbe5646f64fbbb0b8207fc07a`  
		Last Modified: Mon, 29 Jun 2020 20:18:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e238dae9de9d36d2c73796aa4c2a29645bbd5239ab47082579ccdc42e76244d8`  
		Last Modified: Mon, 29 Jun 2020 20:18:53 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbccba413742cc92bb8c53edd613f0be0250226ae8465165c5bc4e25a0c79a0`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911208ad8ab28008b96820a6251bee291bb5840e23ec782b1bbafdfe8019e08c`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2440198b129a0383b522e8b349ec26d2b66b1b33c422df3c3933be7c6591f661`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa72d9c6b7293c4d60c48fc5729c6f3a7eaa2f8276c8cba94bbb20edab126354`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a35778894255e6ba11c0d42ca54c80e69279c8777b609c7366208de7e0ac4c`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b99c2dfe7b1a527300bd8de8147e159f8ecdbab796e7a71c7dd3e2df8cf216`  
		Last Modified: Mon, 29 Jun 2020 20:18:48 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9969646e605208d0301ec4741756dd6257ac0991ed01bfde817b513b8e7a9e19`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2919689d5a48dd6e4ef39397ffed789e7ff54451a9abaadbc274574a363256e`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfa5d572d4b3ac461e8246a58be6e84431cc733d430cb532e99e83af335ded3`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 239.7 KB (239740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90df7192caf1a86dbf2f53b57375af83ea514b4128fc8040808368b6ae7fd815`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:42b2115a0f6b0c698531f3b41f61a85096377ad6f2bc9c7a967b5f7efaecf78b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:e8b1865dd51a79cddf1ce786b52156e81cbaf67046a24bd475a8115ab960445c
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2312693391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ddbcd3c45a5583a6c9b91d6672b879ac5fd94c25a88540d6ca81b52c37931de`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Tue, 09 Jun 2020 22:33:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:02:29 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:03:15 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 29 Jun 2020 20:14:27 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:14:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('360bade38fea4d0e87bf00f2dc0c7e7b4434bb020af49d189b2c424246710bf6a3074e486ef2c3d6994473bcd62393302a1a704c215b4e323eeaecbfa359a533')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 29 Jun 2020 20:15:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 29 Jun 2020 20:15:02 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 29 Jun 2020 20:15:03 GMT
VOLUME [c:/config]
# Mon, 29 Jun 2020 20:15:04 GMT
VOLUME [c:/data]
# Mon, 29 Jun 2020 20:15:05 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 20:15:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 20:15:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 20:15:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 20:15:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 20:15:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 20:15:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 20:15:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 20:15:11 GMT
EXPOSE 80
# Mon, 29 Jun 2020 20:15:12 GMT
EXPOSE 443
# Mon, 29 Jun 2020 20:15:13 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 20:15:29 GMT
RUN caddy version
# Mon, 29 Jun 2020 20:15:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f841c6a0c622cd36b5b2688011a224ac3e8e96273758f4a2804f2f3f099f267d`  
		Last Modified: Tue, 09 Jun 2020 23:17:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e676deb3766189ea2b008f69205017c9ee31a77f9c7001fb5a07fb2e2d4fbb0`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ba576338ed5242ba3fb838ce5fa930abb61e22fc422ba46b260dbca773cb9`  
		Last Modified: Wed, 10 Jun 2020 18:09:48 GMT  
		Size: 4.8 MB (4772911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723eab0814ebbb502654a889ac99b52f2f7cb218a7164887ad0c9a1a5634d191`  
		Last Modified: Mon, 29 Jun 2020 20:18:31 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d3ac5a82f61292731263eecfe0635a4e0b486dd7f7f843a5cf9c1962fb54f1`  
		Last Modified: Mon, 29 Jun 2020 20:18:34 GMT  
		Size: 13.7 MB (13685965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18990846d9f6b2e03b43f0c42307982b5d13426a8d003425ce98e88c1ee61e9e`  
		Last Modified: Mon, 29 Jun 2020 20:18:30 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd85b14725d34f8e3d6505a3730098d0d983c7bfc436fab9f0025e28ea413c9`  
		Last Modified: Mon, 29 Jun 2020 20:18:30 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c83ec7d2b6fe2d3beb4121b8691686945da20d9398144840e2699dd7352378`  
		Last Modified: Mon, 29 Jun 2020 20:18:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7205b75fee4bcd79e0441081d0c18f4f16c9e3faddfbe44e9a2017d9c98e12`  
		Last Modified: Mon, 29 Jun 2020 20:18:29 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2d684094d65ac89815f73d6bb42fcc037bb91d14788f39d7c874f923010f78`  
		Last Modified: Mon, 29 Jun 2020 20:18:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d345ee36ca73380ffc59a00a9f9645c4be0f97bd3450083d5105bfb2456e5379`  
		Last Modified: Mon, 29 Jun 2020 20:18:27 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1399cf9fea037f4b40be192761883219e66d7fac0e8a7e53707b63894fd9a0a`  
		Last Modified: Mon, 29 Jun 2020 20:18:27 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abd79214efe888d78b44116335a0015f91de32819741eba80d9523b930ea548`  
		Last Modified: Mon, 29 Jun 2020 20:18:26 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1ac2c904ffff4f7f0d926f3fedbd61527aaf55aa38e88cde26c9d568962975`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108a4ea5a1055078abaa7e068c8d881cf36e81204a33175caff409d43aa0c9ce`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6c57249f136d38f7aa1045a8956c4f5f4c3f50d93bfb010221f45219da7dd5`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dec9ff0349ee91649d28733494db17d02470cf6a73f8268d7f3e717bb52f90`  
		Last Modified: Mon, 29 Jun 2020 20:18:25 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c09a8d6df681bb92ae4ee08eb66e50aa8636527ebad60c50ee3917dd252a97`  
		Last Modified: Mon, 29 Jun 2020 20:18:22 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3888338b94e4b7f8a0a2eeb0c1724e90d743bddbbda11b28ed6a436cc0acc571`  
		Last Modified: Mon, 29 Jun 2020 20:18:22 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6ef034637a0be1fc8331c80eceeaba597da0bda3d9bb9769fde9678f401e9d`  
		Last Modified: Mon, 29 Jun 2020 20:18:22 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e84984fd0f42956c1dc9d31717a9fada1dfdf8e2cb00ce952e2655bf25249ce`  
		Last Modified: Mon, 29 Jun 2020 20:18:23 GMT  
		Size: 298.4 KB (298450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b4fdef44f059a30624268d4a303dc4436aada1655b41b5380dcdf6a1b925a7`  
		Last Modified: Mon, 29 Jun 2020 20:18:23 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:0f179ab33aa576db54d686130dcb5cfe8c3ce5f292f5bccc9fa16f1128bfc31f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:c9cc0726f345f76e464e535e972374668d02c30c224057e4f82e4186ae942ba6
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758382605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:150ecdbd7cbd511f1549e36fab065abcf44446cf7fcd58e45ceef61df883bf2b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Jun 2020 18:04:40 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 10 Jun 2020 18:06:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Mon, 29 Jun 2020 20:15:40 GMT
ENV CADDY_VERSION=v2.1.0
# Mon, 29 Jun 2020 20:17:02 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.0/caddy_2.1.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('360bade38fea4d0e87bf00f2dc0c7e7b4434bb020af49d189b2c424246710bf6a3074e486ef2c3d6994473bcd62393302a1a704c215b4e323eeaecbfa359a533')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 29 Jun 2020 20:17:05 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 29 Jun 2020 20:17:06 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 29 Jun 2020 20:17:07 GMT
VOLUME [c:/config]
# Mon, 29 Jun 2020 20:17:08 GMT
VOLUME [c:/data]
# Mon, 29 Jun 2020 20:17:09 GMT
LABEL org.opencontainers.image.version=v2.1.0
# Mon, 29 Jun 2020 20:17:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 29 Jun 2020 20:17:11 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 29 Jun 2020 20:17:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 29 Jun 2020 20:17:12 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 29 Jun 2020 20:17:13 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 29 Jun 2020 20:17:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 29 Jun 2020 20:17:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 29 Jun 2020 20:17:16 GMT
EXPOSE 80
# Mon, 29 Jun 2020 20:17:17 GMT
EXPOSE 443
# Mon, 29 Jun 2020 20:17:18 GMT
EXPOSE 2019
# Mon, 29 Jun 2020 20:17:58 GMT
RUN caddy version
# Mon, 29 Jun 2020 20:17:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22985925139cd6a6e83b6eb5286a8a6e1053a5c6ddd9762f34deea2aa6bcaacc`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43c028d6768e901bc64b3edb7e2e5f72050d3ed78ea4e7337fe85725d250c15`  
		Last Modified: Wed, 10 Jun 2020 18:10:17 GMT  
		Size: 5.4 MB (5404509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae58d77a8d67f842374c3e60732465a9aaddfd9ce2b054b39aac0b7f2a420d0f`  
		Last Modified: Mon, 29 Jun 2020 20:18:56 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f76df30f6b9698ddedad69790139a9d2cf4fc871763691861f8aab018ac8ed`  
		Last Modified: Mon, 29 Jun 2020 20:19:01 GMT  
		Size: 18.7 MB (18718943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf3b4f088973e051021b74d9b9f795a9f2c8c71f7ae83e83f0cd6e95343f562`  
		Last Modified: Mon, 29 Jun 2020 20:18:56 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef3ce431d20a03b531eadce4cbe5680aca6c4ee4e24d70578687c89963b41d1`  
		Last Modified: Mon, 29 Jun 2020 20:18:55 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091019db4f4b75fe37b7b7ce991db4c4b02422388f836be3c4eb7c51159208b3`  
		Last Modified: Mon, 29 Jun 2020 20:18:54 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e080558fbf5cadbed8b34080d8bad08b45fff65ab533d87a24639d3ba6fd837f`  
		Last Modified: Mon, 29 Jun 2020 20:18:54 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc66481244327f616ca39ffe8c4b596d1aa9b7d778aa717e75b0b8f4a4c06350`  
		Last Modified: Mon, 29 Jun 2020 20:18:54 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f6e5557d697d57716bbf495fc701cef5b9073dbe5646f64fbbb0b8207fc07a`  
		Last Modified: Mon, 29 Jun 2020 20:18:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e238dae9de9d36d2c73796aa4c2a29645bbd5239ab47082579ccdc42e76244d8`  
		Last Modified: Mon, 29 Jun 2020 20:18:53 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbccba413742cc92bb8c53edd613f0be0250226ae8465165c5bc4e25a0c79a0`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911208ad8ab28008b96820a6251bee291bb5840e23ec782b1bbafdfe8019e08c`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2440198b129a0383b522e8b349ec26d2b66b1b33c422df3c3933be7c6591f661`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa72d9c6b7293c4d60c48fc5729c6f3a7eaa2f8276c8cba94bbb20edab126354`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a35778894255e6ba11c0d42ca54c80e69279c8777b609c7366208de7e0ac4c`  
		Last Modified: Mon, 29 Jun 2020 20:18:51 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b99c2dfe7b1a527300bd8de8147e159f8ecdbab796e7a71c7dd3e2df8cf216`  
		Last Modified: Mon, 29 Jun 2020 20:18:48 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9969646e605208d0301ec4741756dd6257ac0991ed01bfde817b513b8e7a9e19`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2919689d5a48dd6e4ef39397ffed789e7ff54451a9abaadbc274574a363256e`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfa5d572d4b3ac461e8246a58be6e84431cc733d430cb532e99e83af335ded3`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 239.7 KB (239740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90df7192caf1a86dbf2f53b57375af83ea514b4128fc8040808368b6ae7fd815`  
		Last Modified: Mon, 29 Jun 2020 20:18:49 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
