## `caddy:latest`

```console
$ docker pull caddy@sha256:b3a7eac3daba82e1d682a7fa3f11b6d0dbe32869cdcc835fd30748021fbe3b9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4851; amd64
	-	windows version 10.0.20348.1970; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:733fe94133c4bd22c6ee8f9b9802bce8fede5e7b766bebde205a45dd4ac04aea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.4 MB (18363908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1e1b7ae170b7d7d7e524717fe978e0090023cc82a7d9ffe48e344b0351a3ee1`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:09:18 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 18:20:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:19:38 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:19:41 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:19:41 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:19:41 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:19:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:19:42 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:19:42 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:19:42 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:19:42 GMT
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
	-	`sha256:29b3b3e68e52dc5ab939c72a9bbac39cff4bef4b87de399ddf28657471df6845`  
		Last Modified: Mon, 14 Aug 2023 18:20:42 GMT  
		Size: 7.5 KB (7502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c55d3259542348ddb70edc18dda7d48aeca5654962aed568a7034f3667d2ca`  
		Last Modified: Thu, 17 Aug 2023 22:20:10 GMT  
		Size: 14.6 MB (14603949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:dd029220558032e5d1f91173d32a0078dad12ec9b5114bef422ed4cdf05dec52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17314204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1de0523ee8d8173472fb08aa9a74a37bcd054af2b796b7631d847ba8a46986b5`
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
# Thu, 17 Aug 2023 22:49:12 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:49:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:49:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:49:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:49:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:49:17 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:49:17 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:49:17 GMT
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
	-	`sha256:82560a340155261ecbd1d99d87890c5aa0cfd64d571e1dcafc03e3b6a8132d48`  
		Last Modified: Thu, 17 Aug 2023 22:49:41 GMT  
		Size: 13.8 MB (13814204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:24649e9de43354963118f9cdf6ad1f4522c6993735f316763a2f5d1f76cba267
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17042831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb4a48fd29d50802cbf030949e2c9767eb6888e8412330f64246f322bc3b49c`
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
# Thu, 17 Aug 2023 22:57:18 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:57:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:57:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:57:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:57:22 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:57:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:57:23 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:57:24 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:57:24 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:57:24 GMT
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
	-	`sha256:5879767a5d1969beb154b9a4991a767b0ed5be0c9739a972f07d03e825312fa5`  
		Last Modified: Thu, 17 Aug 2023 22:57:51 GMT  
		Size: 13.8 MB (13791384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:ed967fcd1968be6dc4699ff835cdd2d6f3f49105b9677f878c8a6960fd1a0643
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 MB (17162547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed7b6600470cab547aa1090baa39a6192ec83119989884ac742a63ed23be3da2`
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
# Thu, 17 Aug 2023 22:39:17 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:39:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:39:19 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:39:19 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:39:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:39:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:39:20 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:39:20 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:39:20 GMT
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
	-	`sha256:597bfc484ba18727d2df98120cb9d559f346ade9e3a23be6a9af3e76dca89edd`  
		Last Modified: Thu, 17 Aug 2023 22:39:42 GMT  
		Size: 13.5 MB (13463635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:c3679836562d0252e6341a112d2729b8dae0eae550449bfe91fe2798171fd4ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16944934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc5ac831dce746cd0f4448640b7edaf0ce9457d09618e246ba72ee76ea63dcbe`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:44:14 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Mon, 14 Aug 2023 18:18:00 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"
# Thu, 17 Aug 2023 22:16:24 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:16:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:16:29 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:16:29 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:16:29 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:16:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:16:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:16:31 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:16:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:16:32 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:16:33 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:16:33 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:16:34 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:16:34 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:16:35 GMT
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
	-	`sha256:7d19953b5eb53ddaa0e25905527dc138e0c4111467bb7d71f81fa94976091351`  
		Last Modified: Mon, 14 Aug 2023 18:18:54 GMT  
		Size: 7.5 KB (7509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf4bf695323732c5ce84bbb0b976c5cd981eaf6814515a86f521af4a0e64582`  
		Last Modified: Thu, 17 Aug 2023 22:17:22 GMT  
		Size: 13.2 MB (13229001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:ca7ab0dcf4ab146df48cfa8ae6e07fed804feeed4a36358fa652c8eac52b40da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17720356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d4d019ffc0cd69ea8c5d3b8fb0a39c89d3aa1b2037c1012a9ba4bed6abb94dc`
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
# Thu, 17 Aug 2023 22:41:35 GMT
ENV CADDY_VERSION=v2.7.4
# Thu, 17 Aug 2023 22:41:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='68cc53c79b88da5f1a33f5a1e1da7fbac5ad041380e91e27663b44e0cb2d8e07e08690295e86e9e65a37472b52f7d95f84f383ee0b8f3d5e1bd4b755d3990e6a' ;; 		armhf)   binArch='armv6'; checksum='e6db35a9a2d78a8375d287bb1e4dc37f21eeadd5e41ad0c4adc2e35d3f80e061602d3e9c498ac4a4956754ad7be8c5f0489395db2c9729782906d771e528c898' ;; 		armv7)   binArch='armv7'; checksum='5e94a538e9f9d62da2cdfae04294e943800ced348a66fad13ab6c99aa8184485a1ceba2dbcf13d996f4a4bad1a49e2774b880182b0edcf1a112b1001c552e424' ;; 		aarch64) binArch='arm64'; checksum='eb9be2b3d09351d97843a4e2b73f36a4d36d3cb689dd580b5706b243fb66d0dc8a04460fd4a87dea772442c9fe7a1cddb0022e085be663f3d1e12127e3295d9d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3accb7bbfe23d33057bf023951b3ccddd4cf1708314adad71aa2f298581da293af1bc817ff346248c895499908de7ced661f64a4d115b41657630e14cc8f62a7' ;; 		s390x)   binArch='s390x'; checksum='73c4961582ddc4a0d013c7af85642cf68a7bb0069e04aabba28ff3270f86853b394277d90b7b971695b949087e8d3fb50661da03953e632705e3f63c6e7acdb8' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 17 Aug 2023 22:41:39 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 17 Aug 2023 22:41:39 GMT
ENV XDG_DATA_HOME=/data
# Thu, 17 Aug 2023 22:41:39 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 17 Aug 2023 22:41:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 17 Aug 2023 22:41:40 GMT
EXPOSE 80
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 443
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 443/udp
# Thu, 17 Aug 2023 22:41:41 GMT
EXPOSE 2019
# Thu, 17 Aug 2023 22:41:41 GMT
WORKDIR /srv
# Thu, 17 Aug 2023 22:41:41 GMT
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
	-	`sha256:2394cd7c9416df19c45596c558f5a7ee05adc5a7fd166f58dcbf26f1ac6ecae6`  
		Last Modified: Thu, 17 Aug 2023 22:42:16 GMT  
		Size: 14.1 MB (14143708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.4851; amd64

```console
$ docker pull caddy@sha256:3f230e8c687c5611e74c84c3ec6f7ef7844b3cc3443d9302e9bb778e6210bfe2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2032252342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea189389e39a38d33c2124e3c02e0a9bc2f3168e5605fa8a909e749ac52fc3f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:30:52 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:30:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:32:00 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:32:01 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:32:02 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:32:03 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:32:04 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:32:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:32:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:32:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:32:08 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:32:09 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:32:10 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:33:07 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:33:07 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2bc90334de89082943edb24d5f52a3bb36ef134c17a417ba45cc4e122be3b2`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 465.0 KB (465015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba1c9fb8dedf070862eb0526393862bb5a0f2c87a87bc3864b9b24b11af5524`  
		Last Modified: Wed, 13 Sep 2023 05:37:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5249ade277243b1b7f8c198de7d036f2e106b8a679d777b7bfc885af7b9b76`  
		Last Modified: Wed, 13 Sep 2023 05:37:46 GMT  
		Size: 15.2 MB (15176891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224a0aed4c02b4a48f633ac01c40e020d4e8fbc32fe8896d93032f9d72f50cda`  
		Last Modified: Wed, 13 Sep 2023 05:37:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fc1c10b7da22b1e9a26f059801a53ce4ce22e7d24ab14ec56d343a806f3bc2`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bd26e7302c16a8d83a8a6b5d9d263b804279f2b4c7d2fcea59a97c1e187648`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f69e667aa7c5e5a21f7d8a8cdd213b9d20a8a0c790dd18fe51d4df9e5b08a7`  
		Last Modified: Wed, 13 Sep 2023 05:37:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e456b9da79a468c972d487e55e3628f8a8917f78948550c359afc891a5ad24a`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bc4af3e90793180c1ed8b8b9ac6866e24a5de16881f363dacf0ecf47396c8`  
		Last Modified: Wed, 13 Sep 2023 05:37:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0289dff328d597d94fcd8612bd4a726573e13f780790744c5c6f4b40b49823`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b52ff2438c88a58e8be33368f668557c92bcfdc503bd58025d081c7b88ec88b`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0f1c855afa9fd7bcf5ded632c161f2ff013f4b08f5c233fa3bdf3d13701467`  
		Last Modified: Wed, 13 Sep 2023 05:37:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2e0bf79eee4bbd609b5a111793e394f22ad86eb897cf85c6df2c45d9a8d777`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff797288117550c2b80f9a39dd5a04cb449defc2660cf6a7589618b8d3606464`  
		Last Modified: Wed, 13 Sep 2023 05:37:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa0d1665270ae2e22844b2386842b1deab36f8936506db82df0ec69dc72fb84`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867297eb9d01dfe100695ae10a0c67bd38f2124de0ee7446d1e66b6dede5c06`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee97f69cfbd31f5a098d45934b159384d8e986d860ad3007140beee338aa4533`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b741c4ffade19f3d712c3fb839c3ae7f1ae4e39e5f777a2b24917b5e630d0f86`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 256.7 KB (256675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a415b22709a225227fa7ce65d7767f3f820c7e9e445b0d718dfb68ae2249832`  
		Last Modified: Wed, 13 Sep 2023 05:37:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.20348.1970; amd64

```console
$ docker pull caddy@sha256:76214fe6feb9f96f1c46334c01e1b9d310eb2e745bb08ba4130547b2147f3677
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1853253940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f0e585ea0797bdd13d148afed1e86161022e8cf2a79d11337f9d4dde0a8efe6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:33:51 GMT
RUN mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/0c7fa00a87c65a6ef47ed36d841cd223682a2a2c/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Sep 2023 05:33:52 GMT
ENV CADDY_VERSION=v2.7.4
# Wed, 13 Sep 2023 05:34:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.7.4/caddy_2.7.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3bb648c05fed64e6a4815275b92c179d4b6dac4ff34f383cd59e94cde8842aee9c9c14e1334d7f3a0ccf9ac43c96252e4c9e4b6fcca32f7950285379137ab06')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Sep 2023 05:34:25 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Sep 2023 05:34:26 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Sep 2023 05:34:27 GMT
LABEL org.opencontainers.image.version=v2.7.4
# Wed, 13 Sep 2023 05:34:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Sep 2023 05:34:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Sep 2023 05:34:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Sep 2023 05:34:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Sep 2023 05:34:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Sep 2023 05:34:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Sep 2023 05:34:33 GMT
EXPOSE 80
# Wed, 13 Sep 2023 05:34:34 GMT
EXPOSE 443
# Wed, 13 Sep 2023 05:34:35 GMT
EXPOSE 443/udp
# Wed, 13 Sep 2023 05:34:36 GMT
EXPOSE 2019
# Wed, 13 Sep 2023 05:34:56 GMT
RUN caddy version
# Wed, 13 Sep 2023 05:34:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2d313a26784edb67b74292171891c0393ea119a53238e09150b5b7bc52371f`  
		Last Modified: Wed, 13 Sep 2023 05:38:08 GMT  
		Size: 483.0 KB (482985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb50376a60c42178e92d96a048b0e7f2dbc2cafe73274ab76722cda86fb32ee`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeecad99d9c5b378a623153b24130f8c36442e9a48ef6a48f878c5f585a66bd4`  
		Last Modified: Wed, 13 Sep 2023 05:38:11 GMT  
		Size: 15.2 MB (15183860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6b7a19981a71c15e39afbc3a52ed5f0c065f77c1ccd55a88e5f1b51af88753`  
		Last Modified: Wed, 13 Sep 2023 05:38:07 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd7340889e9a6bfc8018c7709595b75ef962cf2608d14398ffbc90b90804a04`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7537acdfe48467d248afb6a69dad6bdb09c62617600305d2b2adb8a45ece2f`  
		Last Modified: Wed, 13 Sep 2023 05:38:06 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf3cb277ba29189d90269123acd401fa787771fb095f2f2ec532be7bba2a025`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64eb5cc4069279b73a665e35bf526fa42558af1a3a71fc13d76913846d96818`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74348cf2ecbfe3a00df246034f9ab755418e8584b24113c9d327fc80cb134829`  
		Last Modified: Wed, 13 Sep 2023 05:38:05 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa3fef62dce81d37fff2c621b94314d2aa9d0318523407b0a1d7d2b1e079234`  
		Last Modified: Wed, 13 Sep 2023 05:38:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d033d5a006e7fa969026194ef48446c840a891ad252f0316d32bc01843f0e4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbef09c0840262b42ba39068c868fc9b353bed78bb7de251e953289149e9a64e`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea46de371cf13fdb02566c79fc3a22c7123bd7c8903d20645b9cfe34f7ca85d4`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63cdcd333c2c131733511c6750d4154ea7f097d981934d1dda8944bf2840860`  
		Last Modified: Wed, 13 Sep 2023 05:38:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8259824bfebcdadd0448ccc0a815b7257636f6eb420e7e00216359908281e7b`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51874919dc1cfa2121d50499f839a702c4cd7340e8708e90b2af042e9debba9`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee3a41ffde2d883c73932756f176ba6901eaeb7a680a351a2b476398263cc8`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73e8028e6f79476106af6c347aa4765644a8ed828c5b6c117ee3dcc2e22e1ef`  
		Last Modified: Wed, 13 Sep 2023 05:38:02 GMT  
		Size: 289.2 KB (289194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd87253476a12fff6cbe718338261ef5ec78a1eb19d8e222838e7f96c3100a0`  
		Last Modified: Wed, 13 Sep 2023 05:38:01 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
